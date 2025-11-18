# kadermic0.github.io
<h1>Website used to reserve private dinner parties</h1>

/* --- CSS VARIABLES FOR EASY THEME CHANGES --- */
:root {
    /* Suggested Primary Brand Colors (Sophisticated, Earthy) */
    --color-primary: #3A4750; /* Deep Charcoal/Navy for text and main elements */
    --color-secondary: #E3B448; /* Gold/Mustard for accents (buttons, links) */
    --color-background: #F8F8F8; /* Off-White/Light Gray for background */
    --color-text-light: #F8F8F8;

    /* Suggested Font Families (Elegant, Readable) */
    --font-heading: 'Georgia', serif; /* For titles like 'Eat In Bloom' */
    --font-body: 'Helvetica Neue', Arial, sans-serif; /* For main content */

    /* Basic Spacing */
    --spacing-sm: 0.5rem;
    --spacing-md: 1.5rem;
    --spacing-lg: 3rem;
}

/* --- GLOBAL RESET & BASE STYLES --- */
* {
    margin: 0;
    padding: 0;
    box-sizing: border-box; /* Crucial for responsive design */
}

body {
    font-family: var(--font-body);
    color: var(--color-primary);
    background-color: var(--color-background);
    line-height: 1.6;
}

/* --- TYPOGRAPHY --- */
h1, h2, h3 {
    font-family: var(--font-heading);
    margin-bottom: var(--spacing-md);
    color: var(--color-primary);
}

h1 {
    font-size: 3rem;
}

h2 {
    font-size: 2rem;
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

/* --- BUTTONS (e.g., 'See Sample Menu', 'BOOK NOW') --- */
.btn {
    display: inline-block;
    padding: 10px 20px;
    background-color: var(--color-secondary);
    color: var(--color-text-light);
    font-weight: bold;
    border: 2px solid var(--color-secondary);
    border-radius: 5px;
    cursor: pointer;
    transition: background-color 0.3s, color 0.3s;
}

.btn:hover {
    background-color: var(--color-primary);
    border-color: var(--color-primary);
    color: var(--color-text-light);
}

/* --- UTILITIES & LAYOUT (Use a class like .container for centering content) --- */
.container {
    width: 90%;
    max-width: 1200px;
    margin: 0 auto;
    padding: var(--spacing-md) 0;
}
.hero {
    background-image: url('path/to/restaurant-setting-image.jpg');
    background-size: cover;
    background-position: center;
    height: 70vh; /* Viewport Height for a tall banner */
    display: flex;
    align-items: center; /* Vertically center the content */
    padding-left: 5%;
}

.hero-text {
    color: var(--color-text-light); /* Light text over the dark/rich image */
    background-color: rgba(0, 0, 0, 0.4); /* Semi-transparent overlay for text readability */
    padding: var(--spacing-sm);
    max-width: 600px;
}
