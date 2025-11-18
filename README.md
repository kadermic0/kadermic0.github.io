# kadermic0.github.io
<h1>Website used to reserve private dinner parties</h1>

:root {
    --color-primary: #3A4750;
    --color-secondary: #E3B448;
    --color-background: #F8F8F8;
    --color-text-light: #F8F8F8;

    --font-heading: 'Georgia', serif;
    --font-body: 'Helvetica Neue', Arial, sans-serif;

    --spacing-sm: 0.5rem;
    --spacing-md: 1.5rem;
    --spacing-lg: 3rem;
}

* {
    margin: 0;
    padding: 0;
    box-sizing: border-box;
}

body {
    font-family: var(--font-body);
    color: var(--color-primary);
    background-color: var(--color-background);
    line-height: 1.6;
}

h1, h2, h3, h4 {
    font-family: var(--font-heading);
    margin-bottom: var(--spacing-md);
    color: var(--color-primary);
}

h1 { font-size: 3rem; }
h2 { font-size: 2rem; }
h3 { font-size: 1.75rem; }
h4 { font-size: 1.25rem; }

p { margin-bottom: 1rem; }

/* --- GLOBAL LAYOUT --- */
.container {
    width: 90%;
    max-width: 1200px;
    margin: 0 auto;
    padding: 0; /* Padding handled by section-padding */
}

.section-padding {
    padding: var(--spacing-lg) 0;
}

.section-light {
    background-color: var(--color-background);
}

.section-dark {
    background-color: var(--color-primary);
    color: var(--color-text-light);
}

.section-dark h2, .section-dark h3, .section-dark h4 {
    color: var(--color-secondary);
}

/* --- NAVIGATION & LINKS --- */
a {
    color: var(--color-secondary);
    text-decoration: none;
    transition: color 0.3s;
}

a:hover {
    color: var(--color-primary);
    text-decoration: underline;
}

header .container {
    display: flex;
    justify-content: space-between;
    align-items: center;
}

nav ul {
    list-style: none;
    display: flex; /* Flexbox for horizontal navigation */
    gap: var(--spacing-md);
}

/* --- BUTTONS --- */
.btn {
    display: inline-block;
    padding: 10px 20px;
    background-color: var(--color-secondary);
    color: var(--color-text-light) !important;
    font-weight: bold;
    border: 2px solid var(--color-secondary);
    border-radius: 5px;
    cursor: pointer;
    transition: background-color 0.3s, color 0.3s;
    text-decoration: none !important;
}

.btn:hover {
    background-color: var(--color-primary);
    border-color: var(--color-primary);
}

/* --- HERO SECTION --- */
.hero {
    background-image: url('path/to/restaurant-setting-image.jpg'); /* REPLACE THIS PATH */
    background-size: cover;
    background-position: center;
    height: 70vh;
    display: flex;
    align-items: center;
    padding-left: 5%;
}

.hero-text {
    color: var(--color-text-light);
    background-color: rgba(0, 0, 0, 0.4);
    padding: var(--spacing-sm);
    max-width: 600px;
}

/* --- ABOUT SECTION --- */
.tagline {
    font-size: 1.5rem;
    font-style: italic;
    font-weight: bold;
    margin-top: var(--spacing-md);
    color: var(--color-secondary);
}

/* --- BENEFITS SECTION (Three Columns) --- */
.three-columns {
    display: grid;
    grid-template-columns: repeat(auto-fit, minmax(300px, 1fr)); /* Responsive grid */
    gap: var(--spacing-lg);
    text-align: center;
}

.benefit-card {
    padding: var(--spacing-md);
    border: 1px solid #ddd;
    border-radius: 8px;
    background-color: white;
}

/* --- CONTACT SECTION --- */
.contact-info {
    margin-bottom: var(--spacing-md);
}

.contact-label {
    font-weight: bold;
    margin-bottom: 0;
    color: var(--color-secondary);
}

<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Eat In Bloom - Fine Dining at Home</title>
    <link rel="stylesheet" href="style.css">
</head>
<body>

    <header class="section-padding">
        <div class="container">
            <h1>Eat In Bloom</h1>
            <nav>
                <ul>
                    <li><a href="#about">Hello!</a></li>
                    <li><a href="#tasting-menus">Tasting Menus</a></li>
                    <li><a href="#contact">CONTACT</a></li>
                    <li><a href="#contact" class="btn">BOOK NOW</a></li>
                </ul>
            </nav>
        </div>
    </header>

    <section class="hero">
        <div class="container hero-text">
            <h2>Re-imagine your home as a world class Restaurant</h2>
        </div>
    </section>

    <section id="about" class="section-light section-padding">
        <div class="container">
            <h3>Hello!</h3>
            <p>**It's Mike and Raf!**</p>
            <p>We've been friends and colleagues since 2019 when we met working at Cardinal Spirits. Over the years we have been integral parts of the Bloomington food scene. As founding members of The Elm's culinary team, we worked with Chef Dan Thomas to provide Bloomington with a, much needed, haven for foodies and seekers of flavor. As Chefs we strive towards providing unforgettable experiences for our guests. Now we want to create those memories in YOUR home.</p>
            <p class="tagline">Your Kitchen <br> Our Expertise</p>
        </div>
    </section>

    <section id="tasting-menus" class="section-dark section-padding">
        <div class="container">
            <h2>Tasting Menus at Home</h2>
            <p>Looking for an unforgettable fine dining experience from the comfort of your own home?</p>

            <div class="features-grid">
                <ul>
                    <li>Coursed dinners for groups of 6-12</li>
                    <li>Focus on seasonal ingredients</li>
                    <li>Turn your home into a 3 star restaurant</li>
                    <li>Impress your guests.</li>
                </ul>
            </div>
            
            <a href="#" class="btn menu-btn">See Sample Menu</a>
        </div>
    </section>

    <section class="section-light section-padding">
        <div class="container three-columns">
            <div class="benefit-card">
                <h4>Accommodation.</h4>
                <p>We observe most dietary restrictions so menus can be flexible.</p>
            </div>
            <div class="benefit-card">
                <h4>Relax.</h4>
                <p>We handle all the work so you don't have to.</p>
            </div>
            <div class="benefit-card">
                <h4>Dine in.</h4>
                <p>No need to leave the house to eat something extraordinary.</p>
            </div>
        </div>
    </section>

    <footer id="contact" class="section-dark section-padding">
        <div class="container">
            <h3>CONTACT</h3>
            <div class="contact-info">
                <p class="contact-label">Email:</p>
                <p><a href="mailto:EatInBloom@gmail.com">EatInBloom@gmail.com</a></p>
                <p class="note">This is a side project for both of us so please be patient for responses!</p>
                <br>
                <p class="contact-label">Location:</p>
                <p>Anywhere in Monroe County</p>
            </div>
            <a href="mailto:EatInBloom@gmail.com" class="btn book-now-footer">BOOK NOW</a>
        </div>
    </footer>

</body>
</html>
