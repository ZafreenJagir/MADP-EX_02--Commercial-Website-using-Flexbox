# Ex02 Commercial Website
## Date: 11-08-2025

## AIM
To create a commercial website using CSS Flexbox.

## ALGORITHM
### STEP 1
Create an HTML file (index.html)

### STEP 2
Create a CSS file (style.css)

### STEP 3
Include a navigation bar with links to different sections.

### STEP 4
Add structured sections for Homepage, Products / Services, About Us, Contact Details and User Account.

### STEP 5
Include social media links at the footer with copyright information.

### STEP 6
Define global styles for fonts, colors, and layout.

### STEP 7
Style the header, navigation bar, and sections.

### STEP 8
Use Flexbox for layout design.

### STEP 9
Add hover effects and transitions for interactivity.

### STEP 10
Add Images and Media.

### STEP 11
Use optimized images for a professional look.

### STEP 12
Open the HTML file in a browser to check layout and functionality.

### STEP 13
Fix styling issues and refine content placement.

### STEP 14
Deploy the website.

### STEP 15
Upload to GitHub Pages for free hosting.

## PROGRAM

indexx.html

```
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1" />
  <title>Z_Hennas | Beautiful Henna Art</title>
  <link rel="stylesheet" href="styles.css" />
</head>
<body>

  <header>
    <h1>Z_Hennas</h1>
    <nav>
      <a href="#services">Services</a>
      <a href="#about">About</a>
      <a href="#contact">Contact</a>
    </nav>
  </header>

  <section class="hero">
    Beautiful Henna Designs for Every Occasion
  </section>

  <div class="container">
    <section id="services" class="services">
      <div class="service-card">
        <img src="C:\Users\admin\Desktop\bridall.jpg" alt="Bridal Henna" />
        <h3>Bridal Henna</h3>
        <p>Elegant, intricate bridal mehndi designs to make your special day unforgettable.</p>
      </div>
      <div class="service-card">
        <img src="C:\Users\admin\Desktop\party.jpg" alt="Party Henna" />
        <h3>Party Designs</h3>
        <p>Fun and trendy henna patterns perfect for parties and social gatherings.</p>
      </div>
      <div class="service-card">
        <img src="C:\Users\admin\Desktop\customizeart.jpg" alt="Custom Henna Art" />
        <h3>Custom Art</h3>
        <p>Personalized henna designs tailored to your unique style and preferences.</p>
      </div>
    </section>

    <section id="about" class="about">
      <h2>About Z_Hennas</h2>
      <p>At Z_Hennas, we specialize in creating beautiful and lasting henna designs for all occasions. We use safe henna to bring your vision to life, whether it’s for weddings, festivals, or just for fun.</p>
    </section>

    <section id="contact" class="contact-form">
      <h2>Contact Us</h2>
      <form>
        <label for="name">Name</label>
        <input type="text" id="name" name="name" placeholder="Your full name" required />

        <label for="email">Email</label>
        <input type="email" id="email" name="email" placeholder="you@example.com" required />

        <label for="message">Message</label>
        <textarea id="message" name="message" rows="5" placeholder="Your message here..." required></textarea>

        <button type="submit">Send Message</button>
      </form>
    </section>
  </div>

  <footer>
    <p>Follow us on Instagram <a href="https://www.instagram.com/z_hennas_" target="_blank" rel="noopener noreferrer">@z_hennas_</a></p>
  </footer>

</body>
</html>


```


styles.css
```
/* Reset some basic styles */
* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
}

body {
  font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
  background: #fff8f0;
  color: #4b3b2b;
  line-height: 1.6;
}

header {
  background: #7e4a35;
  color: white;
  padding: 20px 40px;
  display: flex;
  justify-content: space-between;
  align-items: center;
}

header h1 {
  font-family: 'Brush Script MT', cursive;
  font-size: 2rem;
  letter-spacing: 2px;
}

nav a {
  color: white;
  text-decoration: none;
  margin-left: 20px;
  font-weight: 600;
}

nav a:hover {
  text-decoration: underline;
}

.hero {
  background: #f8e7d1;
  height: 350px;
  display: flex;
  justify-content: center;
  align-items: center;
  color: #fff;
  text-shadow: 2px 2px 4px #000;
  font-size: 2.5rem;
  font-weight: bold;
  text-align: center;
  padding: 0 20px;
}

.container {
  max-width: 1000px;
  margin: 40px auto;
  padding: 0 20px;
}

.services {
  display: flex;
  justify-content: space-between;
  gap: 20px;
  margin-bottom: 60px;
  flex-wrap: wrap;
}

.service-card {
  background: #f8e7d1;
  padding: 20px;
  border-radius: 8px;
  flex: 1 1 300px;
  box-shadow: 2px 2px 8px rgba(0,0,0,0.1);
  transition: transform 0.3s ease;
  cursor: default;
  display: flex;
  flex-direction: column;
  align-items: center;
  text-align: center;
}

.service-card:hover {
  transform: translateY(-5px);
  box-shadow: 4px 4px 12px rgba(0,0,0,0.15);
}

.service-card img {
  width: 100%;
  height: 320px;
  object-fit: cover;
  border-top-left-radius: 15px;
  border-top-right-radius: 15px;
}

.service-card h3 {
  margin-bottom: 15px;
  color: #7e4a35;
}

.about {
  background: #f1d7b0;
  padding: 30px;
  border-radius: 8px;
  margin-bottom: 60px;
}

.contact-form {
  background: #fff;
  padding: 30px;
  border-radius: 8px;
  box-shadow: 0 0 10px rgba(0,0,0,0.1);
}

.contact-form h2 {
  margin-bottom: 20px;
  color: #7e4a35;
  text-align: center;
}

.contact-form label {
  display: block;
  margin-bottom: 8px;
  font-weight: 600;
}

.contact-form input,
.contact-form textarea {
  width: 100%;
  padding: 10px;
  margin-bottom: 20px;
  border: 1px solid #ccc;
  border-radius: 4px;
  font-size: 1rem;
  resize: vertical;
}

.contact-form button {
  background: #7e4a35;
  color: white;
  border: none;
  padding: 12px 25px;
  font-size: 1rem;
  border-radius: 4px;
  cursor: pointer;
  transition: background 0.3s ease;
  display: block;
  margin: 0 auto;
}

.contact-form button:hover {
  background: #5d3a27;
}

footer {
  background: #7e4a35;
  color: white;
  text-align: center;
  padding: 15px 20px;
  margin-top: 40px;
  font-size: 0.9rem;
}

footer a {
  color: #f9d5b4;
  text-decoration: none;
  font-weight: 600;
}

footer a:hover {
  text-decoration: underline;
}

@media (max-width: 768px) {
  .services {
    flex-direction: column;
  }

  nav {
    display: none;
  }
}


```


## OUTPUT

<img width="1891" height="1045" alt="Screenshot 2025-08-11 182428" src="https://github.com/user-attachments/assets/853e6db0-4578-41bc-b714-56b3ca7f39b2" />


<img width="1885" height="1037" alt="Screenshot 2025-08-11 182445" src="https://github.com/user-attachments/assets/0c171193-f108-49db-a800-6abb1139f94c" />


<img width="1889" height="1046" alt="Screenshot 2025-08-11 182459" src="https://github.com/user-attachments/assets/6d7cd3ef-69b4-49aa-8ca1-03f105a6a071" />



## RESULT
The program for creating commercial website using CSS Flexbox is executed successfully.
