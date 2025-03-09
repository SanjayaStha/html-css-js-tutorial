### **CSS Basics Course Content with In-Depth Examples**

This course will cover the fundamentals of **CSS (Cascading Style Sheets)**, its types, imports, and basic structure. You'll learn how to style webpages and apply design principles in a structured way.

---

## **1. Introduction to CSS**  

### **1.1 What is CSS?**  
CSS stands for Cascading Style Sheets and is used to control the layout and appearance of web pages. It allows you to add style to HTML elements, including colors, fonts, spacing, and positioning.

### **1.2 Why CSS?**  
CSS separates content (HTML) from presentation (design), which helps with maintenance, readability, and styling consistency across multiple pages.

---

## **2. Types of CSS**  

### **2.1 Inline CSS**  
Inline CSS is used to style individual HTML elements by adding the `style` attribute directly to the HTML tag.

📌 **Example:**  
```html
<p style="color: blue; font-size: 16px;">This is a blue colored paragraph with font size 16px.</p>
```

📝 **Pros:**  
- Quick and simple for small styling tasks.  
- Styles apply only to specific elements.  

📝 **Cons:**  
- Not scalable or maintainable for large projects.  
- Can make the HTML messy.

### **2.2 Internal CSS**  
Internal CSS is written within the `<style>` tag in the `<head>` section of the HTML document.

📌 **Example:**  
```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Internal CSS Example</title>
    <style>
        body {
            background-color: #f0f0f0;
            font-family: Arial, sans-serif;
        }
        h1 {
            color: darkblue;
        }
    </style>
</head>
<body>
    <h1>Welcome to My Website</h1>
    <p>This is an example of internal CSS styling.</p>
</body>
</html>
```

📝 **Pros:**  
- Easy to implement for single pages.  
- Useful for simple webpages.  

📝 **Cons:**  
- Cannot be reused across multiple pages.
- Increases page load time.

### **2.3 External CSS**  
External CSS is the most commonly used method for styling a website. The CSS is written in a separate file (usually with a `.css` extension), which is linked to the HTML document.

📌 **Example:**  
1. **HTML (index.html):**
```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>External CSS Example</title>
    <link rel="stylesheet" href="styles.css">
</head>
<body>
    <h1>Welcome to My Website</h1>
    <p>This webpage uses external CSS for styling.</p>
</body>
</html>
```

2. **CSS (styles.css):**
```css
body {
    background-color: #f0f0f0;
    font-family: Arial, sans-serif;
}

h1 {
    color: darkblue;
}
```

📝 **Pros:**  
- Allows styling of multiple pages with a single file.  
- Easy to maintain and modify.  
- Reduces HTML file size and increases page load efficiency.

📝 **Cons:**  
- Requires an additional HTTP request for the CSS file.

---

## **3. CSS Syntax and Structure**  

### **3.1 CSS Syntax**  
CSS syntax consists of a **selector**, **property**, and **value**.

📌 **Structure:**  
```css
selector {
    property: value;
}
```

📌 **Example:**  
```css
h1 {
    color: blue;
    font-size: 24px;
}
```

- **Selector**: Specifies the HTML element to style (e.g., `h1`).  
- **Property**: Defines the style property to modify (e.g., `color`, `font-size`).  
- **Value**: Specifies the value for the property (e.g., `blue`, `24px`).

---

### **3.2 CSS Selectors**  

#### **3.2.1 Universal Selector**  
The universal selector `*` targets all elements.

📌 **Example:**  
```css
* {
    margin: 0;
    padding: 0;
}
```

#### **3.2.2 Element Selector**  
Targets specific HTML tags, like `p`, `h1`, `div`, etc.

📌 **Example:**  
```css
p {
    color: green;
}
```

#### **3.2.3 Class Selector**  
The class selector targets elements with a specific class. Use the `.` before the class name.

📌 **Example:**  
```css
.button {
    background-color: blue;
    color: white;
}
```

#### **3.2.4 ID Selector**  
The ID selector targets an element with a specific `id`. Use the `#` before the ID name.

📌 **Example:**  
```css
#header {
    background-color: gray;
    color: white;
}
```

#### **3.2.5 Descendant Selector**  
Targets elements inside a parent element.

📌 **Example:**  
```css
nav ul li {
    display: inline;
}
```

---

### **3.3 CSS Properties and Values**

#### **3.3.1 Color and Background**  
- `color`: Sets the color of text.  
- `background-color`: Sets the background color.

📌 **Example:**  
```css
p {
    color: red;
    background-color: yellow;
}
```

#### **3.3.2 Text Styling**  
- `font-family`: Specifies the font of the text.  
- `font-size`: Specifies the size of the font.  
- `text-align`: Aligns the text (e.g., `left`, `center`, `right`).

📌 **Example:**  
```css
h1 {
    font-family: 'Arial', sans-serif;
    font-size: 32px;
    text-align: center;
}
```

#### **3.3.3 Margin and Padding**  
- `margin`: Adds space outside an element.  
- `padding`: Adds space inside an element.

📌 **Example:**  
```css
div {
    margin: 20px;
    padding: 10px;
    border: 1px solid black;
}
```

---

## **4. CSS Box Model**

### **4.1 What is the Box Model?**  
The CSS box model describes the rectangular boxes generated for elements, which consist of:
- **Content**: The actual content (e.g., text or image).
- **Padding**: Space around the content, inside the border.
- **Border**: Surrounds the padding (optional).
- **Margin**: Space outside the border.

### **4.2 Box Model Example:**

📌 **Example:**  
```css
div {
    width: 200px;
    height: 100px;
    padding: 20px;
    border: 5px solid black;
    margin: 30px;
}
```

---

## **5. CSS Import and Linking**

### **5.1 Using `@import` to Import CSS Files**  
The `@import` rule is used to import external stylesheets within an existing CSS file.

📌 **Example:**
```css
@import url('styles.css');
```

**Note:** Using `@import` might slow down page load times, so it’s recommended to use `<link>` in HTML for better performance.

---

## **6. CSS Responsive Design**

### **6.1 Media Queries**  
Media queries allow you to apply styles based on the device's characteristics, such as screen width.

📌 **Example:**
```css
@media screen and (max-width: 600px) {
    body {
        background-color: lightblue;
    }
    h1 {
        font-size: 20px;
    }
}
```

**Explanation:** The background color will change to light blue when the screen width is 600px or less.

---

## **Conclusion**

CSS is an essential skill for web development, allowing you to control the layout and appearance of websites. Understanding its basic structure, selectors, properties, and types will help you create visually appealing and responsive web pages.  

**Next Steps:**
- Practice using different CSS properties.
- Create small styling projects like buttons, layouts, or card designs.
- Explore more advanced CSS concepts like Flexbox and Grid.

Would you like me to create **practice exercises** or a **mini-project** to implement the concepts covered so far?