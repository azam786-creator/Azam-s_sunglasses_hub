# Azam-s_sunglasses_hub
Explore and purchase your favorite item

1. HTML structure for the main pages
2. CSS styling for a modern, e-commerce look
3. JavaScript for functionality (cart, product filtering, etc.)
4. A clean, professional design suitable for fashion products

Let me create a complete, functional e-commerce website template with:
- Homepage with hero section and featured products
- Product pages for sunglasses and watches
- Shopping cart functionality
- Responsive design
- Modern UI/UX

I'll structure this as a single-page application style with multiple sections that can be navigated to, making it easier to demonstrate all the functionality in one response.

Let me write comprehensive HTML, CSS, and JavaScript code.

</think># Sunglasses & Watches E-Commerce Website

I'll create a complete, modern e-commerce website for selling sunglasses and watches. This includes a responsive design, product catalog, shopping cart functionality, and a professional fashion aesthetic.

```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>LuxeVision - Premium Sunglasses & Watches</title>
    <link rel="stylesheet" href="styles.css">
    <link href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.0.0/css/all.min.css" rel="stylesheet">
    <link href="https://fonts.googleapis.com/css2?family=Playfair+Display:wght@400;600;700&family=Poppins:wght@300;400;500;600&display=swap" rel="stylesheet">
</head>
<body>
    <!-- Navigation -->
    <nav class="navbar">
        <div class="nav-container">
            <a href="#" class="logo">Luxe<span>Vision</span></a>
            <ul class="nav-links">
                <li><a href="#home" class="active">Home</a></li>
                <li><a href="#sunglasses">Sunglasses</a></li>
                <li><a href="#watches">Watches</a></li>
                <li><a href="#about">About</a></li>
                <li><a href="#contact">Contact</a></li>
            </ul>
            <div class="nav-icons">
                <button class="search-btn"><i class="fas fa-search"></i></button>
                <button class="cart-btn" id="cartBtn">
                    <i class="fas fa-shopping-bag"></i>
                    <span class="cart-count" id="cartCount">0</span>
                </button>
            </div>
            <button class="mobile-menu-btn"><i class="fas fa-bars"></i></button>
        </div>
    </nav>

    <!-- Hero Section -->
    <section id="home" class="hero">
        <div class="hero-content">
            <span class="hero-tag">New Collection 2024</span>
            <h1>Timeless Elegance,<br>Modern Style</h1>
            <p>Discover our curated collection of premium sunglasses and luxury watches designed for those who appreciate sophistication.</p>
            <div class="hero-buttons">
                <a href="#sunglasses" class="btn btn-primary">Shop Sunglasses</a>
                <a href="#watches" class="btn btn-secondary">Shop Watches</a>
            </div>
        </div>
        <div class="hero-image">
            <img src="https://images.unsplash.com/photo-1572635196237-14b3f281503f?w=600" alt="Premium Sunglasses">
        </div>
    </section>

    <!-- Features Section -->
    <section class="features">
        <div class="feature-card">
            <i class="fas fa-shipping-fast"></i>
            <h3>Free Shipping</h3>
            <p>On orders over $150</p>
        </div>
        <div class="feature-card">
            <i class="fas fa-undo"></i>
            <h3>30-Day Returns</h3>
            <p>Easy returns policy</p>
        </div>
        <div class="feature-card">
            <i class="fas fa-shield-alt"></i>
            <h3>2-Year Warranty</h3>
            <p>Full coverage</p>
        </div>
        <div class="feature-card">
            <i class="fas fa-headset"></i>
            <h3>24/7 Support</h3>
            <p>Dedicated service</p>
        </div>
    </section>

    <!-- Sunglasses Section -->
    <section id="sunglasses" class="products-section">
        <div class="section-header">
            <span class="section-tag">Premium Collection</span>
            <h2>Sunglasses</h2>
            <p>Protect your eyes with style</p>
        </div>
        <div class="filter-tabs">
            <button class="filter-btn active" data-category="all">All</button>
            <button class="filter-btn" data-category="aviator">Aviator</button>
            <button class="filter-btn" data-category="wayfarer">Wayfarer</button>
            <button class="filter-btn" data-category="round">Round</button>
            <button class="filter-btn" data-category="cat-eye">Cat Eye</button>
        </div>
        <div class="products-grid" id="sunglassesGrid">
            <!-- Products will be loaded dynamically -->
        </div>
    </section>

    <!-- Watches Section -->
    <section id="watches" class="products-section">
        <div class="section-header">
            <span class="section-tag">Luxury Timepieces</span>
            <h2>Watches</h2>
            <p>Precision meets elegance</p>
        </div>
        <div class="filter-tabs">
            <button class="filter-btn active" data-category="all">All</button>
            <button class="filter-btn" data-category="automatic">Automatic</button>
            <button class="filter-btn" data-category="quartz">Quartz</button>
            <button class="filter-btn" data-category="chronograph">Chronograph</button>
            <button class="filter-btn" data-category="smart">Smart</button>
        </div>
        <div class="products-grid" id="watchesGrid">
            <!-- Products will be loaded dynamically -->
        </div>
    </section>

    <!-- Featured Products -->
    <section class="featured-section">
        <div class="section-header">
            <span class="section-tag">Handpicked For You</span>
            <h2>Featured Products</h2>
        </div>
        <div class="featured-grid" id="featuredGrid">
            <!-- Featured products will be loaded dynamically -->
        </div>
    </section>

    <!-- About Section -->
    <section id="about" class="about-section">
        <div class="about-content">
            <span class="section-tag">Our Story</span>
            <h2>Crafting Excellence Since 2010</h2>
            <p>At LuxeVision, we believe that accessories are more than just functional items—they're expressions of personality and style. Our curated collection brings together the finest craftsmanship from around the world.</p>
            <p>Each piece in our collection is carefully selected to ensure the highest quality materials, impeccable design, and lasting durability. Whether you're seeking the perfect sunglasses for summer adventures or a timeless watch for special occasions, we've got you covered.</p>
            <div class="about-stats">
                <div class="stat">
                    <span class="stat-number">50K+</span>
                    <span class="stat-label">Happy Customers</span>
                </div>
                <div class="stat">
                    <span class="stat-number">500+</span>
                    <span class="stat-label">Products</span>
                </div>
                <div class="stat">
                    <span class="stat-number">50+</span>
                    <span class="stat-label">Countries</span>
                </div>
            </div>
        </div>
        <div class="about-image">
            <img src="https://images.unsplash.com/photo-1523170335258-f5ed11844a49?w=600" alt="Watch craftsmanship">
        </div>
    </section>

    <!-- Newsletter Section -->
    <section class="newsletter-section">
        <div class="newsletter-content">
            <h2>Stay in Style</h2>
            <p>Subscribe to our newsletter for exclusive offers, new arrivals, and style tips.</p>
            <form class="newsletter-form" id="newsletterForm">
                <input type="email" placeholder="Enter your email address" required>
                <button type="submit" class="btn btn-primary">Subscribe</button>
            </form>
        </div>
    </section>

    <!-- Contact Section -->
    <section id="contact" class="contact-section">
        <div class="section-header">
            <span class="section-tag">Get In Touch</span>
            <h2>Contact Us</h2>
        </div>
        <div class="contact-container">
            <div class="contact-info">
                <div class="contact-item">
                    <i class="fas fa-map-marker-alt"></i>
                    <div>
                        <h4>Visit Us</h4>
                        <p>123 Fashion Avenue, New York, NY 10001</p>
                    </div>
                </div>
                <div class="contact-item">
                    <i class="fas fa-envelope"></i>
                    <div>
                        <h4>Email Us</h4>
                        <p>hello@luxevision.com</p>
                    </div>
                </div>
                <div class="contact-item">
                    <i class="fas fa-phone"></i>
                    <div>
                        <h4>Call Us</h4>
                        <p>+1 (555) 123-4567</p>
                    </div>
                </div>
                <div class="social-links">
                    <a href="#"><i class="fab fa-facebook-f"></i></a>
                    <a href="#"><i class="fab fa-instagram"></i></a>
                    <a href="#"><i class="fab fa-twitter"></i></a>
                    <a href="#"><i class="fab fa-pinterest"></i></a>
                </div>
            </div>
            <form class="contact-form" id="contactForm">
                <div class="form-group">
                    <input type="text" placeholder="Your Name" required>
                </div>
                <div class="form-group">
                    <input type="email" placeholder="Your Email" required>
                </div>
                <div class="form-group">
                    <textarea placeholder="Your Message" rows="5" required></textarea>
                </div>
                <button type="submit" class="btn btn-primary">Send Message</button>
            </form>
        </div>
    </section>

    <!-- Footer -->
    <footer class="footer">
        <div class="footer-content">
            <div class="footer-brand">
                <a href="#" class="logo">Luxe<span>Vision</span></a>
                <p>Your destination for premium sunglasses and luxury watches. Quality, style, and sophistication in every piece.</p>
            </div>
            <div class="footer-links">
                <h4>Quick Links</h4>
                <ul>
                    <li><a href="#home">Home</a></li>
                    <li><a href="#sunglasses">Sunglasses</a></li>
                    <li><a href="#watches">Watches</a></li>
                    <li><a href="#about">About Us</a></li>
                </ul>
            </div>
            <div class="footer-links">
                <h4>Customer Service</h4>
                <ul>
                    <li><a href="#">Shipping Info</a></li>
                    <li><a href="#">Returns & Exchanges</a></li>
                    <li><a href="#">Size Guide</a></li>
                    <li><a href="#">FAQ</a></li>
                </ul>
            </div>
            <div class="footer-links">
                <h4>Legal</h4>
                <ul>
                    <li><a href="#">Privacy Policy</a></li>
                    <li><a href="#">Terms of Service</a></li>
                    <li><a href="#">Cookie Policy</a></li>
                </ul>
            </div>
        </div>
        <div class="footer-bottom">
            <p>&copy; 2024 LuxeVision. All rights reserved.</p>
            <div class="payment-methods">
                <i class="fab fa-cc-visa"></i>
                <i class="fab fa-cc-mastercard"></i>
                <i class="fab fa-cc-amex"></i>
                <i class="fab fa-cc-paypal"></i>
            </div>
        </div>
    </footer>

    <!-- Shopping Cart Sidebar -->
    <div class="cart-overlay" id="cartOverlay"></div>
    <div class="cart-sidebar" id="cartSidebar">
        <div class="cart-header">
            <h3>Shopping Cart</h3>
            <button class="close-cart" id="closeCart"><i class="fas fa-times"></i></button>
        </div>
        <div class="cart-items" id="cartItems">
            <!-- Cart items will be loaded dynamically -->
        </div>
        <div class="cart-footer">
            <div class="cart-total">
                <span>Total:</span>
                <span id="cartTotal">$0.00</span>
            </div>
            <button class="btn btn-primary checkout-btn">Proceed to Checkout</button>
        </div>
    </div>

    <!-- Product Quick View Modal -->
    <div class="modal" id="productModal">
        <div class="modal-content">
            <button class="close-modal" id="closeModal"><i class="fas fa-times"></i></button>
            <div class="modal-body" id="modalBody">
                <!-- Product details will be loaded dynamically -->
            </div>
        </div>
    </div>

    <script src="script.js"></script>
</body>
</html>
```

```css
/* CSS Styles */
:root {
    --primary-color: #1a1a2e;
    --secondary-color: #16213e;
    --accent-color: #c9a227;
    --text-color: #333;
    --text-light: #666;
    --bg-light: #f8f9fa;
    --white: #ffffff;
    --shadow: 0 10px 40px rgba(0, 0, 0, 0.1);
    --transition: all 0.3s ease;
}

* {
    margin: 0;
    padding: 0;
    box-sizing: border-box;
}

html {
    scroll-behavior: smooth;
}

body {
    font-family: 'Poppins', sans-serif;
    color: var(--text-color);
    line-height: 1.6;
    overflow-x: hidden;
}

h1, h2, h3, h4 {
    font-family: 'Playfair Display', serif;
    font-weight: 600;
}

a {
    text-decoration: none;
    color: inherit;
}

ul {
    list-style: none;
}

img {
    max-width: 100%;
    height: auto;
}

.container {
    max-width: 1200px;
    margin: 0 auto;
    padding: 0 20px;
}

/* Buttons */
.btn {
    display: inline-block;
    padding: 14px 32px;
    border: none;
    border-radius: 50px;
    font-size: 14px;
    font-weight: 500;
    cursor: pointer;
    transition: var(--transition);
    text-transform: uppercase;
    letter-spacing: 1px;
}

.btn-primary {
    background: var(--primary-color);
    color: var(--white);
}

.btn-primary:hover {
    background: var(--accent-color);
    transform: translateY(-2px);
}

.btn-secondary {
    background: transparent;
    color: var(--primary-color);
    border: 2px solid var(--primary-color);
}

.btn-secondary:hover {
    background: var(--primary-color);
    color: var(--white);
}

/* Navigation */
.navbar {
    position: fixed;
    top: 0;
    left: 0;
    right: 0;
    background: var(--white);
    z-index: 1000;
    box-shadow: 0 2px 20px rgba(0, 0, 0, 0.05);
}

.nav-container {
    max-width: 1200px;
    margin: 0 auto;
    padding: 15px 20px;
    display: flex;
    align-items: center;
    justify-content: space-between;
}

.logo {
    font-family: 'Playfair Display', serif;
    font-size: 28px;
    font-weight: 700;
    color: var(--primary-color);
}

.logo span {
    color: var(--accent-color);
}

.nav-links {
    display: flex;
    gap: 40px;
}

.nav-links a {
    font-size: 14px;
    font-weight: 500;
    color: var(--text-color);
    transition: var(--transition);
    position: relative;
}

.nav-links a::after {
    content: '';
    position: absolute;
    bottom: -5px;
    left: 0;
    width: 0;
    height: 2px;
    background: var(--accent-color);
    transition: var(--transition);
}

.nav-links a:hover::after,
.nav-links a.active::after {
    width: 100%;
}

.nav-icons {
    display: flex;
    gap: 20px;
    align-items: center;
}

.nav-icons button {
    background: none;
    border: none;
    font-size: 18px;
    cursor: pointer;
    color: var(--text-color);
    transition: var(--transition);
    position: relative;
}

.nav-icons button:hover {
    color: var(--accent-color);
}

.cart-count {
    position: absolute;
    top: -8px;
    right: -8px;
    background: var(--accent-color);
    color: var(--white);
    font-size: 10px;
    width: 18px;
    height: 18px;
    border-radius: 50%;
    display: flex;
    align-items: center;
    justify-content: center;
}

.mobile-menu-btn {
    display: none;
}

/* Hero Section */
.hero {
    min-height: 100vh;
    display: flex;
    align-items: center;
    padding: 120px 20px 80px;
    background: linear-gradient
