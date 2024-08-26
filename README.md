<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Landing Page</title>
    <link rel="stylesheet" href="styles.css">
<style>
    /* General Styles */
body {
    font-family: Arial, sans-serif;
    margin: 0;
    padding: 0;
    color: #333;
}
.hero {
    background: url('hero-image.jpg') no-repeat center center/cover;
    height: 100vh;
    display: flex;
    align-items: center;
    justify-content: center;
    color: white;
    text-align: center;
}
.hero .container {
    max-width: 800px;
}
.hero h1 {
    font-size: 3rem;
    margin-bottom: 10px;
}
.hero p {
    font-size: 1.2rem;
    margin-bottom: 20px;
}
.hero .btn {
    padding: 10px 20px;
    background-color: #ff6600;
    color: white;
    border: none;
    text-decoration: none;
    font-size: 1rem;
    border-radius: 5px;
}
.hero .btn:hover {
    background-color: #ff4500;
}
/* Features Section */
.features {
    padding: 50px 0;
    background-color: #f4f4f4;
}
.features .container {
    max-width: 1000px;
    margin: auto;
    text-align: center;
}
.features h2 {
    margin-bottom: 40px;
    font-size: 2.5rem;
}
.feature-box {
    background-color: white;
    padding: 20px;
    margin: 20px;
    border-radius: 10px;
    box-shadow: 0 4px 8px rgba(0, 0, 0, 0.1);
}
.feature-box h3 {
    margin-bottom: 15px;
    font-size: 1.5rem;
}
/* Contact Section */
.contact {
    padding: 50px 0;
}
.contact .container {
    max-width: 800px;
    margin: auto;
    text-align: center;
}
.contact h2 {
    margin-bottom: 40px;
    font-size: 2.5rem;
}
.contact input, .contact textarea {
    width: 100%;
    padding: 15px;
    margin: 10px 0;
    border: 1px solid #ddd;
    border-radius: 5px;
    font-size: 1rem;
}
.contact button {
    padding: 10px 20px;
    background-color: #ff6600;
    color: white;
    border: none;
    font-size: 1rem;
    border-radius: 5px;
    cursor: pointer;
}
.contact button:hover {
    background-color: #ff4500;
}
/* Responsive Design */
@media (max-width: 768px) {
    .hero h1 {
        font-size: 2rem;
    }
    .features h2, .contact h2 {
        font-size: 2rem;
    }
    .feature-box, .contact input, .contact textarea {
        padding: 10px;    }
}
</style>
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

  <script src="script.js">
      document.getElementById('contactForm').addEventListener('submit', function(e) {
    e.preventDefault();

    const name = document.getElementById('name').value;
    const email = document.getElementById('email').value;
    const message = document.getElementById('message').value;

    if (name && email && message) {
        document.getElementById('formMessage').innerText = `Thank you, ${name}! We will get back to you soon.`;
        document.getElementById('contactForm').reset();
    } else {
        document.getElementById('formMessage').innerText = 'Please fill in all fields.';
    }
});

  </script>
</body>
</html>
