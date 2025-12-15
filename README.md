# Ex.07 Restaurant Website
## Date:15/12/25
##Reg.No:25013996

## AIM:
To develop a static Restaurant website to display the food items and services provided by them.

## DESIGN STEPS:

### Step 1:
Requirement collection.

### Step 2:
Creating the layout using HTML and CSS.

### Step 3:
Updating the sample content.

### Step 4:
Choose the appropriate style and color scheme.

### Step 5:
Validate the layout in various browsers.

### Step 6:
Validate the HTML code.

### Step 7:
Publish the website in the given URL.

## PROGRAM:
```
index.html

<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>The Ivory Table</title>
    <style>
        /* General Reset */
* {
    margin: 0;
    padding: 0;
    box-sizing: border-box;
}

body {
    font-family: Arial, sans-serif;
    line-height: 1.6;
    color: #333;
}

a {
    text-decoration: none;
    color: inherit;
}

/* Navigation Bar */
header {
    background-color: #333;
    color: #fff;
    padding: 10px 0;
}

nav {
    display: flex;
    justify-content: space-between;
    align-items: center;
    padding: 0 20px;
}

.nav-links {
    list-style: none;
    display: flex;
}

.nav-links li {
    margin: 0 15px;
}

.nav-links a {
    color: #fff;
    font-size: 18px;
}

/* Hero Section */
.hero {
    background-image: url('home3.jpg'); /* Hero image */
    background-size: cover;
    background-position: center;
    height: 60vh;
    display: flex;
    justify-content: center;
    align-items: center;
    text-align: center;
    color: #fff;
    margin-top: 50px;
}

.hero-content h2 {
    font-size: 3em;
}

.hero-content p {
    font-size: 1.5em;
    margin-bottom: 20px;
}

button {
    background-color: #f2a900;
    color: #fff;
    padding: 10px 20px;
    border: none;
    cursor: pointer;
    font-size: 1.2em;
}

button a {
    color: #fff;
}

/* Menu Section */
#menu {
    padding: 50px 20px;
    text-align: center;
    background-color: #f4f4f4;
}

#menu h2 {
    font-size: 2.5em;
    margin-bottom: 30px;
}

.menu-items {
    display: flex;
    justify-content: center;
    gap: 20px;
    flex-wrap: wrap;
}

.menu-item {
    background-color: #fff;
    padding: 20px;
    border-radius: 8px;
    box-shadow: 0 2px 5px rgba(0, 0, 0, 0.1);
    text-align: center;
    width: 300px;
}

.menu-item img {
    width: 100%;
    height: auto;
    border-radius: 8px;
}

.menu-item h3 {
    font-size: 1.8em;
    margin: 15px 0;
}

.price {
    color: #f2a900;
    font-size: 1.5em;
}

/* Contact Section */
#contact {
    padding: 50px 20px;
    text-align: center;
    background-color: #fff;
}

#contact form {
    max-width: 600px;
    margin: 0 auto;
}

#contact label {
    display: block;
    font-size: 1.2em;
    margin: 10px 0 5px;
}

#contact input,
#contact textarea {
    width: 100%;
    padding: 10px;
    margin: 10px 0 20px;
    border: 1px solid #ccc;
    border-radius: 4px;
}

button[type="submit"] {
    background-color: #f2a900;
    color: #fff;
    padding: 12px 30px;
    border: none;
    font-size: 1.2em;
    cursor: pointer;
}

/* Footer */
footer {
    background-color: #333;
    color: #fff;
    text-align: center;
    padding: 20px;
    margin-top: 150px;
}

    </style>
</head>
<body>
    <!-- Navigation Bar -->
    <header>
        <nav>
            <div class="logo">
                <h1>The Ivory Table</h1>
            </div>
            <ul class="nav-links">
                <li><a href="#home">Home</a></li>
                <li><a href="menu.html">Menu</a></li>
                <li><a href="contact.html">Contact</a></li>
            </ul>
        </nav>
    </header>

    <!-- Hero Section -->
    <section id="home" class="hero">
        <div class="hero-content">
            <h2>Welcome to Our Restaurant!</h2>
            <p>Delicious food, great atmosphere</p>
            <button><a href="./menu.html">Explore Menu</a></button>
        </div>
    </section>

    <footer>
        <p>&copy; 2025 The Ivory Table | All Rights Reserved</p>
    </footer>
</body>
</html>


menu.html

<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>menu</title>
    <style>
        #menu {
    padding: 50px 20px;
    text-align: center;
    background-color: #f4f4f4;
}

#menu h2 {
    font-size: 2.5em;
    margin-bottom: 30px;
}

.menu-items {
    display: flex;
    justify-content: center;
    gap: 20px;
    flex-wrap: wrap;
}

.menu-item {
    background-color: #fff;
    padding: 20px;
    border-radius: 8px;
    box-shadow: 0 2px 5px rgba(0, 0, 0, 0.1);
    text-align: center;
    width: 300px;
}

.menu-item img {
    width: 100%;
    height: auto;
    border-radius: 8px;
}

.menu-item h3 {
    font-size: 1.8em;
    margin: 15px 0;
}

.price {
    color: #f2a900;
    font-size: 1.5em;
}
footer {
    background-color: #333;
    color: #fff;
    text-align: center;
    padding: 20px;
    margin-top: 30px;
}
    </style>
</head>
<body>
    <section id="menu">
        <h2>Our Menu</h2>
        <div class="menu-items">
            <div class="menu-item">
                <img src="chicken.jpg" alt="Dish 1">
                <h3>Garlic Herb Grilled Chicken</h3>
                <p>Grilled chicken seasoned with garlic and herbs, served warm and flavorful.</p>
                <p class="price">$125.00</p>
            </div>
            <div class="menu-item">
                <img src="pasta.jpg" alt="Dish 2">
                <h3>Creamy Alfredo Pasta</h3>
                <p>Pasta in a rich yet comforting cream sauce with a touch of parmesan.</p>
                <p class="price">$90.00</p>
            </div>
            <div class="menu-item">
                <img src="cake.jpg" alt="Dish 3">
                <h3>Chocolate Lava Cake</h3>
                <p>Soft chocolate cake with a warm, melted center. Made with exotic cocoa beans.</p>
                <p class="price">$50.00</p>
            </div>
            <!-- Add more items as needed -->
        </div>
    </section>
    <footer>
        <p>&copy; 2025 The Ivory Table | All Rights Reserved</p>
    </footer>
    
</body>
</html>


contact.html

<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>contact</title>
    <style>
        #contact {
    padding: 50px 20px;
    text-align: center;
    background-color: #fff;
}

#contact form {
    max-width: 600px;
    margin: 0 auto;
}

#contact label {
    display: block;
    font-size: 1.2em;
    margin: 10px 0 5px;
}

#contact input,
#contact textarea {
    width: 100%;
    padding: 10px;
    margin: 10px 0 20px;
    border: 1px solid #ccc;
    border-radius: 4px;

    resize: vertical;
}

button[type="submit"] {
    background-color: #f2a900;
    color: #fff;
    padding: 12px 30px;
    border: none;
    font-size: 1.2em;
    cursor: pointer;
}

/* Footer */
footer {
    background-color: #333;
    color: #fff;
    text-align: center;
    padding: 20px;
    margin-top: 50px;
}
    </style>
</head>
<body>
    <section id="contact">
        <h2>Contact Us</h2>
        <form>
            <label for="name">Name</label>
            <input type="text" id="name" name="name" required>

            <label for="email">Email</label>
            <input type="email" id="email" name="email" required>

            <label for="message">Message</label>
            <textarea id="message" name="message" required ></textarea>

            <button type="submit">Send Message</button>
        </form>
    </section>

    <!-- Footer -->
    <footer>
        <p>&copy; 2025 The Ivory Table | All Rights Reserved</p>
    </footer>
</body>
</html>
```


## OUTPUT:
<img width="1031" height="531" alt="Screenshot 2025-12-15 212731" src="https://github.com/user-attachments/assets/c95d0a22-89b1-4e1d-8db5-ab2b685cc86d" />
<img width="1038" height="524" alt="Screenshot 2025-12-15 212748" src="https://github.com/user-attachments/assets/6c2aeb4a-6d35-4e86-bd38-d26e47f7049d" />
<img width="1036" height="448" alt="Screenshot 2025-12-15 212805" src="https://github.com/user-attachments/assets/423c7aed-95ff-437a-8a19-edd290a87f52" />





## RESULT:
The program for designing software company website using HTML and CSS is completed successfully.
