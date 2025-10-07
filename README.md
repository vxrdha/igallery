# Ex.08 Design of Interactive Image Gallery
## Date:

## AIM:
To design a web application for an inteactive image gallery with minimum five images.

## DESIGN STEPS:

### Step 1:
Clone the github repository and create Django admin interface.

### Step 2:
Change settings.py file to allow request from all hosts.

### Step 3:
Use CSS for positioning and styling.

### Step 4:
Write JavaScript program for implementing interactivity.

### Step 5:
Validate the HTML and CSS code.

### Step 6:
Publish the website in the given URL.

## PROGRAM :
```
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Interactive Image Gallery</title>
  <style>
    body {
      margin: 0;
      font-family: Arial, sans-serif;
      background: url('bg.jpg') no-repeat center center fixed;
      background-size: cover;
      color: white;
    }

    .gallery-container {
      display: grid;
      grid-template-columns: repeat(auto-fit, minmax(200px, 1fr));
      gap: 15px;
      padding: 40px;
      max-width: 1000px;
      margin: auto;
    }

    .gallery-item {
      overflow: hidden;
      border-radius: 15px;
      box-shadow: 0 4px 10px rgba(0,0,0,0.5);
      transition: transform 0.3s ease;
      cursor: pointer;
    }

    .gallery-item:hover {
      transform: scale(1.05);
    }

    .gallery-item img {
      width: 100%;
      height: 100%;
      object-fit: cover;
      display: block;
    }

    /* Lightbox */
    .lightbox {
      display: none;
      position: fixed;
      top: 0; left: 0;
      width: 100%;
      height: 100%;
      background: rgba(0,0,0,0.9);
      justify-content: center;
      align-items: center;
      z-index: 1000;
    }

    .lightbox img {
      max-width: 90%;
      max-height: 80%;
      border-radius: 10px;
      box-shadow: 0 0 20px rgba(255,255,255,0.3);
    }

    .lightbox:target {
      display: flex;
    }

    .close {
      position: absolute;
      top: 20px;
      right: 30px;
      font-size: 2em;
      color: white;
      text-decoration: none;
      font-weight: bold;
    }

    .close:hover {
      color: red;
    }
  </style>
</head>
<body>

  <h1 style="text-align:center; padding-top: 20px;">📸 Interactive Image Gallery</h1>

  <div class="gallery-container">
    <a href="#img1" class="gallery-item"><img src="img1.jpg" alt="Image 1"></a>
    <a href="#img2" class="gallery-item"><img src="img2.jpg" alt="Image 2"></a>
    <a href="#img3" class="gallery-item"><img src="img3.jpg" alt="Image 3"></a>
    <a href="#img4" class="gallery-item"><img src="img4.jpg" alt="Image 4"></a>
    <a href="#img5" class="gallery-item"><img src="img5.jpg" alt="Image 5"></a>
  </div>

  <!-- Lightbox Popups -->
  <div id="img1" class="lightbox">
    <a href="#" class="close">&times;</a>
    <img src="img1.jpg" alt="">
  </div>

  <div id="img2" class="lightbox">
    <a href="#" class="close">&times;</a>
    <img src="img2.jpg" alt="">
  </div>

  <div id="img3" class="lightbox">
    <a href="#" class="close">&times;</a>
    <img src="img3.jpg" alt="">
  </div>

  <div id="img4" class="lightbox">
    <a href="#" class="close">&times;</a>
    <img src="img4.jpg" alt="">
  </div>

  <div id="img5" class="lightbox">
    <a href="#" class="close">&times;</a>
    <img src="img5.jpg" alt="">
  </div>

</body>
</html>
```
## OUTPUT:

## RESULT:
The program for designing an interactive image gallery using HTML, CSS and JavaScript is executed successfully.
