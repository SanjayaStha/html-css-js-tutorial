Here’s a **detailed lesson plan** for your **6-hour HTML5 class**, covering all fundamental and advanced concepts with explanations, examples, and hands-on projects.

---

# **HTML5 Full Lesson Plan (6 Hours)**  

## **Hour 1: Introduction to HTML5**  
### **1.1 What is HTML5?**  
HTML5 is the latest version of HTML (HyperText Markup Language) used to create web pages. It introduces new elements, attributes, and APIs to make web development easier and more efficient.

### **1.2 Basic Structure of an HTML5 Document**  
Every HTML5 document starts with a `<!DOCTYPE html>` declaration, which tells the browser that the document is written in HTML5.

📌 **Example:**  
```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>My First HTML5 Page</title>
</head>
<body>
    <h1>Welcome to HTML5</h1>
    <p>This is a simple paragraph.</p>
</body>
</html>
```

### **1.3 Important HTML5 Tags and Attributes**  
- `<html>`: The root element of the HTML document.  
- `<head>`: Contains metadata like title, styles, and scripts.  
- `<meta charset="UTF-8">`: Specifies character encoding for better language support.  
- `<body>`: Contains all the visible content of the page.  

📌 **Project:** **Create a Simple Personal Webpage** (Profile with a heading, paragraph, and an image).  

---

## **Hour 2: Semantic Elements and Page Structure**  
### **2.1 What Are Semantic Elements?**  
Semantic elements clearly define the meaning of content in a web page. Instead of using generic `<div>` tags, HTML5 introduced specific elements for better readability and SEO.

📌 **Common Semantic Elements:**  
| Tag       | Description |
|-----------|-------------|
| `<header>` | Represents introductory content like a page title or logo |
| `<nav>`    | Contains navigation links |
| `<section>` | Groups related content |
| `<article>` | Represents self-contained content like a blog post |
| `<aside>` | Defines side content, like a sidebar |
| `<footer>` | Represents footer content, like copyright or links |

📌 **Example:**  
```html
<header>
    <h1>My Blog</h1>
</header>
<nav>
    <ul>
        <li><a href="#">Home</a></li>
        <li><a href="#">About</a></li>
        <li><a href="#">Contact</a></li>
    </ul>
</nav>
<section>
    <article>
        <h2>First Blog Post</h2>
        <p>This is an example of an article inside a section.</p>
    </article>
</section>
<footer>
    <p>© 2025 My Blog</p>
</footer>
```

📌 **Project:** **Build a Blog Homepage Layout** (Using `<header>`, `<nav>`, `<section>`, `<article>`, and `<footer>`).  

---

## **Hour 3: HTML5 Forms and Input Elements**  
### **3.1 Forms and Input Types**  
Forms are used to collect user input, and HTML5 introduces new input types.

📌 **Common Input Types:**  
| Input Type | Description |
|------------|-------------|
| `text` | Standard text input |
| `email` | Email input with validation |
| `url` | URL input with validation |
| `tel` | Phone number input |
| `date` | Date picker |
| `number` | Numeric input |
| `range` | Slider input |

📌 **Example:**  
```html
<form action="submit.html" method="post">
    <label for="name">Name:</label>
    <input type="text" id="name" name="name" required><br>

    <label for="email">Email:</label>
    <input type="email" id="email" name="email" required><br>

    <label for="dob">Date of Birth:</label>
    <input type="date" id="dob" name="dob"><br>

    <input type="submit" value="Submit">
</form>
```

📌 **Project:** **Create a Registration Form** (Using input validation and new form elements).  

---

## **Hour 4: Media Elements (Audio & Video)**  
### **4.1 Adding Audio and Video to Web Pages**  
HTML5 allows embedding multimedia using `<audio>` and `<video>` elements.

📌 **Example - Video:**  
```html
<video width="400" controls>
    <source src="video.mp4" type="video/mp4">
    Your browser does not support the video tag.
</video>
```

📌 **Example - Audio:**  
```html
<audio controls>
    <source src="audio.mp3" type="audio/mpeg">
    Your browser does not support the audio tag.
</audio>
```

📌 **Project:** **Create a Podcast Website** (Embed audio playlist with episodes).  

---

## **Hour 5: HTML5 Graphics - Canvas & SVG**  
### **5.1 Drawing with the `<canvas>` Element**  
The `<canvas>` element allows drawing shapes and graphics dynamically using JavaScript.

📌 **Example - Drawing a Rectangle on Canvas:**  
```html
<canvas id="myCanvas" width="200" height="100" style="border:1px solid #000;"></canvas>
<script>
    var canvas = document.getElementById("myCanvas");
    var ctx = canvas.getContext("2d");
    ctx.fillStyle = "blue";
    ctx.fillRect(20, 20, 150, 80);
</script>
```

📌 **Project:** **Create an Interactive Drawing App** (Users can draw on a canvas).  

---

## **Hour 6: HTML5 APIs - Geolocation & Local Storage**  
### **6.1 Geolocation API**  
The Geolocation API fetches the user’s current location.

📌 **Example:**  
```html
<button onclick="getLocation()">Get My Location</button>
<p id="location"></p>

<script>
    function getLocation() {
        if (navigator.geolocation) {
            navigator.geolocation.getCurrentPosition(showPosition);
        } else {
            document.getElementById("location").innerHTML = "Geolocation not supported.";
        }
    }
    function showPosition(position) {
        document.getElementById("location").innerHTML =
            "Latitude: " + position.coords.latitude +
            "<br>Longitude: " + position.coords.longitude;
    }
</script>
```

### **6.2 Local Storage API**  
Stores data on the user's browser.

📌 **Example:**  
```html
<input type="text" id="name" placeholder="Enter name">
<button onclick="saveName()">Save Name</button>
<p id="savedName"></p>

<script>
    function saveName() {
        let name = document.getElementById("name").value;
        localStorage.setItem("username", name);
        document.getElementById("savedName").innerText = "Saved: " + name;
    }
</script>
```

📌 **Project:** **Create a Location-Based App** (Show user’s location and save preferences using Local Storage).  

---

## **Final Mini Project:** **Build a Portfolio Website**  
Combine all elements learned in the class:  
✅ **Semantic layout**  
✅ **Forms**  
✅ **Multimedia (audio/video)**  
✅ **Canvas graphics**  
✅ **Geolocation and Local Storage**  

Would you like slides or extra exercises for students? 🚀