<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>DK_FASHION | Premium Women's Footwear</title>
    <link href="https://fonts.googleapis.com/css2?family=Playfair+Display:wght@400;700&family=Inter:wght@300;400;500;600&display=swap" rel="stylesheet">
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css">
    <style>
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }

        :root {
            --primary: #C9A87C;
            --primary-dark: #A68B5C;
            --secondary: #2C2C2C;
            --accent: #F5F1EB;
            --white: #FFFFFF;
            --text: #333333;
            --text-light: #666666;
        }

        body {
            font-family: 'Inter', sans-serif;
            background-color: var(--white);
            color: var(--text);
            overflow-x: hidden;
        }

        /* Navigation */
        nav {
            position: fixed;
            top: 0;
            width: 100%;
            padding: 20px 5%;
            display: flex;
            justify-content: space-between;
            align-items: center;
            z-index: 1000;
            background: rgba(255, 255, 255, 0.95);
            backdrop-filter: blur(10px);
            transition: all 0.3s ease;
        }

        .logo {
            font-family: 'Playfair Display', serif;
            font-size: 28px;
            font-weight: 700;
            color: var(--secondary);
            letter-spacing: 2px;
            text-decoration: none;
        }

        .logo span {
            color: var(--primary);
        }

        .nav-links {
            display: flex;
            gap: 40px;
            list-style: none;
        }

        .nav-links a {
            text-decoration: none;
            color: var(--text);
            font-weight: 500;
            font-size: 14px;
            text-transform: uppercase;
            letter-spacing: 1px;
            position: relative;
            transition: color 0.3s;
        }

        .nav-links a::after {
            content: '';
            position: absolute;
            bottom: -5px;
            left: 0;
            width: 0;
            height: 2px;
            background: var(--primary);
            transition: width 0.3s;
        }

        .nav-links a:hover::after {
            width: 100%;
        }

        .nav-icons {
            display: flex;
            gap: 25px;
            align-items: center;
        }

        .nav-icons i {
            font-size: 20px;
            cursor: pointer;
            transition: transform 0.3s, color 0.3s;
        }

        .nav-icons i:hover {
            transform: scale(1.1);
            color: var(--primary);
        }

        .cart-badge {
            position: absolute;
            top: -8px;
            right: -8px;
            background: var(--primary);
            color: white;
            font-size: 10px;
            width: 18px;
            height: 18px;
            border-radius: 50%;
            display: flex;
            align-items: center;
            justify-content: center;
            font-weight: 600;
        }

        .cart-icon {
            position: relative;
        }

        /* Hero Section */
        .hero {
            margin-top: 80px;
            min-height: 90vh;
            display: grid;
            grid-template-columns: 1fr 1fr;
            align-items: center;
            padding: 0 5%;
            background: linear-gradient(135deg, var(--accent) 0%, var(--white) 100%);
            position: relative;
            overflow: hidden;
        }

        .hero::before {
            content: '';
            position: absolute;
            top: -50%;
            right: -20%;
            width: 800px;
            height: 800px;
            background: radial-gradient(circle, rgba(201, 168, 124, 0.1) 0%, transparent 70%);
            border-radius: 50%;
        }

        .hero-content {
            z-index: 1;
            animation: fadeInUp 1s ease;
        }

        .breadcrumb {
            font-size: 12px;
            color: var(--text-light);
            margin-bottom: 20px;
            text-transform: uppercase;
            letter-spacing: 2px;
        }

        .breadcrumb a {
            color: var(--primary);
            text-decoration: none;
        }

        .product-title {
            font-family: 'Playfair Display', serif;
            font-size: 48px;
            line-height: 1.2;
            margin-bottom: 20px;
            color: var(--secondary);
        }

        .product-subtitle {
            font-size: 18px;
            color: var(--text-light);
            margin-bottom: 30px;
            line-height: 1.6;
        }

        .price-tag {
            display: flex;
            align-items: baseline;
            gap: 15px;
            margin-bottom: 30px;
        }

        .current-price {
            font-size: 36px;
            font-weight: 700;
            color: var(--primary-dark);
        }

        .currency {
            font-size: 24px;
            font-weight: 600;
        }

        .size-selector {
            margin-bottom: 30px;
        }

        .size-label {
            font-weight: 600;
            margin-bottom: 15px;
            display: block;
            text-transform: uppercase;
            letter-spacing: 1px;
            font-size: 14px;
        }

        .size-options {
            display: flex;
            gap: 10px;
            flex-wrap: wrap;
        }

        .size-btn {
            width: 50px;
            height: 50px;
            border: 2px solid #ddd;
            background: white;
            cursor: pointer;
            font-weight: 600;
            transition: all 0.3s;
            border-radius: 8px;
        }

        .size-btn:hover, .size-btn.active {
            border-color: var(--primary);
            background: var(--primary);
            color: white;
            transform: translateY(-2px);
        }

        .color-selector {
            margin-bottom: 30px;
        }

        .color-options {
            display: flex;
            gap: 15px;
        }

        .color-circle {
            width: 40px;
            height: 40px;
            border-radius: 50%;
            cursor: pointer;
            border: 3px solid transparent;
            transition: all 0.3s;
            position: relative;
        }

        .color-circle.active {
            border-color: var(--secondary);
            transform: scale(1.1);
        }

        .color-beige {
            background: #D4C4B0;
        }

        .color-black {
            background: #2C2C2C;
        }

        .color-white {
            background: #F5F5F5;
            border: 1px solid #ddd;
        }

        .action-buttons {
            display: flex;
            gap: 20px;
            margin-bottom: 40px;
        }

        .btn-primary {
            flex: 1;
            padding: 18px 40px;
            background: var(--secondary);
            color: white;
            border: none;
            font-size: 16px;
            font-weight: 600;
            text-transform: uppercase;
            letter-spacing: 1px;
            cursor: pointer;
            transition: all 0.3s;
            border-radius: 4px;
            position: relative;
            overflow: hidden;
        }

        .btn-primary::before {
            content: '';
            position: absolute;
            top: 0;
            left: -100%;
            width: 100%;
            height: 100%;
            background: var(--primary);
            transition: left 0.3s;
            z-index: 0;
        }

        .btn-primary:hover::before {
            left: 0;
        }

        .btn-primary span {
            position: relative;
            z-index: 1;
        }

        .btn-secondary {
            width: 60px;
            height: 60px;
            border: 2px solid var(--secondary);
            background: transparent;
            cursor: pointer;
            border-radius: 4px;
            transition: all 0.3s;
            display: flex;
            align-items: center;
            justify-content: center;
        }

        .btn-secondary:hover {
            background: var(--secondary);
            color: white;
        }

        .features-list {
            display: grid;
            grid-template-columns: repeat(3, 1fr);
            gap: 20px;
            padding-top: 30px;
            border-top: 1px solid #eee;
        }

        .feature-item {
            display: flex;
            align-items: center;
            gap: 10px;
            font-size: 13px;
            color: var(--text-light);
        }

        .feature-item i {
            color: var(--primary);
            font-size: 18px;
        }

        /* Hero Image */
        .hero-image {
            position: relative;
            display: flex;
            justify-content: center;
            align-items: center;
            animation: fadeIn 1.2s ease;
        }

        .image-container {
            position: relative;
            width: 100%;
            max-width: 600px;
        }

        .main-image {
            width: 100%;
            height: auto;
            filter: drop-shadow(0 30px 60px rgba(0,0,0,0.15));
            transform: rotate(-5deg);
            transition: transform 0.5s ease;
        }

        .main-image:hover {
            transform: rotate(0deg) scale(1.05);
        }

        .floating-tag {
            position: absolute;
            background: white;
            padding: 15px 25px;
            border-radius: 50px;
            box-shadow: 0 10px 30px rgba(0,0,0,0.1);
            font-weight: 600;
            font-size: 14px;
            animation: float 3s ease-in-out infinite;
        }

        .tag-1 {
            top: 20%;
            left: -10%;
            animation-delay: 0s;
        }

        .tag-2 {
            bottom: 30%;
            right: -5%;
            animation-delay: 1.5s;
        }

        .tag-3 {
            top: 60%;
            left: -5%;
            animation-delay: 0.75s;
        }

        /* Product Details Section */
        .details-section {
            padding: 100px 5%;
            background: var(--white);
        }

        .section-header {
            text-align: center;
            margin-bottom: 60px;
        }

        .section-title {
            font-family: 'Playfair Display', serif;
            font-size: 42px;
            margin-bottom: 15px;
            color: var(--secondary);
        }

        .section-subtitle {
            color: var(--text-light);
            font-size: 16px;
        }

        .details-grid {
            display: grid;
            grid-template-columns: repeat(4, 1fr);
            gap: 30px;
            max-width: 1200px;
            margin: 0 auto;
        }

        .detail-card {
            background: var(--accent);
            padding: 40px 30px;
            border-radius: 20px;
            text-align: center;
            transition: transform 0.3s, box-shadow 0.3s;
            cursor: pointer;
        }

        .detail-card:hover {
            transform: translateY(-10px);
            box-shadow: 0 20px 40px rgba(0,0,0,0.1);
        }

        .detail-icon {
            width: 80px;
            height: 80px;
            background: white;
            border-radius: 50%;
            display: flex;
            align-items: center;
            justify-content: center;
            margin: 0 auto 20px;
            font-size: 32px;
            color: var(--primary);
            box-shadow: 0 10px 30px rgba(201, 168, 124, 0.2);
        }

        .detail-title {
            font-weight: 700;
            margin-bottom: 10px;
            font-size: 18px;
        }

        .detail-desc {
            font-size: 14px;
            color: var(--text-light);
            line-height: 1.6;
        }

        /* Gallery Section */
        .gallery-section {
            padding: 100px 5%;
            background: linear-gradient(to bottom, var(--accent), var(--white));
        }

        .gallery-grid {
            display: grid;
            grid-template-columns: repeat(3, 1fr);
            gap: 20px;
            max-width: 1400px;
            margin: 0 auto;
        }

        .gallery-item {
            position: relative;
            overflow: hidden;
            border-radius: 15px;
            aspect-ratio: 1;
            cursor: pointer;
        }

        .gallery-item img {
            width: 100%;
            height: 100%;
            object-fit: cover;
            transition: transform 0.5s;
        }

        .gallery-item:hover img {
            transform: scale(1.1);
        }

        .gallery-overlay {
            position: absolute;
            bottom: 0;
            left: 0;
            right: 0;
            background: linear-gradient(to top, rgba(0,0,0,0.7), transparent);
            padding: 30px;
            color: white;
            transform: translateY(100%);
            transition: transform 0.3s;
        }

        .gallery-item:hover .gallery-overlay {
            transform: translateY(0);
        }

        /* Reviews Section */
        .reviews-section {
            padding: 100px 5%;
            background: var(--white);
        }

        .reviews-grid {
            display: grid;
            grid-template-columns: repeat(3, 1fr);
            gap: 30px;
            max-width: 1200px;
            margin: 0 auto;
        }

        .review-card {
            background: var(--accent);
            padding: 40px;
            border-radius: 20px;
            position: relative;
        }

        .review-stars {
            color: var(--primary);
            margin-bottom: 20px;
            font-size: 18px;
        }

        .review-text {
            font-size: 16px;
            line-height: 1.8;
            margin-bottom: 25px;
            color: var(--text);
            font-style: italic;
        }

        .reviewer-info {
            display: flex;
            align-items: center;
            gap: 15px;
        }

        .reviewer-avatar {
            width: 50px;
            height: 50px;
            border-radius: 50%;
            background: var(--primary);
            display: flex;
            align-items: center;
            justify-content: center;
            color: white;
            font-weight: 700;
            font-size: 20px;
        }

        .reviewer-name {
            font-weight: 600;
        }

        .reviewer-verified {
            font-size: 12px;
            color: var(--primary);
        }

        /* Newsletter */
        .newsletter {
            padding: 100px 5%;
            background: var(--secondary);
            color: white;
            text-align: center;
        }

        .newsletter-title {
            font-family: 'Playfair Display', serif;
            font-size: 42px;
            margin-bottom: 20px;
        }

        .newsletter-form {
            max-width: 500px;
            margin: 40px auto 0;
            display: flex;
            gap: 15px;
        }

        .newsletter-input {
            flex: 1;
            padding: 18px 25px;
            border: none;
            border-radius: 4px;
            font-size: 16px;
            outline: none;
        }

        .newsletter-btn {
            padding: 18px 40px;
            background: var(--primary);
            color: white;
            border: none;
            border-radius: 4px;
            font-weight: 600;
            cursor: pointer;
            transition: background 0.3s;
            text-transform: uppercase;
            letter-spacing: 1px;
        }

        .newsletter-btn:hover {
            background: var(--primary-dark);
        }

        /* Footer */
        footer {
            background: #1a1a1a;
            color: white;
            padding: 60px 5% 30px;
        }

        .footer-content {
            display: grid;
            grid-template-columns: 2fr 1fr 1fr 1fr;
            gap: 60px;
            max-width: 1200px;
            margin: 0 auto 40px;
        }

        .footer-brand .logo {
            color: white;
            margin-bottom: 20px;
            display: inline-block;
        }

        .footer-desc {
            color: #999;
            line-height: 1.8;
            margin-bottom: 25px;
        }

        .social-links {
            display: flex;
            gap: 20px;
        }

        .social-links a {
            width: 40px;
            height: 40px;
            border: 1px solid #444;
            border-radius: 50%;
            display: flex;
            align-items: center;
            justify-content: center;
            color: white;
            text-decoration: none;
            transition: all 0.3s;
        }

        .social-links a:hover {
            background: var(--primary);
            border-color: var(--primary);
            transform: translateY(-3px);
        }

        .footer-title {
            font-weight: 700;
            margin-bottom: 25px;
            text-transform: uppercase;
            letter-spacing: 1px;
            font-size: 14px;
        }

        .footer-links {
            list-style: none;
        }

        .footer-links li {
            margin-bottom: 12px;
        }

        .footer-links a {
            color: #999;
            text-decoration: none;
            transition: color 0.3s;
            font-size: 14px;
        }

        .footer-links a:hover {
            color: var(--primary);
        }

        .footer-bottom {
            border-top: 1px solid #333;
            padding-top: 30px;
            text-align: center;
            color: #666;
            font-size: 14px;
        }

        /* Animations */
        @keyframes fadeInUp {
            from {
                opacity: 0;
                transform: translateY(30px);
            }
            to {
                opacity: 1;
                transform: translateY(0);
            }
        }

        @keyframes fadeIn {
            from { opacity: 0; }
            to { opacity: 1; }
        }

        @keyframes float {
            0%, 100% { transform: translateY(0); }
            50% { transform: translateY(-10px); }
        }

        /* Mobile Responsive */
        @media (max-width: 968px) {
            .hero {
                grid-template-columns: 1fr;
                text-align: center;
                padding-top: 120px;
            }

            .hero-content {
                order: 2;
            }

            .hero-image {
                order: 1;
                margin-bottom: 40px;
            }

            .product-title {
                font-size: 36px;
            }

            .details-grid, .reviews-grid {
                grid-template-columns: repeat(2, 1fr);
            }

            .gallery-grid {
                grid-template-columns: repeat(2, 1fr);
            }

            .footer-content {
                grid-template-columns: repeat(2, 1fr);
            }
        }

        @media (max-width: 600px) {
            .nav-links {
                display: none;
            }

            .details-grid, .reviews-grid, .gallery-grid {
                grid-template-columns: 1fr;
            }

            .footer-content {
                grid-template-columns: 1fr;
                gap: 40px;
            }

            .action-buttons {
                flex-direction: column;
            }

            .features-list {
                grid-template-columns: 1fr;
                text-align: left;
            }
        }

        /* Scroll animations */
        .scroll-reveal {
            opacity: 0;
            transform: translateY(30px);
            transition: all 0.8s ease;
        }

        .scroll-reveal.active {
            opacity: 1;
            transform: translateY(0);
        }
    </style>
</head>
<body>

    <!-- Navigation -->
    <nav id="navbar">
        <a href="#" class="logo">DK<span>_</span>FASHION</a>
        <ul class="nav-links">
            <li><a href="#home">Home</a></li>
            <li><a href="#new-arrivals">New Arrivals</a></li>
            <li><a href="#women">Women</a></li>
            <li><a href="#men">Men</a></li>
            <li><a href="#sale">Sale</a></li>
        </ul>
        <div class="nav-icons">
            <i class="fas fa-search"></i>
            <i class="fas fa-user"></i>
            <div class="cart-icon">
                <i class="fas fa-shopping-bag"></i>
                <span class="cart-badge">2</span>
            </div>
        </div>
    </nav>

    <!-- Hero Section -->
    <section class="hero" id="home">
        <div class="hero-content">
            <div class="breadcrumb">
                <a href="#">Home</a> / <a href="#">Women</a> / <a href="#">Sneakers</a> / <span>Chain Detail Mesh</span>
            </div>
            
            <h1 class="product-title">New Mesh Solid Color Round Toe Low-Top Pumps</h1>
            <p class="product-subtitle">Women's Chain Large Size Sports Style Casual Sneakers. Experience ultimate comfort with breathable mesh fabric and elegant gold chain detailing.</p>
            
            <div class="price-tag">
                <span class="current-price"><span class="currency">PKR</span> 15,000</span>
            </div>

            <div class="color-selector">
                <span class="size-label">Select Color</span>
                <div class="color-options">
                    <div class="color-circle color-beige active" onclick="selectColor(this)" title="Beige"></div>
                    <div class="color-circle color-black" onclick="selectColor(this)" title="Black"></div>
                    <div class="color-circle color-white" onclick="selectColor(this)" title="White"></div>
                </div>
            </div>

            <div class="size-selector">
                <span class="size-label">Select Size (EU)</span>
                <div class="size-options">
                    <button class="size-btn">36</button>
                    <button class="size-btn">37</button>
                    <button class="size-btn active">38</button>
                    <button class="size-btn">39</button>
                    <button class="size-btn">40</button>
                    <button class="size-btn">41</button>
                    <button class="size-btn">42</button>
                </div>
            </div>

            <div class="action-buttons">
                <button class="btn-primary" onclick="addToCart()">
                    <span><i class="fas fa-shopping-bag"></i> Add to Cart</span>
                </button>
                <button class="btn-secondary" onclick="toggleWishlist(this)">
                    <i class="far fa-heart"></i>
                </button>
            </div>

            <div class="features-list">
                <div class="feature-item">
                    <i class="fas fa-truck"></i>
                    <span>Free Delivery</span>
                </div>
                <div class="feature-item">
                    <i class="fas fa-undo"></i>
                    <span>30-Day Returns</span>
                </div>
                <div class="feature-item">
                    <i class="fas fa-shield-alt"></i>
                    <span>Secure Payment</span>
                </div>
            </div>
        </div>

        <div class="hero-image">
            <div class="image-container">
                <img src="https://u-mercari-images.mercdn.net/thumb/photos/m36224067515_1.jpg?width=2560&quality=75&_=1762965248" alt="Beige Mesh Sneakers with Chain Detail" class="main-image">
                
                <div class="floating-tag tag-1">
                    <i class="fas fa-wind"></i> Breathable Mesh
                </div>
                <div class="floating-tag tag-2">
                    <i class="fas fa-gem"></i> Gold Chain Accent
                </div>
                <div class="floating-tag tag-3">
                    <i class="fas fa-feather"></i> Ultra Lightweight
                </div>
            </div>
        </div>
    </section>

    <!-- Product Details -->
    <section class="details-section">
        <div class="section-header scroll-reveal">
            <h2 class="section-title">Premium Features</h2>
            <p class="section-subtitle">Designed for the modern woman who values both style and comfort</p>
        </div>
        
        <div class="details-grid">
            <div class="detail-card scroll-reveal">
                <div class="detail-icon">
                    <i class="fas fa-wind"></i>
                </div>
                <h3 class="detail-title">Breathable Mesh</h3>
                <p class="detail-desc">Advanced knit technology allows maximum airflow to keep your feet cool and dry all day long.</p>
            </div>
            
            <div class="detail-card scroll-reveal">
                <div class="detail-icon">
                    <i class="fas fa-link"></i>
                </div>
                <h3 class="detail-title">Chain Detail</h3>
                <p class="detail-desc">Elegant gold-tone chain accent adds a touch of luxury to your casual sporty look.</p>
            </div>
            
            <div class="detail-card scroll-reveal">
                <div class="detail-icon">
                    <i class="fas fa-shoe-prints"></i>
                </div>
                <h3 class="detail-title">Anti-Slip Sole</h3>
                <p class="detail-desc">Durable rubber outsole with advanced grip pattern ensures stability on any surface.</p>
            </div>
            
            <div class="detail-card scroll-reveal">
                <div class="detail-icon">
                    <i class="fas fa-expand-arrows-alt"></i>
                </div>
                <h3 class="detail-title">Large Sizes</h3>
                <p class="detail-desc">Available in extended sizes 36-42, designed to provide perfect fit for every foot.</p>
            </div>
        </div>
    </section>

    <!-- Gallery Section -->
    <section class="gallery-section">
        <div class="section-header scroll-reveal">
            <h2 class="section-title">Style Gallery</h2>
            <p class="section-subtitle">See how our customers style their DK_FASHION sneakers</p>
        </div>
        
        <div class="gallery-grid">
            <div class="gallery-item scroll-reveal">
                <img src="https://i.ebayimg.com/images/g/94EAAOSw-o9kFCNl/s-l400.jpg" alt="Side view of sneakers">
                <div class="gallery-overlay">
                    <h4>Casual Chic</h4>
                    <p>Perfect with jeans</p>
                </div>
            </div>
            
            <div class="gallery-item scroll-reveal">
                <img src="https://img.ltwebstatic.com/images3_pi/2023/08/17/cf/16922866066695403728b068f44957154ac13c8403_thumbnail_720x.jpg" alt="Styled with outfit">
                <div class="gallery-overlay">
                    <h4>Sporty Elegance</h4>
                    <p>Street style ready</p>
                </div>
            </div>
            
            <div class="gallery-item scroll-reveal">
                <img src="https://u-mercari-images.mercdn.net/thumb/photos/m36224067515_1.jpg?width=2560&quality=75&_=1762965248" alt="Detail shot">
                <div class="gallery-overlay">
                    <h4>Detail Focus</h4>
                    <p>Chain accent close-up</p>
                </div>
            </div>
        </div>
    </section>

    <!-- Reviews Section -->
    <section class="reviews-section">
        <div class="section-header scroll-reveal">
            <h2 class="section-title">Customer Love</h2>
            <p class="section-subtitle">See what our customers are saying about these sneakers</p>
        </div>
        
        <div class="reviews-grid">
            <div class="review-card scroll-reveal">
                <div class="review-stars">
                    <i class="fas fa-star"></i>
                    <i class="fas fa-star"></i>
                    <i class="fas fa-star"></i>
                    <i class="fas fa-star"></i>
                    <i class="fas fa-star"></i>
                </div>
                <p class="review-text">"Absolutely love these sneakers! The mesh is so breathable and the chain detail adds such a classy touch. Perfect for both gym and casual outings."</p>
                <div class="reviewer-info">
                    <div class="reviewer-avatar">SK</div>
                    <div>
                        <div class="reviewer-name">Sarah K.</div>
                        <div class="reviewer-verified"><i class="fas fa-check-circle"></i> Verified Buyer</div>
                    </div>
                </div>
            </div>
            
            <div class="review-card scroll-reveal">
                <div class="review-stars">
                    <i class="fas fa-star"></i>
                    <i class="fas fa-star"></i>
                    <i class="fas fa-star"></i>
                    <i class="fas fa-star"></i>
                    <i class="fas fa-star"></i>
                </div>
                <p class="review-text">"Finally found stylish sneakers in size 42! The fit is perfect and they're incredibly comfortable for all-day wear. Highly recommend!"</p>
                <div class="reviewer-info">
                    <div class="reviewer-avatar">AM</div>
                    <div>
                        <div class="reviewer-name">Amina M.</div>
                        <div class="reviewer-verified"><i class="fas fa-check-circle"></i> Verified Buyer</div>
                    </div>
                </div>
            </div>
            
            <div class="review-card scroll-reveal">
                <div class="review-stars">
                    <i class="fas fa-star"></i>
                    <i class="fas fa-star"></i>
                    <i class="fas fa-star"></i>
                    <i class="fas fa-star"></i>
                    <i class="fas fa-star-half-alt"></i>
                </div>
                <p class="review-text">"Great quality for the price. The beige color goes with everything in my wardrobe. Fast delivery to Lahore too!"</p>
                <div class="reviewer-info">
                    <div class="reviewer-avatar">FR</div>
                    <div>
                        <div class="reviewer-name">Fatima R.</div>
                        <div class="reviewer-verified"><i class="fas fa-check-circle"></i> Verified Buyer</div>
                    </div>
                </div>
            </div>
        </div>
    </section>

    <!-- Newsletter -->
    <section class="newsletter">
        <h2 class="newsletter-title">Join the DK_FASHION Family</h2>
        <p>Subscribe for exclusive offers, new arrivals, and style tips</p>
        <form class="newsletter-form" onsubmit="handleSubscribe(event)">
            <input type="email" class="newsletter-input" placeholder="Enter your email address" required>
            <button type="submit" class="newsletter-btn">Subscribe</button>
        </form>
    </section>

    <!-- Footer -->
    <footer>
        <div class="footer-content">
            <div class="footer-brand">
                <a href="#" class="logo">DK<span>_</span>FASHION</a>
                <p class="footer-desc">Premium footwear for the modern woman. We blend comfort with contemporary style to bring you shoes that make every step confident.</p>
                <div class="social-links">
                    <a href="#"><i class="fab fa-facebook-f"></i></a>
                    <a href="#"><i class="fab fa-instagram"></i></a>
                    <a href="#"><i class="fab fa-twitter"></i></a>
                    <a href="#"><i class="fab fa-pinterest"></i></a>
                </div>
            </div>
            
            <div>
                <h4 class="footer-title">Shop</h4>
                <ul class="footer-links">
                    <li><a href="#">New Arrivals</a></li>
                    <li><a href="#">Best Sellers</a></li>
                    <li><a href="#">Women's Shoes</a></li>
                    <li><a href="#">Sale</a></li>
                </ul>
            </div>
            
            <div>
                <h4 class="footer-title">Help</h4>
                <ul class="footer-links">
                    <li><a href="#">Track Order</a></li>
                    <li><a href="#">Returns</a></li>
                    <li><a href="#">Shipping Info</a></li>
                    <li><a href="#">Size Guide</a></li>
                </ul>
            </div>
            
            <div>
                <h4 class="footer-title">Contact</h4>
                <ul class="footer-links">
                    <li><a href="#">supportdanishgamingyt317@gmail.com</a></li>
                    <li><a href="#">Lahore, Pakistan</a></li>
                </ul>
            </div>
        </div>
        
        <div class="footer-bottom">
            <p>&copy; 2026 DK_FASHION. All rights reserved. | Designed with <i class="fas fa-heart" style="color: var(--primary);"></i> in Pakistan</p>
        </div>
    </footer>

    <script>
        // Navbar scroll effect
        window.addEventListener('scroll', function() {
            const navbar = document.getElementById('navbar');
            if (window.scrollY > 50) {
                navbar.style.boxShadow = '0 2px 20px rgba(0,0,0,0.1)';
            } else {
                navbar.style.boxShadow = 'none';
            }
        });

        // Size selection
        document.querySelectorAll('.size-btn').forEach(btn => {
            btn.addEventListener('click', function() {
                document.querySelectorAll('.size-btn').forEach(b => b.classList.remove('active'));
                this.classList.add('active');
            });
        });

        // Color selection
        function selectColor(element) {
            document.querySelectorAll('.color-circle').forEach(c => c.classList.remove('active'));
            element.classList.add('active');
        }

        // Add to cart animation
        function addToCart() {
            const btn = document.querySelector('.btn-primary');
            const originalContent = btn.innerHTML;
            
            btn.innerHTML = '<span><i class="fas fa-check"></i> Added!</span>';
            btn.style.background = '#C9A87C';
            
            setTimeout(() => {
                btn.innerHTML = originalContent;
                btn.style.background = '';
            }, 2000);
            
            // Update cart badge
            const badge = document.querySelector('.cart-badge');
            badge.textContent = parseInt(badge.textContent) + 1;
            badge.style.animation = 'pulse 0.5s';
        }

        // Wishlist toggle
        function toggleWishlist(btn) {
            const icon = btn.querySelector('i');
            if (icon.classList.contains('far')) {
                icon.classList.remove('far');
                icon.classList.add('fas');
                icon.style.color = '#e74c3c';
                btn.style.borderColor = '#e74c3c';
            } else {
                icon.classList.remove('fas');
                icon.classList.add('far');
                icon.style.color = '';
                btn.style.borderColor = '';
            }
        }

        // Newsletter subscription
        function handleSubscribe(e) {
            e.preventDefault();
            const btn = e.target.querySelector('button');
            const input = e.target.querySelector('input');
            
            btn.textContent = 'Subscribed!';
            btn.style.background = '#27ae60';
            input.value = '';
            
            setTimeout(() => {
                btn.textContent = 'Subscribe';
                btn.style.background = '';
            }, 3000);
        }

        // Scroll reveal animation
        const observerOptions = {
            threshold: 0.1,
            rootMargin: '0px 0px -50px 0px'
        };

        const observer = new IntersectionObserver(function(entries) {
            entries.forEach(entry => {
                if (entry.isIntersecting) {
                    entry.target.classList.add('active');
                }
            });
        }, observerOptions);

        document.querySelectorAll('.scroll-reveal').forEach(el => {
            observer.observe(el);
        });

        // Smooth scroll for navigation
        document.querySelectorAll('a[href^="#"]').forEach(anchor => {
            anchor.addEventListener('click', function(e) {
                e.preventDefault();
                const target = document.querySelector(this.getAttribute('href'));
                if (target) {
                    target.scrollIntoView({
                        behavior: 'smooth',
                        block: 'start'
                    });
                }
            });
        });

        // Add pulse animation to cart badge
        const style = document.createElement('style');
        style.textContent = `
            @keyframes pulse {
                0% { transform: scale(1); }
                50% { transform: scale(1.3); }
                100% { transform: scale(1); }
            }
        `;
        document.head.appendChild(style);
    </script>
</body>
</html>
