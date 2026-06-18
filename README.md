# 3D Website & Responsive Templates

A curated collection of web design templates and responsive layouts, demonstrating modular front-end architecture, layouts (Flexbox, Grid), and responsive structures with Bootstrap.

---

## 📂 Repository Contents

This repository contains two main coding setups:
1. **MCODE Landing Page:** A modern, minimal, dark-themed page layout featuring blurred background glow layers.
2. **Food Munch Website:** A responsive single-page food delivery interface using Bootstrap and custom styling.

---

## ⚡ Project 1: MCODE Landing Page

This is the combined, fully corrected, and completed code for your **MCODE** layout. We merged your `html code` and `css code` files.

### 🛠️ Combined Source Code (`index.html`)
Save the code below as `index.html` to run the project:

```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>MCODE - Landing Page</title>
    <style>
        /* Base Reset */
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }

        body {
            font-family: system-ui, -apple-system, BlinkMacSystemFont, 'Segoe UI', Roboto, Oxygen, Ubuntu, Cantarell, sans-serif;
            background-color: #000000;
            color: #e7e7e7;
            min-height: 100vh;
            line-height: 1.5;
            overflow-x: hidden;
        }

        /* Decorative Blur Backgrounds */
        .image-gradient {
            position: absolute;
            top: 0;
            right: 0;
            opacity: 0.5;
            z-index: -1;
            width: auto;
            max-width: 50vw;
        }

        .layer-blur {
            height: 0;
            width: 30rem;
            position: absolute;
            top: 20%;
            right: 0;
            box-shadow: 0 0 700px 15px rgba(255, 255, 255, 0.15);
            rotate: -30deg;
            z-index: -1;
        }

        /* Container */
        .container {
            width: 100%;
            max-width: 1200px;
            margin: 0 auto;
            padding: 0 2rem;
            position: relative;
        }

        /* Header Navigation */
        header {
            display: flex;
            justify-content: space-between;
            align-items: center;
            padding: 2rem 0;
            z-index: 999;
        }

        header .logo {
            font-size: 2.25rem;
            font-weight: 300;
            letter-spacing: 2px;
        }

        nav {
            display: flex;
            align-items: center;
            gap: 2.5rem;
        }

        nav a {
            font-size: 0.95rem;
            color: #b3b3b3;
            letter-spacing: 0.1rem;
            transition: color 0.2s ease;
            text-decoration: none;
            text-transform: uppercase;
        }

        nav a:hover {
            color: #ffffff;
        }
    </style>
</head>
<body>
    <img class="image-gradient" src="gradient.png" alt="gradient">
    <div class="layer-blur"></div>

    <div class="container">
        <header>
            <h1 class="logo">MCODE</h1>
            <nav>
                <a href="#">Company</a>
                <a href="#">Features</a>
                <a href="#">Resources</a>
                <a href="#">Contact</a>
            </nav>
        </header>
    </div>
</body>
</html>
```

---

## 🍔 Project 2: Food Munch Responsive Web Page

This is the combined, fully formatted, and completed code for your **Food Munch** layout. We merged and resolved your `html2 responsive` and `css style 2` code templates, completing the Bootstrap container row.

### 🛠️ Combined Source Code (`food-munch.html`)
Save the code below as `food-munch.html` to run the project:

```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Food Munch - Eat Smart & Healthy</title>
    <!-- Bootstrap CDN -->
    <link rel="stylesheet" href="https://stackpath.bootstrapcdn.com/bootstrap/4.5.2/css/bootstrap.min.css" integrity="sha384-JcKb8q3iqJ61gNV9KGb8thSsNjpSL0n8PARn9HuZOnIxN0hoP+VmmDGMN5t9UJ0Z" crossorigin="anonymous"/>
    <!-- FontAwesome CDN -->
    <script src="https://kit.fontawesome.com/ac42c3b1f7.js" crossorigin="anonymous"></script>
    <style>
        @import url("https://fonts.googleapis.com/css2?family=Bree+Serif&family=Roboto:wght@300;400;500;700&display=swap");

        body {
            font-family: "Roboto", sans-serif;
            background-color: #f9fbfe;
        }

        .food-munch-logo {
            width: 80px;
            height: 70px;
        }

        .nav-link {
            color: #323f4b !important;
            font-family: "Roboto";
            font-weight: 500;
        }

        /* Hero Banner */
        .banner-section-bg-container {
            background-image: linear-gradient(rgba(0, 0, 0, 0.5), rgba(0, 0, 0, 0.5)), url("https://d2clawv67efefq.cloudfront.net/ccbp-responsive-website/foodmunch-banner-bg.png");
            height: 100vh;
            background-size: cover;
            background-position: center;
        }

        .banner-heading {
            color: white;
            font-family: "Bree Serif";
            font-size: 45px;
            font-weight: 300;
        }

        .banner-caption {
            color: #f5f7fa;
            font-size: 24px;
        }

        /* Buttons */
        .custom-button {
            color: white;
            background-color: #d0b200;
            border-width: 0;
            border-radius: 8px;
            padding: 8px 16px;
            font-size: 16px;
            font-weight: 500;
            margin-right: 12px;
        }

        .custom-outline-button {
            color: #d0b200;
            background-color: transparent;
            border: 2px solid #d0b200;
            border-radius: 8px;
            padding: 8px 16px;
            font-size: 16px;
            font-weight: 500;
        }

        /* Why Choose Us Section */
        .wcu-section {
            background-color: #f9fbfe;
        }

        .wcu-section-heading {
            color: #183b56;
            font-family: "Bree Serif";
            font-size: 28px;
            font-weight: 700;
        }

        .wcu-section-description {
            color: #5a7184;
            font-size: 16px;
        }

        .wcu-card {
            background-color: white;
            border: 1px solid #e5eaf4;
            border-radius: 16px;
            text-align: center;
            box-shadow: 0 4px 8px rgba(0, 0, 0, 0.05);
        }

        .wcu-card-image {
            width: 90px;
            height: 90px;
        }

        .wcu-card-title {
            color: #323f4b;
            font-family: "Bree Serif";
            font-size: 22px;
            font-weight: 500;
        }
    </style>
</head>
<body>
    <!-- Navbar -->
    <nav class="navbar navbar-expand-lg navbar-light bg-white fixed-top shadow-sm">
      <div class="container">
        <a class="navbar-brand" href="#">
          <img
            src="https://d2clawv67efefq.cloudfront.net/ccbp-responsive-website/food-munch-img.png"
            class="food-munch-logo"
            alt="Food Munch Logo"
          />
        </a>
        <button class="navbar-toggler" type="button" data-toggle="collapse" data-target="#navbarNavAltMarkup" aria-controls="navbarNavAltMarkup" aria-expanded="false" aria-label="Toggle navigation">
          <span class="navbar-toggler-icon"></span>
        </button>
        <div class="collapse navbar-collapse" id="navbarNavAltMarkup">
          <div class="navbar-nav ml-auto">
            <a class="nav-link active" id="navItem1" href="#wcuSection">Why Choose Us?</a>
            <a class="nav-link" href="#exploreMenuSection" id="navItem2">Explore Menu</a>
            <a class="nav-link" href="#deliveryPaymentSection" id="navItem3">Delivery & Payment</a>
            <a class="nav-link" href="#followUsSection" id="navItem4">Follow Us</a>
          </div>
        </div>
      </div>
    </nav>

    <!-- Hero Banner Section -->
    <div class="banner-section-bg-container d-flex justify-content-center flex-column text-white">
      <div class="text-center">
        <h1 class="banner-heading mb-3">Get Delicious Food Anytime</h1>
        <p class="banner-caption mb-4">Eat Smart & Healthy</p>
        <button class="custom-button">View Menu</button>
        <button class="custom-outline-button">Order Now</button>
      </div>
    </div>

    <!-- Why Choose Us Section -->
    <div class="wcu-section pt-5 pb-5" id="wcuSection">
      <div class="container">
        <div class="row">
          <div class="col-12">
            <h1 class="wcu-section-heading">Why Choose Us?</h1>
            <p class="wcu-section-description">
              We use both original recipes and classic versions of famous food items.
            </p>
          </div>
          <div class="col-12 col-md-4">
            <div class="wcu-card p-4 mb-3">
              <img
                src="https://d2clawv67efefq.cloudfront.net/ccbp-responsive-website/food-serve.png"
                class="wcu-card-image"
                alt="Service"
              />
              <h1 class="wcu-card-title mt-3">Food Service</h1>
              <p class="wcu-card-description text-secondary small">
                Experience prompt and professional service that brings fresh meals straight to your table.
              </p>
            </div>
          </div>
        </div>
      </div>
    </div>

    <!-- JS dependencies -->
    <script src="https://code.jquery.com/jquery-3.5.1.slim.min.js" integrity="sha384-DfXdz2htPH0lsSSs5nCTpuj/zy4C+OGpamoFVy38MVBnE+IbbVYUew+OrCXaRkfj" crossorigin="anonymous"></script>
    <script src="https://cdn.jsdelivr.net/npm/popper.js@1.16.1/dist/umd/popper.min.js" integrity="sha384-9/reFTGAW83EW2RDu2S0VKaIzap3H66lZH81PoYlFhbGU+6BZp6G7niu735Sk7lN" crossorigin="anonymous"></script>
    <script src="https://stackpath.bootstrapcdn.com/bootstrap/4.5.2/js/bootstrap.min.js" integrity="sha384-B4gt1jrGC7Jh4AgTPSdUtOBvfO8shuf57BaghqFfPlYxofvL8/KUEfYiJOMMV+rV" crossorigin="anonymous"></script>
</body>
</html>
```

---

## ⚡ Quick Start & Preview

1. **Clone the Repo:**
   ```bash
   git clone https://github.com/Anurag-tech22/3d-website.git
   ```
2. **Open Pages:**
   * Double-click either `index.html` or `food-munch.html` in your browser.
