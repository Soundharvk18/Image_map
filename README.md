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

oneplus.html

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


<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <meta name="description" content="Welcome to One8 Restaurant - Delight in Exquisite Cuisines.">
    <title>One8 Restaurant</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            margin: 0;
            padding: 0;
            background-color: black;
        }

        header {
            background-image: url("download.png");
            background-repeat: no-repeat;
            object-fit: cover;
            color: white;
            padding: 15px 0;
            text-align: center;
        }

        nav ul {
            list-style: none;
            margin: 0;
            padding: 0;
            display: flex;
            justify-content: center;
            background-color: #444;
        }

        nav ul li {
            margin: 0 15px;
        }

        nav ul li a {
            color: white;
            text-decoration: none;
            padding: 14px 20px;
            display: block;
        }

        nav ul li a:hover {
            background-color: #555;
        }

        section {
            padding: 20px;
            margin: 20px;
            background-color: white;
            border-radius: 8px;
            box-shadow: 0 0 10px rgba(0,0,0,0.1);
        }

        footer {
            background-color: black;
            color: white;
            text-align: center;
            padding: 2px ;
            position: fixed;
            bottom: 0;
            width: 100%;
        }

        h1 {
            color: white;
        }

        .menu-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(200px, 1fr));
            gap: 20px;
            padding: 20px;
        }
        .image1{
            background-color: #f9f9f9;
            padding: 20px;
            border-radius: 8px;
            text-align: center;
            box-shadow: 0 0 10px rgba(0,0,0,0.1);
        }

        .menu-item {
            background-color: #f9f9f9;
            padding: 20px;
            border-radius: 8px;
            text-align: center;
            box-shadow: 0 0 10px rgba(0,0,0,0.1);
        }

        .menu-item h3 {
            margin: 0 0 10px 0;
        }

        .menu-item p {
            color: #666;
        }
        
      </style>
</head>
<body>

<header>
    <h1>One8 Restaurant</h1>
    <p>Delight in Exquisite Cuisines</p>
</header>

<nav>
    <ul>
        <li><a href="#home">Home</a></li>
        <li><a href="#menu">Menu</a></li>
        <li><a href="#image">image</a></li>
        <li><a href="#admini">Administration</a></li>
        <li><a href="#about">About Us</a></li>
        
        <li><a href="#contact">Contact</a></li>
    </ul>
</nav>

<section id="home">
    <h2>Welcome to One8 Restaurant</h2>
    <p>At One8, we serve the finest dishes made from the freshest ingredients. Our chefs are dedicated to bringing you an unforgettable dining experience, where great food meets warm hospitality. We are dedicated to providing you with an unforgettable dining experience, featuring fresh ingredients and bold flavors. Whether you're here for a casual meal or a special occasion, we look forward to serving you. Enjoy your time at one8!</p>
</section>

<section id="menu">
    <h2>Our Menu</h2>
    <div class="menu-grid" >
        <div class="menu-item">
            <img src="salman.jpg">
            <h3>Grilled Salmon</h3>
            <p>Freshly grilled salmon with a side of vegetables.</p>
            <p><strong> ₹440</strong></p>
        </div>
        <div class="menu-item">
            <img src="c:\Users\admin\Downloads\filet migon.jpg" width="100%">
            <h3>Filet Mignon</h3>
            <p>Tender filet mignon served with mashed potatoes and asparagus.</p>
            <p><strong> ₹380</strong></p>
        </div>
        <div class="menu-item">
            <img src="seisar.jpg" width="100%">
            <h3>Caesar Salad</h3>
            <p>Crispy romaine lettuce with parmesan and Caesar dressing.</p>
            <p><strong> ₹270</strong></p>
        </div>
        <div class="menu-item">
            <img src="salad.jpg" width="100%">
            <h3>super food salad</h3>
            <p>assorted mesclun green, roasted pumpkin seeds, cantaloupe melon, amaranth seeds</p>
            <p><strong> ₹310</strong></p>
        </div>
        <div class="menu-item">
            <img src="pasta.jpg" width="100%">
            <h3>Pasta Primavera</h3>
            <p>Penne pasta with fresh vegetables in a light garlic sauce.</p>
            <p><strong> ₹520</strong></p>
        </div>
        <div class="menu-item">
            <img src="avacada.jpg" width="100%">
            <h3>Tartar Topped On Avocado</h3>
            <p>with crispy corn, sriracha, scallion, japanese spicy mayonnaise </p>
            <p><strong> ₹460</strong></p>
        </div>
        <div class="menu-item">
            <img src="mush.jpg" width="100%">
            <h3>Mushroom Googly </h3>
            <p>assorted wild mushrooms, cream cheese, vegetarian broth, truffle oil            </p>
            <p><strong> ₹460</strong></p>
        </div>
        <div class="menu-item">
            <img src="cheese.jpg" width="100%">
            <h3>cheese board </h3>
            <p>choice of cheese selections, fresh fruits, relish and crackers            </p>
            <p><strong> ₹1245</strong></p>
        </div>
        <div class="menu-item">
            <img src="charcute.jpg" width="100%">
            <h3>Charcutiere Board            </h3>
            <p>choice of cold cut selections, pickles vegetables, relish and crackers           </p>
            <p><strong> ₹1475</strong></p>
        </div>
        <div class="menu-item">
            <img src="buratta.jpg" width="100%">
            <h3>Deconstructed Buratta            </h3>
            <p>olive tapenade, sweet and sour jam, sour dough            </p>
            <p><strong> ₹775</strong></p>
        </div>
        <div class="menu-item">
            <img src="phyiio.jpg" width="100%">
            <h3>Phyllo Baked            </h3>
            <p>raw papaya relish, California grapes and truffle honey drizzle          </p>
            <p><strong> ₹695</strong></p>
        </div>
        <div class="menu-item">
            <img src="beirut.jpg" width="100%">
            <h3> Beirut Hummus</h3>
            <p>Assorted lavash stick,olive,pita,fattoush salad and pickles</p>
            <p><strong> ₹560</strong></p>
        </div>
<section id="admini">
    <h2>Administration</h2>
    <div class="menu-grid">
        <div class="menu-item">
        <img src="viratcasual.jpg">
            <h3>Founder</h3>
            <p>Virat kohli</p>
        </div>
        <div class="menu-grid">
        <img src="c:\web developmebt\manager.jpg">
        <h3>Co-Founder</h3>
        <p>dhinesh</p>
        </div>
        <a href="https://www.instagram.com/shraddhakapoor/?hl=en"></a>
        <img src="WhatsApp Image 2024-11-25 at 13.35.59_c5bd1e50.jpg" width="100%" height="70%">
        <h3>Brand ambassador </h3>
        <p>Deepan adhithya</p>
        </div>
        <div class="menu-grid">
            <img src="soundhar1.jpg" width="100%" height="70%">
            <h3>Brand ambassador</h3>
            <p>soundhar</p>
        </div>

        <div class="menu-grid">
            <img src="monish.jpg" width="100%">
            <h3>manager</h3>
            <p>monish</p>
        </div>
        <div class="menu-grid">
            <img src="danu.jpg" width="100%">
            <h3>Chief Chef</h3>
            <p>chef Damu</p>
        </div>
    
        <div class="administration">
            <img src="venkatesh.jpg" width="100%">
            <h3>Assistant Chef</h3>
            <p>venkatesh batt</p>
        </div>

</div>
</section>
<section id="image">
    <div class="menu-grid">
        <div class="image1">
           <img src="download7.jpg" width="100%">
        </div>
        <div class="image1">
           <img src="download1.jpg" width="100%">
        </div>
        <div class="image1">
           <img src="download2.jpg" width="100%">
        </div>
        <div class="image1">
            <img src="download3.jpg" width="100%">
        </div>
        <div class="image1">
            <img src="download8.jpg" width="105%">
        </div>
    </div>
</section>

<section id="about">
    <h2>About Us</h2>
    <p>One8 Restaurant was founded with the vision of creating a dining experience like no other. Our passion for food and hospitality drives us to continuously innovate and serve dishes that captivate the senses.</p>
</section>

<section id="contact">
    <h2>Contact Us</h2>
    <p>123 Flavor Street, Gourmet City,bangal0re</p>
    <p>Phone: 9360723703</p>
    <p>Email: one8restaurant18@gmail.com</p>
</section>

<footer>
    <p><strong>One8</strong>&copy; Created by Jeya Soundhar</p>
</footer>

</body>
</html>


```
# OUTPUT
![Screenshot 2024-12-07 214705](https://github.com/user-attachments/assets/846fc417-eda4-40f9-bf30-451426d65225)
![Screenshot 2024-12-07 214723](https://github.com/user-attachments/assets/f52ea0e1-73f0-49b3-8119-a7b88a791653)
![Screenshot 2024-12-07 215031](https://github.com/user-attachments/assets/0710a16e-cba5-4e37-9462-051e859a5f72)
![Screenshot 2024-12-07 215346](https://github.com/user-attachments/assets/90253194-8838-452b-8418-ea8e1055a422)
![image](https://github.com/user-attachments/assets/48bd983c-3e3d-4ff0-a3b0-149fe5dcad98)


# RESULT
The program for implementing image maps using HTML is executed successfully.
