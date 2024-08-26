
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Landing Page</title>
    <link rel="stylesheet" href="styles.css">
</head>
<body>
    <!-- Hero Section -->
    <header class="hero">
        <div class="container">
            <h1>Welcome to Our Website</h1>
            <p>Discover our amazing features and services.</p>
            <a href="#features" class="btn">Learn More</a>
        </div>
    </header>

    <!-- Features Section -->
    <section id="features" class="features">
        <div class="container">
            <h2>Our Features</h2>
            <div class="feature-box">
                <h3>Feature One</h3>
                <p>Details about feature one.</p>
            </div>
            <div class="feature-box">
                <h3>Feature Two</h3>
                <p>Details about feature two.</p>
            </div>
            <div class="feature-box">
                <h3>Feature Three</h3>
                <p>Details about feature three.</p>
            </div>
        </div>
    </section>

    <!-- Contact Section -->
    <section id="contact" class="contact">
        <div class="container">
            <h2>Contact Us</h2>
            <form id="contactForm">
                <input type="text" id="name" placeholder="Your Name" required>
                <input type="email" id="email" placeholder="Your Email" required>
                <textarea id="message" placeholder="Your Message" required></textarea>
                <button type="submit" class="btn">Send Message</button>
            </form>
            <p id="formMessage"></p>
        </div>
    </section>

    <script src="script.js"></script>
</body>
</html>
