# Ex04 Places Around Me
# Date: 28/11/2024
# AIM
To develop a website to display details about the places around my house.

# DESIGN STEPS
## STEP 1
Create a Django admin interface.

## STEP 2
Download your city map from Google.

## STEP 3
Using <map> tag name the map.

## STEP 4
Create clickable regions in the image using <area> tag.

## STEP 5
Write HTML programs for all the regions identified.

## STEP 6
Execute the programs and publish them.

# CODE
```
map.html
<!DOCTYPE html>
<html>
    <body>
        <div style="text-align: center;">
        <h1> Explore My Neighbourhood</h1>
        <h2> Please click any of the pictures in the middle to know more about it</h2>
        
            <div style="text-align: center;">
            <img src="Screenshot 2024-10-19 111347.png" alt=""  usemap="#Landmark" style="width: fit-content;">
            </div>
         <map name="Landmark">
            <area shape="circle" coords="403,347,13" title="zudio" href="zu.html">
            <area shape="rect" coords="674,608,688,606" title="public food shelter" href="res.html"> 
            <area shape="circle" coords="1192,542,15" title="one plus experience store" href="one.html">
        </map>
        </div>
    </body>
</html>

zudio.html

<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Zudio - Affordable Fashion</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            margin: 0;
            padding: 0;
            background-color: #f9f9f9;
            color: #333;
        }
        header {
            background-color: #000;
            color: #fff;
            text-align: center;
            padding: 20px;
        }
        nav {
            display: flex;
            justify-content: center;
            background-color: #444;
            padding: 10px 0;
        }
        nav a {
            color: white;
            padding: 10px 20px;
            text-decoration: none;
            text-transform: uppercase;
        }
        nav a:hover {
            background-color: #666;
        }
        section {
            padding: 20px;
            text-align: center;
        }
        .products {
            display: flex;
            flex-wrap: wrap;
            justify-content: center;
            gap: 20px;
        }
        .product {
            background-color: #fff;
            border: 1px solid #ddd;
            border-radius: 10px;
            padding: 15px;
            width: 250px;
            text-align: center;
        }
        .product img {
            max-width: 100%;
            border-radius: 10px;
        }
        footer {
            background-color: #000;
            color: #fff;
            text-align: center;
            padding: 10px 0;
            margin-top: 20px;
        }
        .contact-form input, .contact-form textarea, .contact-form button {
            width: 100%;
            padding: 10px;
            margin: 10px 0;
        }
        .contact-form {
            max-width: 500px;
            margin: 0 auto;
        }
    </style>
</head>
<body>
    <header>
        <h1>Zudio</h1>
        <p>Style that Defines You</p>
    </header>
    <nav>
        <a href="#products">Products</a>
        <a href="#about">About Us</a>
        <a href="#contact">Contact</a>
    </nav>
    <section id="products">
        <h2>Our Collections</h2>
        <div class="products">
            <div class="product">
                <img src="imagesmen.jpg" alt="Men's Wear">
                <h3>Men's Wear</h3>
                <p>Trendy styles at unbeatable prices.</p>
            </div>
            <div class="product">
                <img src="women.jpg" alt="Women's Wear">
                <h3>Women's Wear</h3>
                <p>Fashion-forward outfits for every occasion.</p>
            </div>
            <div class="product">
                <img src="kids.jpg" alt="Kids' Wear">
                <h3>Kids' Wear</h3>
                <p>Comfortable and stylish apparel for kids.</p>
            </div>
        </div>
    </section>
    <section id="about">
        <h2>About Zudio</h2>
        <p>Zudio is your one-stop destination for affordable and stylish clothing for all ages. Our goal is to make fashion accessible to everyone, with a wide range of products that cater to diverse tastes and preferences.</p>
    </section>
    <footer>
        <p>&copy; 2024 Zudio. All rights reserved.</p>
    </footer>
</body>
</html>

oneplua.html

<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>OnePlus - Never Settle</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            margin: 0;
            padding: 0;
            background-color: #f4f4f4;
            color: #333;
        }
        header {
            background-color: #000;
            color: #fff;
            padding: 10px 20px;
            text-align: center;
        }
        nav {
            display: flex;
            justify-content: center;
            background-color: #333;
        }
        nav a {
            color: #fff;
            padding: 10px 20px;
            text-decoration: none;
            text-transform: uppercase;
        }
        nav a:hover {
            background-color: #555;
        }
        section {
            padding: 20px;
            text-align: center;
        }
        .products {
            display: flex;
            justify-content: center;
            gap: 20px;
            flex-wrap: wrap;
        }
        .product {
            border: 1px solid #ddd;
            border-radius: 10px;
            padding: 20px;
            background-color: #fff;
            width: 300px;
        }
        .product img {
            max-width: 100%;
            border-radius: 10px;
        }
        footer {
            text-align: center;
            padding: 10px;
            background-color: #000;
            color: #fff;
            margin-top: 20px;
        }
        .contact-form input, .contact-form textarea, .contact-form button {
            width: 100%;
            margin: 10px 0;
            padding: 10px;
        }
    </style>
</head>
<body>
    <header>
        <h1>OnePlus</h1>
        <p>Never Settle</p>
    </header>
    <nav>
        <a href="#products">Products</a>
        <a href="#about">About Us</a>
        <a href="#contact">Contact</a>
    </nav>
    <section id="products">
        <h2>Our Products</h2>
        <div class="products">
            <div class="product">
                <img src="download.jpg" alt="OnePlus Phone">
                <h3>OnePlus 11</h3>
                <p>Experience ultimate speed and performance.</p>
            </div>
            <div class="product">
                <img src="buds.jpg" alt="OnePlus Buds">
                <h3>OnePlus Buds Pro 2</h3>
                <p>Immersive sound with active noise cancellation.</p>
            </div>
        </div>
    </section>
    <section id="about">
        <h2>About Us</h2>
        <p>OnePlus is a global technology company committed to creating cutting-edge devices that enhance user experiences. Our philosophy, "Never Settle," drives us to continually innovate and exceed expectations.</p>
    </section>
    <section id="contact">
        <h2>Contact Us</h2>
        <form class="contact-form">
            <input type="text" placeholder="Your Name" required>
            <input type="email" placeholder="Your Email" required>
            <textarea rows="5" placeholder="Your Message" required></textarea>
            <button type="submit">Send</button>
        </form>
    </section>
    <footer>
        <p>&copy; 2024 OnePlus. All rights reserved.</p>
    </footer>
</body>
</html>

restaurant.html

            <p><strong> ₹270</strong></p>

```
# OUTPUT
![Screenshot 2024-12-07 214705](https://github.com/user-attachments/assets/846fc417-eda4-40f9-bf30-451426d65225)
![Screenshot 2024-12-07 214723](https://github.com/user-attachments/assets/f52ea0e1-73f0-49b3-8119-a7b88a791653)
![Screenshot 2024-12-07 215031](https://github.com/user-attachments/assets/0710a16e-cba5-4e37-9462-051e859a5f72)
![Screenshot 2024-12-07 215346](https://github.com/user-attachments/assets/90253194-8838-452b-8418-ea8e1055a422)
![image](https://github.com/user-attachments/assets/48bd983c-3e3d-4ff0-a3b0-149fe5dcad98)


# RESULT
The program for implementing image maps using HTML is executed successfully.
