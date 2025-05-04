# Ex.07 Restaurant Website
# Date:30-04-2025
# AIM:
To develop a static Restaurant website to display the food items and services provided by them.

# DESIGN STEPS:
## Step 1:
Requirement collection.

## Step 2:
Creating the layout using HTML and CSS.

## Step 3:
Updating the sample content.

## Step 4:
Choose the appropriate style and color scheme.

## Step 5:
Validate the layout in various browsers.

## Step 6:
Validate the HTML code.

## Step 7:
Publish the website in the given URL.

# PROGRAM:
```
home.html

<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <title>Delicious Bites | Restaurant</title>
  <link rel="stylesheet" href="style.css" />
</head>
<body>

  <centre>
  <nav>
    <!-- Optional Logo -->
    <div style="display: flex; align-items: center;">
      <img src="logo.png" alt="Delicious Bites Logo" style="height: 40px; margin-right: 10px;">
      <h1 style="color: #000000;">Delicious Bites</h1>
    </div>
    <div>
      <a href="#home">Home</a>
      <a href="#menu">Menu</a>
      <a href="#about">About</a>
      <a href="#contact">Contact</a>
    </div>
  </nav>

  <!-- Hero Section -->
  <section class="hero" id="home">
    <h1 style="color: #ab8445;">Welcome to Delicious Bites</h1>
    <p style="color: #1f1e1b;">Experience gourmet flavors with fresh ingredients and passionate chefs.</p> 
  </section>

  <!-- Menu Section -->
  <section class="menu" id="menu">
    <h2>Top Foods From Our Menu</h2>
    <div class="menu-items">
      <div class="menu-item">
        <img src="salmon.jpg" alt="Grilled Salmon" style="width:100%; border-radius: 8px;">
        <h3>Grilled Salmon</h3>
        <p>Fresh Atlantic salmon grilled to perfection, served with seasonal vegetables.</p>
      </div>
      <div class="menu-item">
        <img src="pizza.jpg" alt="Margherita Pizza" style="width:100%; border-radius: 8px;">
        <h3>Margherita Pizza</h3>
        <p>Classic wood-fired pizza with mozzarella, basil, and tomato sauce.</p>
      </div>
      <div class="menu-item">
        <img src="spagetti.jpg" alt="Spaghetti Carbonara" style="width:100%; border-radius: 8px;">
        <h3>Spaghetti Carbonara</h3>
        <p>Authentic Italian pasta tossed in creamy egg and pancetta sauce.</p>
      </div>
      <div class="menu-item">
        <img src="cake.jpg" alt="Chocolate Lava Cake" style="width:100%; border-radius: 8px;">
        <h3>Chocolate Lava Cake</h3>
        <p>Warm molten chocolate cake served with vanilla ice cream.</p>
      </div>
    </div>
  </section>

  <!-- Chefs Section -->
<section class="chefs" id="chefs">
    <h2>Meet Our Chefs</h2>
    <div class="chef-cards">
      <div class="chef">
        <img src="rafi.jpg" alt="Chef Rafi">
        <h3>Chef Rafi</h3>
        <p>Head Chef – Italian Cuisine</p>
      </div>
      <div class="chef">
        <img src="ravi.jpg" alt="Chef Ravi">
        <h3>Chef Ravi</h3>
        <p>Pastry Chef</p>
      </div>
      <div class="chef">
        <img src="hari.jpg" alt="Chef Hari">
        <h3>Chef Hari</h3>
        <p>Grill Master</p>
      </div>
      <div class="chef">
        <img src="madhes.jpg" alt="Chef Madhesh">
        <h3>Chef Madhesh</h3>
        <p>Sushi & Fusion</p>
      </div>
    </div>
  </section>
  

  <!-- About Section -->
  <section class="about" id="about">
    <h2>About Us</h2>
    <img src="restaurant.jpg" alt="" style="width: 100%; max-width: 800px; border-radius: 12px; margin-bottom: 1rem;">
    <p>
      At Delicious Bites, we believe in crafting unforgettable culinary experiences.
      Our chefs use the freshest ingredients to create dishes that delight your taste buds
      in a cozy and welcoming atmosphere.
    </p>
  </section>

  <!-- Footer -->
  <footer id="contact">

    <p>123 Flavor Street, Foodie City, FL 12345</p>
    <p>Email: info@deliciousbites.com | Phone: 8870864909</p>
    <p>&copy; 2025 Delicious Bites. All rights reserved.</p>
  </footer>

</body>
</html>
```
```
style.css

/* Global Styles */
* {
    margin: 0;
    padding: 0;
    box-sizing: border-box;
  }
  
  body {
    font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
    line-height: 1.6;
    color: #333;
    background-color: #fff;
  }
  
  /* Navigation */
  nav {
    background-color: #ab8445;
    padding: 1rem 2rem;
    display: flex;
    justify-content: space-between;
    align-items: center;
  }
  
  nav a {
    color: #fff;
    text-decoration: none;
    margin-left: 1.5rem;
    font-weight: bold;
  }
  
  nav a:hover {
    color: #f39c12;
  }
  
  /* Hero Section */
  .hero {
    background: url('background.jpg') center/cover no-repeat;
    height: 90vh;
    color: rgb(0, 0, 0);
    display: flex;
    flex-direction: column;
    justify-content: center;
    align-items: center;
    text-align: center;
    padding: 0 2rem;
  }
  
  .hero h1 {
    font-size: 4rem;
    margin-bottom: 1rem;
    text-shadow: 2px 2px 4px #000;
  }
  
  .hero p {
    font-size: 1.5rem;
    max-width: 600px;
  }
  
  /* Menu Section */
  .menu {
    padding: 4rem 2rem;
    background-color: #ab8445;
    text-align: center;
  }
  
  .menu h2 {
    font-size: 2.5rem;
    margin-bottom: 2rem;
  }
  
  .menu-items {
    display: grid;
    grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
    gap: 2rem;
  }
  
  .menu-item {
    background: #fff;
    padding: 1.5rem;
    border-radius: 10px;
    box-shadow: 0 2px 10px rgba(0, 0, 0, 0.1);
  }
  
  .menu-item h3 {
    margin-bottom: 0.5rem;
    color: #e67e22;
  }
  
  .menu-item p {
    font-size: 0.95rem;
    color: #666;
  }
  
  /* About Section */
  .about {
    background: url(blur.jpg) center/cover no-repeat;
    background-color: #ffffff;
    padding: 4rem 2rem;
    color: #fff;
    text-align: center;
  }
  
  .about h2 {
    font-size: 2.5rem;
    margin-bottom: 1.5rem;
  }
  
  .about p {
    max-width: 800px;
    margin: 0 auto;
    font-size: 1.1rem;
    color: #ffffff;
  }
  
  /* Contact / Footer */
  footer {
    background-color: #ffffff;
    color: #ffffff;
    background: url('res.jpg') center/cover no-repeat;
    text-align: center;
    padding: 2rem;
    margin-top: 2rem;
  }
  
  footer p {
    margin: 0.5rem 0;
  }
  
  /* Responsive Tweaks */
  @media (max-width: 768px) {
    .hero h1 {
      font-size: 4.5rem;
    }
  
    .hero p {
      font-size: 1rem;
    }
  }
  .hero-title {
    position: relative;
    display: inline-block;
    padding: 1rem 2rem;
    background: url('welcome.jpeg') center/cover no-repeat;
    color: rgb(187, 161, 69);
    font-size: 4rem;
    border-radius: 12px;
    text-shadow: 1px 1px 3px rgba(0,0,0,0.7);
  }
  .chefs {
    padding: 4rem 2rem;
    text-align: center;
    background-color: #ab8445;
  }
  
  .chefs h2 {
    font-size: 2.5rem;
    margin-bottom: 2rem;
    color: #2c3e50;
  }
  
  .chef-cards {
    display: grid;
    grid-template-columns: repeat(auto-fit, minmax(220px, 1fr));
    gap: 2rem;
    justify-items: center;
  }
  
  .chef {
    background: #ffffff;
    padding: 2.5rem;
    border-radius: 12px;
    box-shadow: 0 2px 12px rgba(0, 0, 0, 0.05);
    transition: transform 0.3s ease;
  }
  
  .chef:hover {
    transform: scale(1.05);
  }
  
  .chef img {
    width: 100%;
    max-width: 180px;
    height: auto;
    border-radius: 100%;
    margin-bottom: 1rem;
  }
  
  .chef h3 {
    font-size: 2.25rem;
    margin: 0.5rem 0 0.25rem;
    color: #000000;
  }
  
  .chef p {
    color: #ab8445;
    font-size: 0.95rem;
  }
  ```


# OUTPUT:
![Screenshot 2025-05-04 145943](https://github.com/user-attachments/assets/6fe6e7a9-04f5-4d68-acfa-eabeb507cf6d)
![Screenshot 2025-05-04 145933](https://github.com/user-attachments/assets/0535238e-4ffc-4e59-b33a-1e4bd2f559d1)
![Screenshot 2025-05-04 145918](https://github.com/user-attachments/assets/a4b7a10f-3ade-412e-a10f-9c07e6d07682)
![Screenshot 2025-05-04 145949](https://github.com/user-attachments/assets/1cd28d35-9c07-4894-8f1a-3e99035fbf5d)

# RESULT:
The program for designing software company website using HTML and CSS is completed successfully.
