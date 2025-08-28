<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Worldwide Marriage Encounter - Fiji</title>
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css">
    <style>
        /* General Styles */
        * {
            box-sizing: border-box;
            margin: 0;
            padding: 0;
        }
        
        body {
            font-family: 'Arial', sans-serif;
            margin: 0;
            padding: 0;
            background-color: #f4f4f4;
            color: #333;
            text-align: center;
            line-height: 1.6;
        }

        /* Header */
        header {
            background: linear-gradient(to right, #8e3c3c, #6b2b2b);
            color: white;
            padding: 3rem 2rem;
            position: relative;
            overflow: hidden;
        }

        header::before {
            content: "";
            position: absolute;
            top: 0;
            left: 0;
            width: 100%;
            height: 100%;
            background-image: url('data:image/svg+xml;utf8,<svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 100 100" width="100" height="100" opacity="0.1"><circle cx="50" cy="50" r="40" fill="white" /></svg>');
            opacity: 0.1;
        }

        header h1 {
            margin: 0;
            font-size: 2.8rem;
            text-shadow: 2px 2px 4px rgba(0, 0, 0, 0.3);
            animation: fadeIn 1.5s ease;
        }

        header p {
            font-size: 1.3rem;
            max-width: 800px;
            margin: 1rem auto;
            animation: fadeIn 2s ease;
        }

        /* Navigation */
        nav {
            background: #6b2b2b;
            padding: 1.2rem;
            position: sticky;
            top: 0;
            z-index: 100;
            box-shadow: 0 2px 10px rgba(0, 0, 0, 0.2);
        }

        nav a {
            color: white;
            text-decoration: none;
            margin: 0 15px;
            font-weight: bold;
            transition: all 0.3s ease;
            padding: 8px 15px;
            border-radius: 4px;
        }

        nav a:hover, nav a.active {
            background-color: rgba(255, 255, 255, 0.2);
            text-decoration: none;
        }

        /* Mobile Navigation */
        .menu-toggle {
            display: none;
            background: none;
            border: none;
            color: white;
            font-size: 1.5rem;
            cursor: pointer;
        }

        /* Content Sections */
        .section {
            padding: 3rem 2rem;
            max-width: 1000px;
            margin: auto;
            text-align: left;
            background: white;
            margin-top: 30px;
            border-radius: 10px;
            box-shadow: 0 5px 15px rgba(0,0,0,0.1);
            transition: transform 0.3s ease;
        }

        .section:hover {
            transform: translateY(-5px);
        }

        .section h2 {
            color: #8e3c3c;
            margin-bottom: 1.5rem;
            padding-bottom: 0.5rem;
            border-bottom: 2px solid #f4f4f4;
            font-size: 2rem;
        }

        /* About Section */
        .about-content {
            display: flex;
            flex-wrap: wrap;
            gap: 2rem;
            align-items: center;
            margin-top: 1.5rem;
        }

        .about-text {
            flex: 1;
            min-width: 300px;
        }

        .about-image {
            flex: 1;
            min-width: 300px;
            height: 300px;
            background: linear-gradient(45deg, #8e3c3c, #6b2b2b);
            border-radius: 10px;
            display: flex;
            align-items: center;
            justify-content: center;
            color: white;
            font-size: 1.5rem;
            text-align: center;
            padding: 1rem;
        }

        /* Events Section */
        .event-highlight {
            background-color: #f9f3f3;
            padding: 1.5rem;
            border-radius: 8px;
            margin: 1.5rem 0;
            border-left: 4px solid #8e3c3c;
        }

        .gallery {
            display: flex;
            flex-wrap: wrap;
            gap: 1rem;
            margin: 1.5rem 0;
            justify-content: center;
        }

        .gallery-item {
            flex: 1;
            min-width: 200px;
            height: 150px;
            background: #ddd;
            border-radius: 8px;
            overflow: hidden;
            position: relative;
        }

        .gallery-item::before {
            content: "";
            position: absolute;
            top: 0;
            left: 0;
            width: 100%;
            height: 100%;
            background: linear-gradient(45deg, #8e3c3c, #6b2b2b);
            opacity: 0.7;
        }

        .gallery-item:nth-child(2)::before {
            background: linear-gradient(45deg, #3c8e6b, #2b6b50);
        }

        .gallery-item:nth-child(3)::before {
            background: linear-gradient(45deg, #3c6b8e, #2b4c6b);
        }

        /* Contact Form */
        .contact-form {
            margin-top: 1.5rem;
        }

        .form-group {
            margin-bottom: 1.5rem;
            text-align: left;
        }

        .form-group label {
            display: block;
            margin-bottom: 0.5rem;
            font-weight: bold;
            color: #555;
        }

        .form-group input,
        .form-group textarea,
        .form-group select {
            width: 100%;
            padding: 12px;
            border: 1px solid #ddd;
            border-radius: 4px;
            font-family: inherit;
            font-size: 1rem;
        }

        .form-group textarea {
            min-height: 150px;
            resize: vertical;
        }

        /* Footer */
        footer {
            background: #333;
            color: white;
            padding: 2rem 1rem;
            margin-top: 3rem;
        }

        .footer-content {
            max-width: 1000px;
            margin: auto;
            display: flex;
            flex-wrap: wrap;
            justify-content: space-between;
            gap: 2rem;
        }

        .footer-section {
            flex: 1;
            min-width: 250px;
            text-align: left;
        }

        .footer-section h3 {
            margin-bottom: 1rem;
            color: #f9f3f3;
            border-bottom: 1px solid #555;
            padding-bottom: 0.5rem;
        }

        .social-links a {
            color: white;
            font-size: 1.5rem;
            margin-right: 1rem;
            transition: color 0.3s ease;
        }

        .social-links a:hover {
            color: #8e3c3c;
        }

        /* Button Style */
        .btn {
            display: inline-block;
            background: #8e3c3c;
            color: white;
            padding: 12px 25px;
            border-radius: 5px;
            text-decoration: none;
            margin-top: 10px;
            font-weight: bold;
            border: none;
            cursor: pointer;
            transition: all 0.3s ease;
        }

        .btn:hover {
            background: #6b2b2b;
            transform: translateY(-2px);
            box-shadow: 0 5px 15px rgba(0,0,0,0.1);
        }

        .btn-large {
            padding: 15px 30px;
            font-size: 1.1rem;
        }

        /* Animations */
        @keyframes fadeIn {
            from { opacity: 0; transform: translateY(20px); }
            to { opacity: 1; transform: translateY(0); }
        }

        /* Responsive Design */
        @media (max-width: 768px) {
            header h1 {
                font-size: 2.2rem;
            }
            
            header p {
                font-size: 1.1rem;
            }
            
            nav {
                padding: 1rem;
            }
            
            nav a {
                display: block;
                margin: 10px 0;
            }
            
            .nav-links {
                display: none;
            }
            
            .menu-toggle {
                display: block;
                position: absolute;
                top: 15px;
                right: 20px;
            }
            
            .nav-active {
                display: block;
            }
            
            .section {
                padding: 2rem 1.5rem;
            }
        }
    </style>
</head>
<body>
    <header id="home">
        <h1>Worldwide Marriage Encounter Fiji</h1>
        <p>Strengthening Marriages · Building Community · Renewing the Church</p>
    </header>

    <nav>
        <button class="menu-toggle" id="menuToggle">
            <i class="fas fa-bars"></i>
        </button>
        <div class="nav-links" id="navLinks">
            <a href="#home" class="active">Home</a>
            <a href="#about">About</a>
            <a href="#events">Events</a>
            <a href="#contact">Contact</a>
        </div>
    </nav>

    <div class="section" id="home-content">
        <h2>Welcome</h2>
        <p>Worldwide Marriage Encounter invites couples to experience deeper communication and a stronger relationship through faith-based retreats right here in Fiji.</p>
        <p>Join us to reconnect, reflect, and renew your marriage covenant. Our weekends are designed to help couples communicate more effectively, deepen their commitment, and strengthen their relationship with God and each other.</p>
        <a href="#contact" class="btn">Learn More</a>
    </div>

    <div class="section" id="about">
        <h2>About Us</h2>
        <div class="about-content">
            <div class="about-text">
                <p>Marriage Encounter is a Catholic-based movement that offers married couples the opportunity to spend time together away from the busyness of the world to focus on each other.</p>
                <p>Our mission is to proclaim the value of marriage and holy family life through Christ. Since our founding, we have helped thousands of couples worldwide rediscover the joy in their relationships.</p>
                <p>In Fiji, we've been serving the community for over 15 years, offering weekend retreats that combine spiritual growth with practical relationship tools.</p>
            </div>
            <div class="about-image">
                <div>Strengthening Fijian Marriages Since 2008</div>
            </div>
        </div>
    </div>

    <div class="section" id="events">
        <h2>Upcoming Events</h2>
        <p>Our next Marriage Encounter Weekend will be held in <strong>Suva, Fiji</strong> on:</p>
        
        <div class="event-highlight">
            <p><strong>Date:</strong> October 15-17, 2025</p>
            <p><strong>Location:</strong> Pacific Conference Center</p>
            <p><strong>Theme:</strong> "Renewing Your Covenant: Love in Action"</p>
        </div>
        
        <p>This weekend retreat includes guided discussions, private couple reflection time, and spiritual activities designed to strengthen your marriage.</p>
        
        <h3>What Past Participants Say</h3>
        <p>"This weekend transformed our communication and brought us closer than we've been in years." - Maria and Josefa R.</p>
        
        <div class="gallery">
            <div class="gallery-item"></div>
            <div class="gallery-item"></div>
            <div class="gallery-item"></div>
        </div>
        
        <a href="#contact" class="btn btn-large">Register Now</a>
    </div>

    <div class="section" id="contact">
        <h2>Contact Us</h2>
        <p>Have questions or want to learn more? Reach out to us!</p>
        
        <div class="contact-info">
            <p><i class="fas fa-envelope"></i> Email: <strong>fiji@wwme.org</strong></p>
            <p><i class="fas fa-phone"></i> Phone: <strong>+679 123 4567</strong></p>
            <p><i class="fas fa-map-marker-alt"></i> Address: Catholic Archdiocese of Suva, Fiji</p>
        </div>
        
        <div class="contact-form">
            <h3>Send us a Message</h3>
            <form id="contactForm">
                <div class="form-group">
                    <label for="name">Your Name</label>
                    <input type="text" id="name" required>
                </div>
                <div class="form-group">
                    <label for="email">Email Address</label>
                    <input type="email" id="email" required>
                </div>
                <div class="form-group">
                    <label for="subject">Subject</label>
                    <select id="subject">
                        <option value="general">General Inquiry</option>
                        <option value="registration">Event Registration</option>
                        <option value="volunteer">Volunteering</option>
                        <option value="donation">Making a Donation</option>
                    </select>
                </div>
                <div class="form-group">
                    <label for="message">Your Message</label>
                    <textarea id="message" required></textarea>
                </div>
                <button type="submit" class="btn">Send Message</button>
            </form>
        </div>
    </div>

    <footer>
        <div class="footer-content">
            <div class="footer-section">
                <h3>Worldwide Marriage Encounter Fiji</h3>
                <p>Dedicated to strengthening marriages throughout Fiji through faith-based retreats and ongoing community support.</p>
            </div>
            <div class="footer-section">
                <h3>Quick Links</h3>
                <p><a href="#home" style="color: white;">Home</a></p>
                <p><a href="#about" style="color: white;">About</a></p>
                <p><a href="#events" style="color: white;">Events</a></p>
                <p><a href="#contact" style="color: white;">Contact</a></p>
            </div>
            <div class="footer-section">
                <h3>Connect With Us</h3>
                <div class="social-links">
                    <a href="#"><i class="fab fa-facebook"></i></a>
                    <a href="#"><i class="fab fa-instagram"></i></a>
                    <a href="#"><i class="fab fa-twitter"></i></a>
                    <a href="#"><i class="fab fa-youtube"></i></a>
                </div>
                <p>Subscribe to our newsletter for updates</p>
            </div>
        </div>
        <p style="margin-top: 2rem;">© 2025 Worldwide Marriage Encounter Fiji. All Rights Reserved.</p>
        <p>Part of the Worldwide Marriage Encounter International Community</p>
    </footer>

    <script>
        // Mobile menu toggle
        document.getElementById('menuToggle').addEventListener('click', function() {
            document.getElementById('navLinks').classList.toggle('nav-active');
        });
        
        // Smooth scrolling for navigation links
        document.querySelectorAll('nav a').forEach(anchor => {
            anchor.addEventListener('click', function(e) {
                e.preventDefault();
                
                const targetId = this.getAttribute('href');
                const targetElement = document.querySelector(targetId);
                
                window.scrollTo({
                    top: targetElement.offsetTop - 60,
                    behavior: 'smooth'
                });
                
                // Update active class
                document.querySelectorAll('nav a').forEach(link => link.classList.remove('active'));
                this.classList.add('active');
            });
        });
        
        // Simple form validation
        document.getElementById('contactForm').addEventListener('submit', function(e) {
            e.preventDefault();
            alert('Thank you for your message! We will get back to you soon.');
            this.reset();
        });
        
        // Update active nav link on scroll
        window.addEventListener('scroll', function() {
            const sections = document.querySelectorAll('.section');
            const navLinks = document.querySelectorAll('nav a');
            
            let current = '';
            
            sections.forEach(section => {
                const sectionTop = section.offsetTop;
                const sectionHeight = section.clientHeight;
                
                if (pageYOffset >= (sectionTop - 100)) {
                    current = section.getAttribute('id');
                }
            });
            
            navLinks.forEach(link => {
                link.classList.remove('active');
                if (link.getAttribute('href') === '#' + current) {
                    link.classList.add('active');
                }
            });
        });
    </script>
</body>
</html>
