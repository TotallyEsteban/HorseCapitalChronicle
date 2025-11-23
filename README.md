<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Horse Capital Chronicle | Where Luxury Meets Equestrianism</title>
    <style>
        @import url('https://fonts.googleapis.com/css2?family=Playfair+Display:wght@400;500;600;700;800&family=Lato:wght@300;400;700;900&display=swap');
        
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }
        
        body {
            background: #ffffff;
            color: #1a1a1a;
            font-family: 'Lato', sans-serif;
            line-height: 1.6;
        }
        
        h1, h2, h3, h4 {
            font-family: 'Playfair Display', serif;
            font-weight: 400;
        }
        
        .container {
            max-width: 1400px;
            margin: 0 auto;
            padding: 0 40px;
        }
        
        /* Navigation */
        nav {
            position: fixed;
            top: 0;
            width: 100%;
            background: rgba(255, 255, 255, 0.98);
            backdrop-filter: blur(10px);
            border-bottom: 1px solid #e5e5e5;
            z-index: 1000;
            padding: 20px 0;
        }
        
        nav .container {
            display: flex;
            justify-content: space-between;
            align-items: center;
        }
        
        .logo {
            font-family: 'Playfair Display', serif;
            font-size: 1.8rem;
            font-weight: 700;
            color: #1a1a1a;
            letter-spacing: 1px;
        }
        
        .nav-links {
            display: flex;
            gap: 48px;
            align-items: center;
        }
        
        .nav-links a {
            text-decoration: none;
            color: #1a1a1a;
            font-size: 13px;
            letter-spacing: 1px;
            text-transform: uppercase;
            font-weight: 400;
            transition: opacity 0.3s;
        }
        
        .nav-links a:hover {
            opacity: 0.6;
        }
        
        .btn {
            padding: 12px 28px;
            background: #1a1a1a;
            color: #ffffff;
            border: none;
            font-size: 11px;
            letter-spacing: 1.5px;
            text-transform: uppercase;
            cursor: pointer;
            transition: all 0.3s;
            text-decoration: none;
            display: inline-block;
        }
        
        .btn:hover {
            background: #333;
        }
        
        /* Hero */
        .hero {
            padding: 140px 40px 80px;
            background: linear-gradient(to bottom, #f8f8f8 0%, #ffffff 100%);
            text-align: center;
        }
        
        .hero-content {
            max-width: 900px;
            margin: 0 auto;
        }
        
        .hero-badge {
            font-size: 11px;
            letter-spacing: 2px;
            text-transform: uppercase;
            color: #666;
            margin-bottom: 32px;
        }
        
        h1 {
            font-size: 5.5rem;
            line-height: 1.1;
            margin-bottom: 32px;
            font-weight: 400;
            letter-spacing: -1px;
        }
        
        .hero-subtitle {
            font-size: 1.3rem;
            color: #666;
            margin-bottom: 48px;
            font-weight: 300;
            line-height: 1.8;
        }
        
        .divider {
            width: 60px;
            height: 1px;
            background: #1a1a1a;
            margin: 48px auto;
        }
        
        /* Featured Content */
        .featured {
            padding: 100px 40px;
        }
        
        .featured-grid {
            display: grid;
            grid-template-columns: 2fr 1fr;
            gap: 40px;
            margin-top: 60px;
        }
        
        .featured-main {
            position: relative;
            overflow: hidden;
        }
        
        .featured-image {
            width: 100%;
            height: 600px;
            background: #f0f0f0;
            display: flex;
            align-items: center;
            justify-content: center;
            color: #999;
            font-size: 14px;
            letter-spacing: 2px;
        }
        
        .featured-content {
            padding: 32px 0;
        }
        
        .category {
            font-size: 11px;
            letter-spacing: 2px;
            text-transform: uppercase;
            color: #999;
            margin-bottom: 16px;
        }
        
        h2 {
            font-size: 3rem;
            line-height: 1.2;
            margin-bottom: 20px;
            font-weight: 400;
        }
        
        h3 {
            font-size: 1.8rem;
            line-height: 1.3;
            margin-bottom: 16px;
            font-weight: 400;
        }
        
        .excerpt {
            font-size: 1.05rem;
            color: #666;
            line-height: 1.8;
            margin-bottom: 24px;
        }
        
        .read-more {
            font-size: 12px;
            letter-spacing: 1.5px;
            text-transform: uppercase;
            color: #1a1a1a;
            text-decoration: none;
            border-bottom: 1px solid #1a1a1a;
            padding-bottom: 2px;
            transition: opacity 0.3s;
        }
        
        .read-more:hover {
            opacity: 0.6;
        }
        
        .featured-sidebar {
            display: flex;
            flex-direction: column;
            gap: 40px;
        }
        
        .sidebar-item {
            border-bottom: 1px solid #e5e5e5;
            padding-bottom: 32px;
        }
        
        .sidebar-item:last-child {
            border-bottom: none;
        }
        
        .sidebar-image {
            width: 100%;
            height: 250px;
            background: #f0f0f0;
            margin-bottom: 20px;
            display: flex;
            align-items: center;
            justify-content: center;
            color: #999;
            font-size: 12px;
        }
        
        /* Content Pillars */
        .pillars {
            padding: 100px 40px;
            background: #f8f8f8;
        }
        
        .section-header {
            text-align: center;
            margin-bottom: 80px;
        }
        
        .section-title {
            font-size: 3rem;
            margin-bottom: 20px;
        }
        
        .section-subtitle {
            font-size: 1.1rem;
            color: #666;
            font-weight: 300;
        }
        
        .pillars-grid {
            display: grid;
            grid-template-columns: repeat(4, 1fr);
            gap: 40px;
        }
        
        .pillar-card {
            text-align: center;
            padding: 40px 20px;
            background: #ffffff;
            transition: transform 0.3s;
        }
        
        .pillar-card:hover {
            transform: translateY(-8px);
        }
        
        .pillar-icon {
            font-size: 3rem;
            margin-bottom: 24px;
        }
        
        .pillar-title {
            font-size: 1.3rem;
            margin-bottom: 16px;
        }
        
        .pillar-desc {
            font-size: 14px;
            color: #666;
            line-height: 1.7;
        }
        
        /* Latest Stories */
        .latest {
            padding: 100px 40px;
        }
        
        .stories-grid {
            display: grid;
            grid-template-columns: repeat(3, 1fr);
            gap: 48px;
            margin-top: 60px;
        }
        
        .story-card {
            text-decoration: none;
            color: inherit;
            display: block;
        }
        
        .story-image {
            width: 100%;
            height: 320px;
            background: #f0f0f0;
            margin-bottom: 24px;
            display: flex;
            align-items: center;
            justify-content: center;
            color: #999;
            font-size: 12px;
        }
        
        /* Newsletter */
        .newsletter {
            padding: 120px 40px;
            background: #1a1a1a;
            color: #ffffff;
            text-align: center;
        }
        
        .newsletter h2 {
            color: #ffffff;
            font-size: 3.5rem;
            margin-bottom: 24px;
        }
        
        .newsletter-subtitle {
            font-size: 1.2rem;
            color: rgba(255,255,255,0.7);
            margin-bottom: 48px;
            font-weight: 300;
        }
        
        .newsletter-form {
            max-width: 600px;
            margin: 0 auto;
            display: flex;
            gap: 16px;
        }
        
        .newsletter-form input {
            flex: 1;
            padding: 18px 24px;
            border: 1px solid rgba(255,255,255,0.2);
            background: transparent;
            color: #ffffff;
            font-size: 14px;
            letter-spacing: 0.5px;
        }
        
        .newsletter-form input::placeholder {
            color: rgba(255,255,255,0.5);
        }
        
        .newsletter-form input:focus {
            outline: none;
            border-color: #ffffff;
        }
        
        .newsletter-form button {
            padding: 18px 40px;
            background: #ffffff;
            color: #1a1a1a;
            border: none;
            font-size: 11px;
            letter-spacing: 1.5px;
            text-transform: uppercase;
            cursor: pointer;
            font-weight: 700;
            transition: opacity 0.3s;
        }
        
        .newsletter-form button:hover {
            opacity: 0.9;
        }
        
        /* Premium Membership */
        .premium {
            padding: 100px 40px;
        }
        
        .premium-content {
            max-width: 900px;
            margin: 0 auto;
            text-align: center;
        }
        
        .benefits-grid {
            display: grid;
            grid-template-columns: repeat(3, 1fr);
            gap: 48px;
            margin: 60px 0;
            text-align: left;
        }
        
        .benefit-item {
            padding: 32px;
            border: 1px solid #e5e5e5;
        }
        
        .benefit-icon {
            font-size: 2rem;
            margin-bottom: 20px;
        }
        
        .benefit-title {
            font-size: 1.2rem;
            margin-bottom: 12px;
        }
        
        .benefit-desc {
            font-size: 14px;
            color: #666;
            line-height: 1.7;
        }
        
        .price {
            font-family: 'Playfair Display', serif;
            font-size: 4rem;
            margin: 40px 0 16px;
        }
        
        .price-detail {
            font-size: 13px;
            color: #999;
            letter-spacing: 1px;
            text-transform: uppercase;
        }
        
        /* Footer */
        footer {
            padding: 80px 40px 40px;
            background: #f8f8f8;
            border-top: 1px solid #e5e5e5;
        }
        
        .footer-grid {
            display: grid;
            grid-template-columns: 2fr 1fr 1fr 1fr;
            gap: 60px;
            margin-bottom: 60px;
        }
        
        .footer-logo {
            font-family: 'Playfair Display', serif;
            font-size: 1.5rem;
            font-weight: 700;
            margin-bottom: 20px;
        }
        
        .footer-desc {
            font-size: 14px;
            color: #666;
            line-height: 1.8;
        }
        
        .footer-title {
            font-size: 13px;
            letter-spacing: 1.5px;
            text-transform: uppercase;
            margin-bottom: 24px;
            font-weight: 700;
        }
        
        .footer-links {
            list-style: none;
        }
        
        .footer-links li {
            margin-bottom: 12px;
        }
        
        .footer-links a {
            text-decoration: none;
            color: #666;
            font-size: 14px;
            transition: color 0.3s;
        }
        
        .footer-links a:hover {
            color: #1a1a1a;
        }
        
        .footer-bottom {
            padding-top: 40px;
            border-top: 1px solid #e5e5e5;
            text-align: center;
            color: #999;
            font-size: 12px;
            letter-spacing: 1px;
        }
        
        /* Responsive */
        @media (max-width: 768px) {
            h1 {
                font-size: 3rem;
            }
            
            h2 {
                font-size: 2rem;
            }
            
            .nav-links {
                display: none;
            }
            
            .featured-grid,
            .pillars-grid,
            .stories-grid,
            .benefits-grid,
            .footer-grid {
                grid-template-columns: 1fr;
            }
            
            .newsletter-form {
                flex-direction: column;
            }
        }
    </style>
</head>
<body>
    <!-- Navigation -->
    <nav>
        <div class="container">
            <div class="logo">Horse Capital Chronicle</div>
            <div class="nav-links">
                <a href="#featured">Latest</a>
                <a href="#pillars">Sections</a>
                <a href="#premium">Premium</a>
                <a href="#newsletter">Newsletter</a>
                <a href="#premium" class="btn">Subscribe</a>
            </div>
        </div>
    </nav>

    <!-- Hero -->
    <section class="hero">
        <div class="container">
            <div class="hero-content">
                <div class="hero-badge">Luxury Equestrian Lifestyle</div>
                <h1>Where Luxury Meets<br>Equestrianism</h1>
                <div class="divider"></div>
                <p class="hero-subtitle">
                    From Olympic riders to million-dollar farms, stunning photography to insider access—
                    <strong>Horse Capital Chronicle</strong> is the premier destination for those who 
                    appreciate the finest in equestrian sport and lifestyle.
                </p>
                <a href="#newsletter" class="btn">Subscribe to Newsletter</a>
            </div>
        </div>
    </section>

    <!-- Featured Content -->
    <section id="featured" class="featured">
        <div class="container">
            <div class="featured-grid">
                <div class="featured-main">
                    <div class="featured-image">FEATURED IMAGE</div>
                    <div class="featured-content">
                        <div class="category">Elite Estates</div>
                        <h2>Inside the $15 Million<br>Florida Equestrian Estate</h2>
                        <p class="excerpt">
                            Nestled on 200 pristine acres in Ocala, this architectural masterpiece combines 
                            world-class horse facilities with resort-style living. From the 40-stall barn 
                            to the infinity pool overlooking training arenas, every detail speaks to excellence.
                        </p>
                        <a href="#" class="read-more">Read Full Story →</a>
                    </div>
                </div>
                
                <div class="featured-sidebar">
                    <div class="sidebar-item">
                        <div class="sidebar-image">SIDEBAR IMAGE</div>
                        <div class="category">Rider Profile</div>
                        <h3>The Making of an Olympic Champion</h3>
                        <p style="font-size: 14px; color: #666; line-height: 1.7; margin-bottom: 16px;">
                            An intimate conversation with show jumping sensation Sarah Chen about discipline, 
                            sacrifice, and the path to gold.
                        </p>
                        <a href="#" class="read-more">Read More →</a>
                    </div>
                    
                    <div class="sidebar-item">
                        <div class="sidebar-image">SIDEBAR IMAGE</div>
                        <div class="category">Market Intelligence</div>
                        <h3>Bloodstock Investment Strategies for 2025</h3>
                        <p style="font-size: 14px; color: #666; line-height: 1.7; margin-bottom: 16px;">
                            Industry experts weigh in on emerging bloodlines, market trends, and where 
                            savvy investors are placing their bets.
                        </p>
                        <a href="#" class="read-more">Read More →</a>
                    </div>
                </div>
            </div>
        </div>
    </section>

    <!-- Content Pillars -->
    <section id="pillars" class="pillars">
        <div class="container">
            <div class="section-header">
                <h2 class="section-title">Explore Our Coverage</h2>
                <p class="section-subtitle">
                    Four pillars of exceptional content for the discerning equestrian enthusiast
                </p>
            </div>
            
            <div class="pillars-grid">
                <div class="pillar-card">
                    <div class="pillar-icon">🏇</div>
                    <h4 class="pillar-title">Horses & Sport</h4>
                    <p class="pillar-desc">
                        Elite rider profiles, major competition coverage, training techniques, 
                        and behind-the-scenes access to the world's premier events.
                    </p>
                </div>
                
                <div class="pillar-card">
                    <div class="pillar-icon">✨</div>
                    <h4 class="pillar-title">Luxury Lifestyle</h4>
                    <p class="pillar-desc">
                        Equestrian real estate, fashion and style, travel destinations, 
                        entertaining, and the art of living well with horses.
                    </p>
                </div>
                
                <div class="pillar-card">
                    <div class="pillar-icon">📊</div>
                    <h4 class="pillar-title">Business & Investing</h4>
                    <p class="pillar-desc">
                        Market trends, investment strategies, farm management, technology innovations, 
                        and thought leadership from industry titans.
                    </p>
                </div>
                
                <div class="pillar-card">
                    <div class="pillar-icon">🌿</div>
                    <h4 class="pillar-title">Health & Wellness</h4>
                    <p class="pillar-desc">
                        Horse health and nutrition, rider fitness, longevity strategies, 
                        veterinary innovations, and the mind-body connection.
                    </p>
                </div>
            </div>
        </div>
    </section>

    <!-- Latest Stories -->
    <section class="latest">
        <div class="container">
            <div class="section-header">
                <h2 class="section-title">Latest Stories</h2>
            </div>
            
            <div class="stories-grid">
                <a href="#" class="story-card">
                    <div class="story-image">STORY IMAGE</div>
                    <div class="category">Style</div>
                    <h3>The New Era of Riding Fashion</h3>
                    <p class="excerpt">
                        How today's top designers are reimagining traditional equestrian attire 
                        for the modern rider who demands both function and style.
                    </p>
                </a>
                
                <a href="#" class="story-card">
                    <div class="story-image">STORY IMAGE</div>
                    <div class="category">Technology</div>
                    <h3>Genetic Testing Transforms Breeding</h3>
                    <p class="excerpt">
                        Elite breeders are using cutting-edge DNA analysis to identify future 
                        champions before they're even born.
                    </p>
                </a>
                
                <a href="#" class="story-card">
                    <div class="story-image">STORY IMAGE</div>
                    <div class="category">Travel</div>
                    <h3>10 Must-Visit Equestrian Destinations</h3>
                    <p class="excerpt">
                        From Ireland's rolling hills to Argentina's polo fields, discover 
                        the world's most spectacular places to experience horses.
                    </p>
                </a>
            </div>
        </div>
    </section>

    <!-- Newsletter -->
    <section id="newsletter" class="newsletter">
        <div class="container">
            <h2>Never Miss a Story</h2>
            <p class="newsletter-subtitle">
                Join 150,000 subscribers receiving daily insights, exclusive content,<br>
                and behind-the-scenes access to the equestrian elite.
            </p>
            <form class="newsletter-form">
                <input type="email" placeholder="Enter your email address" required>
                <button type="submit">Subscribe</button>
            </form>
            <p style="margin-top: 24px; font-size: 12px; color: rgba(255,255,255,0.5);">
                Free • No spam • Unsubscribe anytime
            </p>
        </div>
    </section>

    <!-- Premium Membership -->
    <section id="premium" class="premium">
        <div class="container">
            <div class="premium-content">
                <div class="section-header">
                    <h2 class="section-title">Premium Membership</h2>
                    <p class="section-subtitle">
                        An elevated experience for serious enthusiasts
                    </p>
                </div>
                
                <div class="benefits-grid">
                    <div class="benefit-item">
                        <div class="benefit-icon">📖</div>
                        <h4 class="benefit-title">Ad-Free Reading</h4>
                        <p class="benefit-desc">
                            Enjoy uninterrupted access to all content across web and mobile 
                            without advertisements.
                        </p>
                    </div>
                    
                    <div class="benefit-item">
                        <div class="benefit-icon">📚</div>
                        <h4 class="benefit-title">Full Digital Archive</h4>
                        <p class="benefit-desc">
                            Unlimited access to our complete library of articles, videos, 
                            and exclusive content.
                        </p>
                    </div>
                    
                    <div class="benefit-item">
                        <div class="benefit-icon">📰</div>
                        <h4 class="benefit-title">Quarterly Print Edition</h4>
                        <p class="benefit-desc">
                            Receive our stunning 200-page coffee table magazine delivered 
                            to your door four times a year.
                        </p>
                    </div>
                    
                    <div class="benefit-item">
                        <div class="benefit-icon">🎥</div>
                        <h4 class="benefit-title">Exclusive Video Series</h4>
                        <p class="benefit-desc">
                            Premium documentaries, farm tours, and behind-the-scenes content 
                            not available anywhere else.
                        </p>
                    </div>
                    
                    <div class="benefit-item">
                        <div class="benefit-icon">🎟️</div>
                        <h4 class="benefit-title">Event Access</h4>
                        <p class="benefit-desc">
                            Early registration and special pricing for Horse Capital Summit 
                            and regional experiences.
                        </p>
                    </div>
                    
                    <div class="benefit-item">
                        <div class="benefit-icon">💎</div>
                        <h4 class="benefit-title">Platform Discounts</h4>
                        <p class="benefit-desc">
                            10% off genetic testing, nutrition supplements, analytics services, 
                            and more from our partners.
                        </p>
                    </div>
                </div>
                
                <div class="price">$199</div>
                <div class="price-detail">Per Year • Cancel Anytime</div>
                <div style="margin-top: 40px;">
                    <a href="#" class="btn" style="padding: 16px 48px; font-size: 12px;">Start Premium Membership</a>
                </div>
            </div>
        </div>
    </section>

    <!-- Footer -->
    <footer>
        <div class="container">
            <div class="footer-grid">
                <div>
                    <div class="footer-logo">Horse Capital Chronicle</div>
                    <p class="footer-desc">
                        The premier destination for luxury equestrian lifestyle, 
                        combining stunning photography, insider access, and authoritative 
                        journalism for those who appreciate excellence in all things equestrian.
                    </p>
                </div>
                
                <div>
                    <h4 class="footer-title">Sections</h4>
                    <ul class="footer-links">
                        <li><a href="#">Horses & Sport</a></li>
                        <li><a href="#">Luxury Lifestyle</a></li>
                        <li><a href="#">Business & Investing</a></li>
                        <li><a href="#">Health & Wellness</a></li>
                    </ul>
                </div>
                
                <div>
                    <h4 class="footer-title">Company</h4>
                    <ul class="footer-links">
                        <li><a href="#">About Us</a></li>
                        <li><a href="#">Advertise</a></li>
                        <li><a href="#">Partnerships</a></li>
                        <li><a href="#">Careers</a></li>
                        <li><a href="#">Contact</a></li>
                    </ul>
                </div>
                
                <div>
                    <h4 class="footer-title">Follow Us</h4>
                    <ul class="footer-links">
                        <li><a href="#">Instagram</a></li>
                        <li><a href="#">YouTube</a></li>
                        <li><a href="#">LinkedIn</a></li>
                        <li><a href="#">Facebook</a></li>
                        <li><a href="#">Pinterest</a></li>
                    </ul>
                </div>
            </div>
            
            <div class="footer-bottom">
                <p>&copy; 2024 Horse Capital Chronicle. All rights reserved.</p>
            </div>
        </div>
    </footer>

    <script>
        // Smooth scrolling
        document.querySelectorAll('a[href^="#"]').forEach(anchor => {
            anchor.addEventListener('click', function (e) {
                e.preventDefault();
                const target = document.querySelector(this.getAttribute('href'));
                if (target) {
                    target.scrollIntoView({ behavior: 'smooth', block: 'start' });
                }
            });
        });

        // Newsletter form
        document.querySelector('.newsletter-form').addEventListener('submit', function(e) {
            e.preventDefault();
            alert('Thank you for subscribing! Check your email for confirmation.');
            this.reset();
        });
    </script>
</body>
</html>
