# Ex.06 Book Front Cover Page Design
## Date:14/05/2025

## AIM:
To design a book front cover page using HTML and CSS.

## DESIGN STEPS:

### Step 1:
Create a Django Admin project.

### Step 2:
Create an app in the Django interface.

### Step 3:
Create a folder named 'static' in the app folder.

### Step 4:
Create a new HTML file in the static folder.

### Step 5:
Write the HTML code with relevant CSS properties.

### Step 6:
Choose the appropriate style and color scheme.

### Step 7:
Insert the images in their appropriate places.

### Step 8:
Publish the website in the LocalHost.

## PROGRAM:
   ```
   <!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <title>Harry Potter - Book Cover</title>

  <!-- Optional: Fancy serif font -->
  <link href="https://fonts.googleapis.com/css2?family=IM+Fell+English+SC&display=swap" rel="stylesheet">

  <style>
    * {
      margin: 0;
      padding: 0;
      box-sizing: border-box;
    }

    body {
      background: #121212;
      display: flex;
      justify-content: center;
      align-items: center;
      height: 100vh;
      font-family: 'IM Fell English SC', serif;
    }

    .book-cover {
      position: relative;
      width: 360px;
      height: 560px;
      background: linear-gradient(to bottom, #0f0f1a, #1c1c2e);
      border: 4px solid gold;
      border-radius: 10px;
      box-shadow: 0 0 30px rgba(255, 215, 0, 0.3);
      overflow: hidden;
      color: #f5c518;
    }

    .magic-orb {
      position: absolute;
      top: 20%;
      left: 50%;
      transform: translateX(-50%);
      width: 60px;
      height: 60px;
      background: radial-gradient(circle, rgba(255,215,0,0.8), transparent 70%);
      border-radius: 50%;
      box-shadow: 0 0 60px 20px rgba(255, 215, 0, 0.4);
      animation: pulse 2s infinite ease-in-out;
    }

    @keyframes pulse {
      0% {
        transform: translateX(-50%) scale(1);
        opacity: 1;
      }
      100% {
        transform: translateX(-50%) scale(1.3);
        opacity: 0.5;
      }
    }

    .book-content {
      position: relative;
      text-align: center;
      padding: 100px 20px 40px;
      z-index: 2;
    }

    .book-title {
      font-size: 2.8rem;
      letter-spacing: 2px;
      text-shadow: 1px 1px 5px #000;
    }

    .book-subtitle {
      margin-top: 15px;
      font-size: 1.2rem;
      font-style: italic;
      color: #ffd700;
    }

    .author {
      margin-top: 40px;
      font-size: 1rem;
      color: #ffdd55;
    }

    .photo {
      width: 100px;
      height: 100px;
      border-radius: 50%;
      border: 3px solid gold;
      object-fit: cover;
      position: absolute;
      bottom: 10px;
      right: 10px;
      box-shadow: 0 0 20px rgba(255, 215, 0, 0.5);
      z-index: 1;
    }
  </style>
</head>
<body>
  <div class="book-cover">
    <div class="magic-orb"></div>

    <div class="book-content">
      <h1 class="book-title">Harry Potter</h1>
      <h2 class="book-subtitle">and the Sorcerer's Stone</h2>
      <p class="author">by J.K. Rowling</p>
    </div>

    <!-- Photo now at bottom right -->
    <img src="mypic.jpg" alt="Your Photo" class="photo" />
  </div>
</body>
</html>
```

## OUTPUT:
![alt text](<Screenshot (1).png>)

## RESULT:
The program for designing book front cover page using HTML and CSS is completed successfully.
