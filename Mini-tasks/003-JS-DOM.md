# JS, DOM Micro Tasks

1. Color a `span/div` element content when a user moves the mouse over the element. <!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Color Change on Hover</title>
  <style>
    /* CSS styles for the element */
    .hover-element {
      display: inline-block; /* or block, depending on your layout needs */
      padding: 10px;
      background-color: #f0f0f0; /* Default background color */
      cursor: pointer; /* Optional: Change cursor to pointer on hover */
    }
  </style>
</head>
<body>

  <!-- Example span element -->
  <span class="hover-element" onmouseover="changeColor(this)" onmouseout="restoreColor(this)">
    Hover over me!
  </span>

  <!-- Example div element -->
  <!--
  <div class="hover-element" onmouseover="changeColor(this)" onmouseout="restoreColor(this)">
    Hover over me!
  </div>
  -->

  <!-- JavaScript to change colors -->
  <script>
    function changeColor(element) {
      element.style.backgroundColor = 'lightblue'; // Change background color on mouse over
    }

    function restoreColor(element) {
      element.style.backgroundColor = '#f0f0f0'; // Restore original color on mouse out
    }
  </script>

</body>
</html>


2. Use prompt to read a value from user and display it in the span element. <!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>User Input Display</title>
  <style>
    /* CSS styles for the element */
    .user-input-span {
      display: inline-block;
      padding: 10px;
      background-color: #f0f0f0;
      cursor: pointer;
    }
  </style>
</head>
<body>

  <!-- Span element to display user input -->
  <span id="userInputDisplay" class="user-input-span"
        onclick="displayUserInput()">
    Click to enter text!
  </span>

  <!-- JavaScript to handle user input -->
  <script>
    function displayUserInput() {
      var userInput = prompt('Enter some text:');
      if (userInput !== null) { // Check if user clicked OK or Cancel
        document.getElementById('userInputDisplay').textContent = userInput;
      }
    }
  </script>

</body>
</html>


3. Display the mouse X and Y coordinates in a `<span>` tag when you click on a `<h1>` tag which contains a paragraph. <!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Mouse Coordinates Display</title>
  <style>
    /* CSS styles for the elements */
    #mouseCoordinates {
      display: inline-block;
      padding: 5px;
      background-color: #f0f0f0;
    }
  </style>
</head>
<body>

  <!-- Heading with a paragraph -->
  <h1 id="headingWithParagraph">Click here to show mouse coordinates
    <p>This is a paragraph inside the heading.</p>
  </h1>

  <!-- Span tag to display mouse coordinates -->
  <span id="mouseCoordinates"></span>

  <!-- JavaScript to handle mouse click and display coordinates -->
  <script>
    // Get the heading element
    var heading = document.getElementById('headingWithParagraph');

    // Add click event listener to the heading
    heading.addEventListener('click', function(event) {
      // Get mouse X and Y coordinates relative to the document
      var mouseX = event.pageX;
      var mouseY = event.pageY;

      // Get the span element to display coordinates
      var coordinatesSpan = document.getElementById('mouseCoordinates');

      // Update the span content with coordinates
      coordinatesSpan.textContent = 'Mouse X: ' + mouseX + ', Mouse Y: ' + mouseY;
    });
  </script>

</body>
</html>


4. Write a Javascript code for character counts in the `textarea`.

   # Example: ![](https://miro.medium.com/max/1600/1*1HI4NXCeCz1EiIWcIE_0iQ.gif)
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Character Count in Textarea</title>
  <style>
    /* Optional: CSS styles for the textarea and character count */
    #textareaContainer {
      margin-bottom: 20px;
    }
    #charCount {
      font-size: 14px;
      color: #666;
    }
  </style>
</head>
<body>

  <div id="textareaContainer">
    <textarea id="inputText" rows="4" cols="50" placeholder="Type something..."></textarea>
  </div>

  <div id="charCount">Characters: 0</div>

  <script>
    // Get the textarea element
    var textarea = document.getElementById('inputText');
    
    // Get the div element where character count will be displayed
    var charCount = document.getElementById('charCount');

    // Add input event listener to the textarea
    textarea.addEventListener('input', function() {
      // Get the current value of the textarea
      var text = textarea.value;

      // Count the number of characters
      var count = text.length;

      // Update the character count display
      charCount.textContent = 'Characters: ' + count;
    });
  </script>

</body>
</html>

5. Convert a given number from decimal to binary or hexadecimal function decimalToBinary(decimalNumber) {
  return (decimalNumber >>> 0).toString(2);
}

// Example usage:
var decimalNumber = 123; // Replace with your decimal number
var binaryNumber = decimalToBinary(decimalNumber);
console.log(`Binary representation of ${decimalNumber}: ${binaryNumber}`);

function decimalToHexadecimal(decimalNumber) {
  return decimalNumber.toString(16).toUpperCase();
}

// Example usage:
var decimalNumber = 123; // Replace with your decimal number
var hexadecimalNumber = decimalToHexadecimal(decimalNumber);
console.log(`Hexadecimal representation of ${decimalNumber}: ${hexadecimalNumber}`);


6. With Javascript write a simple from validation <!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Simple Form Validation</title>
  <style>
    .error-message {
      color: red;
      font-size: 12px;
    }
  </style>
</head>
<body>

  <h2>Simple Form Validation Example</h2>

  <form id="myForm" onsubmit="return validateForm()">
    <label for="name">Name:</label><br>
    <input type="text" id="name" name="name"><br>
    <span id="nameError" class="error-message"></span><br><br>

    <label for="email">Email:</label><br>
    <input type="email" id="email" name="email"><br>
    <span id="emailError" class="error-message"></span><br><br>

    <input type="submit" value="Submit">
  </form>

  <script>
    function validateForm() {
      var name = document.getElementById('name').value;
      var email = document.getElementById('email').value;
      var nameError = document.getElementById('nameError');
      var emailError = document.getElementById('emailError');
      var isValid = true;

      // Reset error messages
      nameError.textContent = '';
      emailError.textContent = '';

      // Validate name
      if (name.trim() === '') {
        nameError.textContent = 'Name is required';
        isValid = false;
      }

      // Validate email if provided
      if (email.trim() !== '') {
        // Basic email validation with regex
        var emailRegex = /^[^\s@]+@[^\s@]+\.[^\s@]+$/;
        if (!emailRegex.test(email)) {
          emailError.textContent = 'Invalid email format';
          isValid = false;
        }
      }

      return isValid;
    }
  </script>

</body>
</html>


7. In your HTML Add two buttons, where first button action for full screen mode and the second button for exit from full screen mode.
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Fullscreen Mode Toggle</title>
  <style>
    #content {
      height: 300px; /* Example content height */
      background-color: #f0f0f0;
      padding: 20px;
      text-align: center;
    }
  </style>
</head>
<body>

  <div id="content">
    <h2>Fullscreen Mode Toggle Example</h2>
    <p>This is some example content.</p>

    <button onclick="toggleFullScreen()">Enter Fullscreen</button>
    <button onclick="exitFullScreen()">Exit Fullscreen</button>
  </div>

  <script>
    var content = document.getElementById('content');

    function toggleFullScreen() {
      if (!document.fullscreenElement) {
        content.requestFullscreen().catch(err => {
          alert(`Error attempting to enable full-screen mode: ${err.message}`);
        });
      }
    }

    function exitFullScreen() {
      if (document.fullscreenElement) {
        document.exitFullscreen();
      }
    }
  </script>

</body>
</html>

8. When user press any key in your html page show a alert that `Invalid Key Pressed`, but when user press spacebar show an alert `Thank You..!!` and close the current window. <!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Key Press Event Handling</title>
</head>
<body>

  <h2>Press any key to see the alerts</h2>

  <script>
    // Function to handle key press events
    function handleKeyPress(event) {
      var keyCode = event.keyCode || event.which; // Get the key code

      if (keyCode === 32) { // 32 is the key code for spacebar
        alert('Thank You..!!');
        window.close(); // Close the current window
      } else {
        alert('Invalid Key Pressed');
      }
    }

    // Add event listener for key press events on the whole document
    document.addEventListener('keypress', handleKeyPress);
  </script>

</body>
</html>


9. When a cursor is moved over an content, allow the user to edit the content in HTML page.<br>
   NOTE: Input element should not be used.
 <!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Edit Content on Hover</title>
  <style>
    .editable-content {
      padding: 10px;
      border: 1px solid #ccc;
      display: inline-block;
      cursor: pointer;
    }
  </style>
</head>
<body>

  <div class="editable-content" onmouseover="makeEditable(this)" onmouseout="makeNonEditable(this)">
    Hover over this content to edit it.
  </div>

  <script>
    function makeEditable(element) {
      element.setAttribute('contenteditable', true);
      element.focus(); // Automatically focus on the element to start editing
    }

    function makeNonEditable(element) {
      element.removeAttribute('contenteditable');
    }
  </script>

</body>
</html>

