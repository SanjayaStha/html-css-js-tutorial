Absolutely! Here are **some CSS practice examples with HTML-only code**, progressing from basic to more advanced concepts. Each snippet can be run directly in your browser.

---

## 🔹 **1. Basic Text Styling**
```html
<!DOCTYPE html>
<html>
<head>
  <style>
    h1 {
      color: darkblue;
      text-align: center;
      font-family: Arial, sans-serif;
    }

    p {
      font-size: 16px;
      line-height: 1.6;
      color: #333;
    }
  </style>
</head>
<body>
  <h1>Welcome to CSS World</h1>
  <p>This is a basic example of how CSS can style your text and align it beautifully.</p>
</body>
</html>
```

---

## 🔹 **2. Box Model Practice**
```html
<!DOCTYPE html>
<html>
<head>
  <style>
    .box {
      width: 300px;
      padding: 20px;
      margin: 30px auto;
      border: 3px solid #ff6347;
      background-color: #f9f9f9;
      box-sizing: border-box;
    }
  </style>
</head>
<body>
  <div class="box">
    <p>This box shows how padding, margin, and border work in the box model.</p>
  </div>
</body>
</html>
```

---

## 🔹 **3. Flexbox Layout**
```html
<!DOCTYPE html>
<html>
<head>
  <style>
    .container {
      display: flex;
      justify-content: space-around;
      background-color: #eee;
      padding: 20px;
    }

    .item {
      background-color: #4caf50;
      padding: 30px;
      color: white;
      font-weight: bold;
    }
  </style>
</head>
<body>
  <div class="container">
    <div class="item">Box 1</div>
    <div class="item">Box 2</div>
    <div class="item">Box 3</div>
  </div>
</body>
</html>
```

---

## 🔹 **4. Grid Layout**
```html
<!DOCTYPE html>
<html>
<head>
  <style>
    .grid-container {
      display: grid;
      grid-template-columns: repeat(3, 1fr);
      gap: 15px;
      padding: 20px;
    }

    .grid-item {
      background-color: #2196f3;
      color: white;
      padding: 20px;
      text-align: center;
    }
  </style>
</head>
<body>
  <div class="grid-container">
    <div class="grid-item">1</div>
    <div class="grid-item">2</div>
    <div class="grid-item">3</div>
    <div class="grid-item">4</div>
    <div class="grid-item">5</div>
    <div class="grid-item">6</div>
  </div>
</body>
</html>
```

---

## 🔹 **5. Hover Effect with Transition**
```html
<!DOCTYPE html>
<html>
<head>
  <style>
    .button {
      background-color: #008cba;
      color: white;
      padding: 15px 25px;
      text-align: center;
      display: inline-block;
      font-size: 16px;
      border: none;
      transition: background-color 0.3s;
    }

    .button:hover {
      background-color: #005f73;
    }
  </style>
</head>
<body>
  <button class="button">Hover Me</button>
</body>
</html>
```

---

## 🔹 **6. Responsive Card with Media Query**
```html
<!DOCTYPE html>
<html>
<head>
  <style>
    .card {
      width: 90%;
      max-width: 400px;
      margin: 20px auto;
      padding: 20px;
      border: 1px solid #ccc;
      background-color: #fff;
      text-align: center;
    }

    @media (min-width: 600px) {
      .card {
        background-color: #e0f7fa;
      }
    }
  </style>
</head>
<body>
  <div class="card">
    <h2>Responsive Card</h2>
    <p>Resize the browser to see background color change.</p>
  </div>
</body>
</html>
```

---

Would you like:
- More practice examples for specific topics like **navigation bar**, **login form UI**, or **animations**?
- Or a **zip file with all examples**?

Let me know how you'd like to use or share these!