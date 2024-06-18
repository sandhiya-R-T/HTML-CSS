# [Guvi Zen](https://www.guvi.io/zen/)

## HTML Task to know usage of basic tags.

1. Fix the bugs in below snippet

```HTML
    <html lang="en">
    <head>
        <title>Document
            <body>
                guvi
        </title>
    </head>
    <div>
        Lorem ipsum dolor sit amet consectetur adipisicing elit.
        <div>
            <div>
                Guvi Geek Network
            </div>
        </body>
    </html>
```
2. Try the below one

```HTML
<html lang="en">
    <head>
        <title>Document</title>
            <body>
                guvi
    </head>
    <div>
        Lorem ipsum dolor sit amet consectetur adipisicing elit.
        <div>
            <div>
                Guvi Geek Network
            </div>
        </body>
    </html>
```

---

3. Design a contact us form with all fields as required.

<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Contact Us</title>
<style>
    body {
        font-family: Arial, sans-serif;
        background-color: #f0f0f0;
        padding: 20px;
    }
    .container {
        max-width: 600px;
        margin: 0 auto;
        background: #fff;
        padding: 20px;
        border-radius: 8px;
        box-shadow: 0 0 10px rgba(0,0,0,0.1);
    }
    .form-group {
        margin-bottom: 20px;
    }
    .form-group label {
        display: block;
        font-weight: bold;
        margin-bottom: 5px;
    }
    .form-group input, .form-group textarea {
        width: 100%;
        padding: 10px;
        font-size: 16px;
        border: 1px solid #ccc;
        border-radius: 4px;
        box-sizing: border-box;
    }
    .form-group textarea {
        height: 120px;
    }
    .form-group input[type="submit"] {
        background-color: #4CAF50;
        color: white;
        border: none;
        cursor: pointer;
        padding: 12px 20px;
        border-radius: 4px;
        font-size: 16px;
    }
    .form-group input[type="submit"]:hover {
        background-color: #45a049;
    }
</style>
</head>
<body>

<div class="container">
    <h2>Contact Us</h2>
    <form action="#" method="post">
        <div class="form-group">
            <label for="name">Name:</label>
            <input type="text" id="name" name="name" required>
        </div>
        <div class="form-group">
            <label for="email">Email:</label>
            <input type="email" id="email" name="email" required>
        </div>
        <div class="form-group">
            <label for="phone">Phone:</label>
            <input type="tel" id="phone" name="phone" required>
        </div>
        <div class="form-group">
            <label for="message">Message:</label>
            <textarea id="message" name="message" required></textarea>
        </div>
        <div class="form-group">
            <input type="submit" value="Submit">
        </div>
    </form>
</div>

</body>
</html>

---

4. Use certain HTML elements to display the following in a HTML page.

- Programming Language
  - JavaScript
    1. Angular
    2. React
    3. Vue.js
  - Python
    1. Django Framework
    2. Flask Framework
  - Java
    1. Spring
    2. Maven
    3. Hibernate
- Database
  - MySQL
  - MongoDB
  - Cansandra

<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Programming Languages and Databases</title>
<style>
    body {
        font-family: Arial, sans-serif;
        padding: 20px;
    }
    h2 {
        margin-bottom: 10px;
    }
    ul {
        list-style-type: none;
        padding-left: 20px;
    }
    li {
        margin-bottom: 5px;
    }
</style>
</head>
<body>

<h2>Programming Languages</h2>
<ul>
    <li>
        <strong>JavaScript</strong>
        <ul>
            <li>Angular</li>
            <li>React</li>
            <li>Vue.js</li>
        </ul>
    </li>
    <li>
        <strong>Python</strong>
        <ul>
            <li>Django Framework</li>
            <li>Flask Framework</li>
        </ul>
    </li>
    <li>
        <strong>Java</strong>
        <ul>
            <li>Spring</li>
            <li>Maven</li>
            <li>Hibernate</li>
        </ul>
    </li>
</ul>

<h2>Database</h2>
<ul>
    <li>MySQL</li>
    <li>MongoDB</li>
    <li>Cassandra</li>
</ul>

</body>
</html>

---

5. Create an element that helps you to open the https://google.com in separate new tab.

<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Open Google in New Tab</title>
</head>
<body>

<p>Click the link below to open Google in a new tab:</p>

<a href="https://google.com" target="_blank">Open Google</a>

</body>
</html>

---

6. In the form, add two radio buttons with grouping them for employee type(Salaried and own business)

<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Contact Us</title>
<style>
    body {
        font-family: Arial, sans-serif;
        background-color: #f0f0f0;
        padding: 20px;
    }
    .container {
        max-width: 600px;
        margin: 0 auto;
        background: #fff;
        padding: 20px;
        border-radius: 8px;
        box-shadow: 0 0 10px rgba(0,0,0,0.1);
    }
    .form-group {
        margin-bottom: 20px;
    }
    .form-group label {
        display: block;
        font-weight: bold;
        margin-bottom: 5px;
    }
    .form-group input, .form-group textarea {
        width: 100%;
        padding: 10px;
        font-size: 16px;
        border: 1px solid #ccc;
        border-radius: 4px;
        box-sizing: border-box;
    }
    .form-group textarea {
        height: 120px;
    }
    .form-group input[type="submit"] {
        background-color: #4CAF50;
        color: white;
        border: none;
        cursor: pointer;
        padding: 12px 20px;
        border-radius: 4px;
        font-size: 16px;
    }
    .form-group input[type="submit"]:hover {
        background-color: #45a049;
    }
</style>
</head>
<body>

<div class="container">
    <h2>Contact Us</h2>
    <form action="#" method="post">
        <div class="form-group">
            <label for="name">Name:</label>
            <input type="text" id="name" name="name" required>
        </div>
        <div class="form-group">
            <label for="email">Email:</label>
            <input type="email" id="email" name="email" required>
        </div>
        <div class="form-group">
            <label for="phone">Phone:</label>
            <input type="tel" id="phone" name="phone" required>
        </div>
        <div class="form-group">
            <label>Employee Type:</label>
            <div>
                <input type="radio" id="salaried" name="employee_type" value="Salaried" required>
                <label for="salaried">Salaried</label>
            </div>
            <div>
                <input type="radio" id="business_owner" name="employee_type" value="Own Business" required>
                <label for="business_owner">Own Business</label>
            </div>
        </div>
        <div class="form-group">
            <label for="message">Message:</label>
            <textarea id="message" name="message" required></textarea>
        </div>
        <div class="form-group">
            <input type="submit" value="Submit">
        </div>
    </form>
</div>

</body>
</html>

---

7. Design form shown in the link (http://evc-cit.info/cit040/formguide/card_0.png)

<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Contact Information Form</title>
<style>
    body {
        font-family: Arial, sans-serif;
        background-color: #f0f0f0;
        padding: 20px;
    }
    .container {
        max-width: 600px;
        margin: 0 auto;
        background: #fff;
        padding: 20px;
        border-radius: 8px;
        box-shadow: 0 0 10px rgba(0,0,0,0.1);
    }
    .form-group {
        margin-bottom: 15px;
    }
    .form-group label {
        display: block;
        font-weight: bold;
        margin-bottom: 5px;
    }
    .form-group input[type="text"],
    .form-group input[type="email"],
    .form-group input[type="tel"] {
        width: calc(100% - 20px);
        padding: 10px;
        font-size: 16px;
        border: 1px solid #ccc;
        border-radius: 4px;
        box-sizing: border-box;
    }
    .form-group input[type="radio"] {
        margin-right: 10px;
    }
    .form-group textarea {
        width: calc(100% - 20px);
        padding: 10px;
        font-size: 16px;
        border: 1px solid #ccc;
        border-radius: 4px;
        box-sizing: border-box;
        resize: vertical;
    }
    .form-group input[type="submit"] {
        background-color: #4CAF50;
        color: white;
        border: none;
        cursor: pointer;
        padding: 12px 20px;
        border-radius: 4px;
        font-size: 16px;
    }
    .form-group input[type="submit"]:hover {
        background-color: #45a049;
    }
</style>
</head>
<body>

<div class="container">
    <h2>Contact Information</h2>
    <form action="#" method="post">
        <div class="form-group">
            <label for="name">Name:</label>
            <input type="text" id="name" name="name" required>
        </div>
        <div class="form-group">
            <label for="address">Address:</label>
            <input type="text" id="address" name="address" required>
        </div>
        <div class="form-group">
            <label for="city">City:</label>
            <input type="text" id="city" name="city" required>
        </div>
        <div class="form-group">
            <label for="state">State:</label>
            <input type="text" id="state" name="state" required>
        </div>
        <div class="form-group">
            <label for="zip">Zip Code:</label>
            <input type="text" id="zip" name="zip" required>
        </div>
        <div class="form-group">
            <label for="email">Email:</label>
            <input type="email" id="email" name="email" required>
        </div>
        <div class="form-group">
            <label for="phone">Phone:</label>
            <input type="tel" id="phone" name="phone" required>
        </div>
        <div class="form-group">
            <label for="gender">Gender:</label>
            <input type="radio" id="male" name="gender" value="male" required>
            <label for="male">Male</label>
            <input type="radio" id="female" name="gender" value="female" required>
            <label for="female">Female</label>
        </div>
        <div class="form-group">
            <label for="comments">Comments:</label>
            <textarea id="comments" name="comments" rows="5" required></textarea>
        </div>
        <div class="form-group">
            <input type="submit" value="Submit">
        </div>
    </form>
</div>

</body>
</html>

---

8. Use the table tag to design given image [Click here](https://www.bapugraphics.com/assets/img/port_upload_dir/table-4.jpg).

<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Product Details</title>
<style>
    body {
        font-family: Arial, sans-serif;
        background-color: #f0f0f0;
        padding: 20px;
    }
    table {
        width: 100%;
        border-collapse: collapse;
        margin-bottom: 20px;
    }
    th, td {
        border: 1px solid #ddd;
        padding: 8px;
        text-align: left;
    }
    th {
        background-color: #f2f2f2;
    }
    tr:nth-child(even) {
        background-color: #f9f9f9;
    }
</style>
</head>
<body>

<h2>Product Details</h2>

<table>
    <thead>
        <tr>
            <th>Product ID</th>
            <th>Product Name</th>
            <th>Price</th>
            <th>Discount</th>
            <th>Availability</th>
        </tr>
    </thead>
    <tbody>
        <tr>
            <td>P001</td>
            <td>Keyboard</td>
            <td>$50</td>
            <td>10%</td>
            <td>In Stock</td>
        </tr>
        <tr>
            <td>P002</td>
            <td>Mouse</td>
            <td>$20</td>
            <td>5%</td>
            <td>In Stock</td>
        </tr>
        <tr>
            <td>P003</td>
            <td>Monitor</td>
            <td>$200</td>
            <td>15%</td>
            <td>Out of Stock</td>
        </tr>
        <tr>
            <td>P004</td>
            <td>Headphones</td>
            <td>$30</td>
            <td>7%</td>
            <td>In Stock</td>
        </tr>
    </tbody>
</table>

</body>
</html>

---

9. Write HTML input tags snippet to show default values for all Form elements.

<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Default Values for Form Elements</title>
</head>
<body>

<form action="#" method="post">
    <label for="name">Name:</label>
    <input type="text" id="name" name="name" value="John Doe"><br><br>
    
    <label for="email">Email:</label>
    <input type="email" id="email" name="email" value="johndoe@example.com"><br><br>
    
    <label for="phone">Phone:</label>
    <input type="tel" id="phone" name="phone" value="+1234567890"><br><br>
    
    <label for="birthdate">Birthdate:</label>
    <input type="date" id="birthdate" name="birthdate" value="2000-01-01"><br><br>
    
    <label for="gender">Gender:</label>
    <input type="radio" id="male" name="gender" value="male" checked>
    <label for="male">Male</label>
    <input type="radio" id="female" name="gender" value="female">
    <label for="female">Female</label><br><br>
    
    <label for="country">Country:</label>
    <select id="country" name="country">
        <option value="usa">USA</option>
        <option value="uk" selected>UK</option>
        <option value="canada">Canada</option>
    </select><br><br>
    
    <label for="message">Message:</label><br>
    <textarea id="message" name="message" rows="4" cols="50">Default message...</textarea><br><br>
    
    <input type="checkbox" id="subscribe" name="subscribe" checked>
    <label for="subscribe">Subscribe to newsletter</label><br><br>
    
    <input type="submit" value="Submit">
</form>

</body>
</html>

---

10. In your, HTML page add the below line and Highlight it without using any CSS.

- "HTML & CSS is awesome"

<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Highlight Text</title>
</head>
<body>

<p>HTML &amp; CSS is <mark>awesome</mark>.</p>

</body>
</html>

---

11. Create an HTML page, which should contain all types of input elements.
    <!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>All Types of Input Elements</title>
<style>
    body {
        font-family: Arial, sans-serif;
        padding: 20px;
    }
    .input-container {
        margin-bottom: 20px;
    }
    label {
        display: block;
        font-weight: bold;
        margin-bottom: 5px;
    }
    input[type="text"],
    input[type="email"],
    input[type="tel"],
    input[type="date"],
    textarea {
        width: calc(100% - 20px);
        padding: 10px;
        font-size: 16px;
        border: 1px solid #ccc;
        border-radius: 4px;
        box-sizing: border-box;
        margin-top: 5px;
    }
    select {
        width: calc(100% - 22px);
        padding: 10px;
        font-size: 16px;
        border: 1px solid #ccc;
        border-radius: 4px;
        box-sizing: border-box;
        margin-top: 5px;
    }
    input[type="checkbox"],
    input[type="radio"] {
        margin-right: 10px;
    }
</style>
</head>
<body>

<div class="input-container">
    <label for="text">Text Input:</label>
    <input type="text" id="text" name="text" placeholder="Enter text...">
</div>

<div class="input-container">
    <label for="email">Email Input:</label>
    <input type="email" id="email" name="email" placeholder="Enter email...">
</div>

<div class="input-container">
    <label for="tel">Telephone Input:</label>
    <input type="tel" id="tel" name="tel" placeholder="Enter telephone number...">
</div>

<div class="input-container">
    <label for="date">Date Input:</label>
    <input type="date" id="date" name="date">
</div>

<div class="input-container">
    <label for="textarea">Textarea:</label>
    <textarea id="textarea" name="textarea" rows="4" placeholder="Enter text..."></textarea>
</div>

<div class="input-container">
    <label for="checkbox">Checkbox:</label>
    <input type="checkbox" id="checkbox1" name="checkbox1" value="checkbox1">
    <label for="checkbox1">Option 1</label><br>
    <input type="checkbox" id="checkbox2" name="checkbox2" value="checkbox2">
    <label for="checkbox2">Option 2</label>
</div>

<div class="input-container">
    <label for="radio">Radio Buttons:</label><br>
    <input type="radio" id="radio1" name="radio" value="radio1">
    <label for="radio1">Option 1</label><br>
    <input type="radio" id="radio2" name="radio" value="radio2">
    <label for="radio2">Option 2</label><br>
    <input type="radio" id="radio3" name="radio" value="radio3">
    <label for="radio3">Option 3</label>
</div>

<div class="input-container">
    <label for="select">Select Dropdown:</label>
    <select id="select" name="select">
        <option value="option1">Option 1</option>
        <option value="option2">Option 2</option>
        <option value="option3">Option 3</option>
    </select>
</div>

<div class="input-container">
    <label for="file">File Upload:</label>
    <input type="file" id="file" name="file">
</div>

<div class="input-container">
    <label for="color">Color Picker:</label>
    <input type="color" id="color" name="color">
</div>

<div class="input-container">
    <label for="range">Range Slider:</label>
    <input type="range" id="range" name="range" min="0" max="100" value="50">
</div>

<div class="input-container">
    <label for="number">Number Input:</label>
    <input type="number" id="number" name="number" min="0" max="100" step="1" value="50">
</div>

<div class="input-container">
    <label for="search">Search Input:</label>
    <input type="search" id="search" name="search" placeholder="Search...">
</div>

<div class="input-container">
    <label for="url">URL Input:</label>
    <input type="url" id="url" name="url" placeholder="Enter URL...">
</div>

<div class="input-container">
    <label for="submit">Submit Button:</label>
    <input type="submit" id="submit" name="submit" value="Submit">
</div>

</body>
</html>

