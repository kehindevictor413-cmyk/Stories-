<main>
    <section class="hero">
        <div class="container hero-content">
            <div class="left">
                <h1>Human stories & ideas</h1>
                <p>A place to read, write, and deepen your understanding</p>
                <button class="cta-button">Start Reading</button>
            </div>
            <div class="right">
                <div class="illustration">
                    <!-- Insert illustration or SVG here -->
                </div>
            </div>
        </div>
    </section>

    <section class="features">
        <div class="container">
            <h2>Features</h2>
            <div class="feature-cards">
                <div class="feature-card">
                    <div class="icon">📖</div>
                    <h3>Read Quality Content</h3>
                    <p>Explore articles that inspire and inform.</p>
                </div>
                <div class="feature-card">
                    <div class="icon">✍️</div>
                    <h3>Share Your Ideas</h3>
                    <p>Contribute your thoughts and stories.</p>
                </div>
                <div class="feature-card">
                    <div class="icon">🔗</div>
                    <h3>Connect With Readers</h3>
                    <p>Engage with a community of like-minded individuals.</p>
                </div>
            </div>
        </div>
    </section>
</main>

<footer class="footer">
    <div class="container">
        <ul>
            <li><a href="#">Help</a></li>
            <li><a href="#">Status</a></li>
            <li><a href="#">About</a></li>
            <li><a href="#">Careers</a></li>
            <li><a href="#">Press</a></li>
            <li><a href="#">Blog</a></li>
            <li><a href="#">Privacy</a></li>
            <li><a href="#">Terms</a></li>
        </ul>
    </div>
</footer>

<script src="script.js"></script>
* {
    box-sizing: border-box;
}

body {
    margin: 0;
    font-family: 'Inter', sans-serif;
    background-color: #F5F3EF;
    color: #000;
    line-height: 1.6;
}

.container {
    width: 90%;
    max-width: 1200px;
    margin: auto;
}

.header {
    position: fixed;
    top: 0;
    width: 100%;
    background: rgba(255, 255, 255, 0.9);
    box-shadow: 0 2px 5px rgba(0, 0, 0, 0.1);
    z-index: 1000;
}

.logo {
    font-family: 'Playfair Display', serif;
    font-size: 24px;
    font-weight: bold;
    padding: 15px 0;
}

.nav {
    display: flex;
    justify-content: space-between;
    align-items: center;
}

.nav ul {
    list-style: none;
    display: flex;
    gap: 20px;
    padding: 0;
}

.nav a {
    text-decoration: none;
    color: #000;
}

.get-started {
    background-color: #000;
    color: #fff;
    border: none;
    border-radius: 25px;
    padding: 10px 20px;
    cursor: pointer;
    transition: background 0.3s;
}

.get-started:hover {
    background-color: #333;
}

.hero {
    display: flex;
    align-items: center;
    margin-top: 80px;
    padding: 50px 0;
}

.hero-content {
    display: flex;
    justify-content: space-between;
}

.left {
    flex: 1;
}

.left h1 {
    font-size: 48px;
    font-family: 'Playfair Display', serif;
}

.cta-button {
    background-color: #000;
    color: #fff;
    border: none;
    border-radius: 25px;
    padding: 15px 30px;
    cursor: pointer;
    transition: background 0.3s;
}

.cta-button:hover {
    background-color: #333;
}

.right {
    flex: 1;
    /* Placeholder for illustration */
    display: flex;
    align-items: center;
    justify-content: center;
    height: 300px; /* Example height */
}

.features {
    padding: 50px 0;
}

.feature-cards {
    display: flex;
    justify-content: space-between;
    gap: 20px;
}

.feature-card {
    background: rgba(255, 255, 255, 0.9);
    padding: 20px;
    border-radius: 10px;
    flex: 1;
    text-align: center;
    transition: transform 0.3s;
}

.feature-card:hover {
    transform: scale(1.05);
}

.footer {
    background: #fff;
    padding: 20px 0;
}

.footer ul {
    list-style: none;
    display: flex;
    justify-content: center;
    gap: 20px;
}

.footer a {
    text-decoration: none;
    color: #000;
    transition: color 0.3s;
}

.footer a:hover {
    color: #25C05A;
}
// Smooth scrolling for anchor links
document.querySelectorAll('a[href^="#"]').forEach(anchor => {
    anchor.addEventListener('click', function (e) {
        e.preventDefault();
        document.querySelector(this.getAttribute('href')).scrollIntoView({
            behavior: 'smooth'
        });
    });
});

// Fade-in effect on page load
window.onload = function() {
    document.body.classList.add('fade-in');
};
