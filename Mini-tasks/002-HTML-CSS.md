# [Guvi Zen](https://www.guvi.io/zen/)

## HTML & CSS Tasks.

1. Design the below equation using HTML & CSS <!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Wave Equation</title>
    <script src="https://polyfill.io/v3/polyfill.min.js?features=es6"></script>
    <script id="MathJax-script" async src="https://cdn.jsdelivr.net/npm/mathjax@3/es5/tex-mml-chtml.js"></script>
</head>
<body>
    <p>$$\frac{\partial^2 u}{\partial t^2} = c^2 \frac{\partial^2 u}{\partial x^2}$$</p>
</body>
</html>


   ![click here to view sample equation](https://i.insider.com/4ff178a269bedd6f1800000f?width=600&format=jpeg&auto=webp)

2. Write a css rule of rounded rectangle, dashed border, grayscale for all image tags in your webpage.
   <!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Styled Images</title>
    <script src="https://polyfill.io/v3/polyfill.min.js?features=es6"></script>
    <script id="MathJax-script" async src="https://cdn.jsdelivr.net/npm/mathjax@3/es5/tex-mml-chtml.js"></script>
    <style>
        img {
            border: 2px dashed #000; /* Dashed border */
            border-radius: 15px; /* Rounded corners */
            filter: grayscale(100%); /* Grayscale */
        }
    </style>
</head>
<body>
    <p>$$\frac{\partial^2 u}{\partial t^2} = c^2 \frac{\partial^2 u}{\partial x^2}$$</p>
    <img src="path-to-your-image.jpg" alt="Example Image">
</body>
</html>


3. Write a media rule to change only the font size of web page when it's resized. <!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Responsive Font Size</title>
    <script src="https://polyfill.io/v3/polyfill.min.js?features=es6"></script>
    <script id="MathJax-script" async src="https://cdn.jsdelivr.net/npm/mathjax@3/es5/tex-mml-chtml.js"></script>
    <style>
        body {
            font-size: 16px; /* Default font size */
        }
        
        /* Small devices (phones, 600px and down) */
        @media only screen and (max-width: 600px) {
            body {
                font-size: 14px;
            }
        }

        /* Medium devices (portrait tablets and large phones, 600px and up) */
        @media only screen and (min-width: 600px) and (max-width: 768px) {
            body {
                font-size: 16px;
            }
        }

        /* Large devices (landscape tablets, 768px and up) */
        @media only screen and (min-width: 768px) and (max-width: 992px) {
            body {
                font-size: 18px;
            }
        }

        /* Extra large devices (large laptops and desktops, 992px and up) */
        @media only screen and (min-width: 992px) {
            body {
                font-size: 20px;
            }
        }
    </style>
</head>
<body>
    <p>$$\frac{\partial^2 u}{\partial t^2} = c^2 \frac{\partial^2 u}{\partial x^2}$$</p>
    <img src="path-to-your-image.jpg" alt="Example Image">
</body>
</html>


4. Use HTML & CSS to display different types of cursors. <!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Different Cursors</title>
    <style>
        .default-cursor {
            cursor: default;
        }
        
        .pointer-cursor {
            cursor: pointer;
        }
        
        .crosshair-cursor {
            cursor: crosshair;
        }
        
        .text-cursor {
            cursor: text;
        }
        
        .move-cursor {
            cursor: move;
        }
        
        .not-allowed-cursor {
            cursor: not-allowed;
        }
        
        .wait-cursor {
            cursor: wait;
        }
        
        .help-cursor {
            cursor: help;
        }
    </style>
</head>
<body>
    <h1>Different Cursor Types</h1>
    
    <p class="default-cursor">Default Cursor: Hover over this text.</p>
    <p class="pointer-cursor">Pointer Cursor: Hover over this text.</p>
    <p class="crosshair-cursor">Crosshair Cursor: Hover over this text.</p>
    <p class="text-cursor">Text Cursor: Hover over this text.</p>
    <p class="move-cursor">Move Cursor: Hover over this text.</p>
    <p class="not-allowed-cursor">Not Allowed Cursor: Hover over this text.</p>
    <p class="wait-cursor">Wait Cursor: Hover over this text.</p>
    <p class="help-cursor">Help Cursor: Hover over this text.</p>
</body>
</html>


5. Write a CSS class that meets the **Box Model** requirement for all the div tags in your page.

   - Use certain properties padding, margin, border. <!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Box Model Example</title>
    <style>
        .box-model {
            padding: 20px;    /* Inner spacing within the div */
            margin: 15px;     /* Outer spacing outside the div */
            border: 2px solid #000; /* Border around the div */
            box-sizing: border-box; /* Ensures padding and border are included in the element's total width and height */
        }
    </style>
</head>
<body>
    <div class="box-model">This is a div with the box model applied.</div>
    <div class="box-model">Another div with the same box model.</div>
    <div class="box-model">Yet another div with the box model applied.</div>
</body>
</html>


6. Write a CSS class to change size of font, color font family when mouse moves over of span tag in your webpage.
   <!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Hover Effects on Span</title>
    <style>
        .hover-effect {
            transition: all 0.3s ease; /* Smooth transition for the changes */
        }

        .hover-effect:hover {
            font-size: 20px;           /* Changes font size on hover */
            color: #ff5733;            /* Changes font color on hover */
            font-family: 'Arial', sans-serif; /* Changes font family on hover */
        }
    </style>
</head>
<body>
    <p>Hover over the following text to see the effect:</p>
    <span class="hover-effect">This text will change when you hover over it.</span>
</body>
</html>


7. Write a CSS 2D rule with `translate()` property to move an element.
   <!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>CSS Translate Example</title>
    <style>
        .translate-effect {
            width: 100px;
            height: 100px;
            background-color: lightblue;
            transition: transform 0.3s ease; /* Smooth transition for the transform property */
        }

        .translate-effect:hover {
            transform: translate(50px, 100px); /* Moves the element 50px to the right and 100px down on hover */
        }
    </style>
</head>
<body>
    <div class="translate-effect">Hover over me!</div>
</body>
</html>


8. Define a CSS class to show tooltip when mouse moved over the elements.
   <!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Tooltip Example</title>
    <style>
        .tooltip {
            position: relative; /* Required for positioning the tooltip */
            display: inline-block; /* Makes sure the element displays inline */
            cursor: pointer; /* Changes cursor to pointer on hover */
        }

        .tooltip::after {
            content: attr(data-tooltip); /* Use the value of the data-tooltip attribute as content */
            position: absolute;
            bottom: 100%; /* Position above the element */
            left: 50%;
            transform: translateX(-50%);
            background-color: #333;
            color: #fff;
            padding: 5px;
            border-radius: 5px;
            white-space: nowrap; /* Prevents the tooltip text from wrapping */
            visibility: hidden; /* Hide the tooltip by default */
            opacity: 0;
            transition: opacity 0.3s;
        }

        .tooltip:hover::after {
            visibility: visible; /* Show the tooltip on hover */
            opacity: 1;
        }
    </style>
</head>
<body>
    <p>Hover over the following text to see the tooltip:</p>
    <span class="tooltip" data-tooltip="This is a tooltip!">Hover over me!</span>
</body>
</html>


9. For the below shown image apply `clip property` with values of right & bottom and display the output.

   ![](https://encrypted-tbn0.gstatic.com/images?q=tbn%3AANd9GcR1WuQLHjaoqFLQBVJTPmqVG6WfIwK2jDxf1RAycCQJJhuhjit6&usqp=CAU) <!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Tooltip Example</title>
    <style>
        .tooltip {
            position: relative; /* Required for positioning the tooltip */
            display: inline-block; /* Makes sure the element displays inline */
            cursor: pointer; /* Changes cursor to pointer on hover */
        }

        .tooltip::after {
            content: attr(data-tooltip); /* Use the value of the data-tooltip attribute as content */
            position: absolute;
            bottom: 100%; /* Position above the element */
            left: 50%;
            transform: translateX(-50%);
            background-color: #333;
            color: #fff;
            padding: 5px;
            border-radius: 5px;
            white-space: nowrap; /* Prevents the tooltip text from wrapping */
            visibility: hidden; /* Hide the tooltip by default */
            opacity: 0;
            transition: opacity 0.3s;
        }

        .tooltip:hover::after {
            visibility: visible; /* Show the tooltip on hover */
            opacity: 1;
        }
    </style>
</head>
<body>
    <p>Hover over the following text to see the tooltip:</p>
    <span class="tooltip" data-tooltip="This is a tooltip!">Hover over me!</span>
</body>
</html>

<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Clip Property Example</title>
    <style>
        .clipped-image {
            position: absolute;
            clip: rect(auto, 100px, 100px, auto); /* top, right, bottom, left */
        }
    </style>
</head>
<body>
    <div style="position: relative; width: 200px; height: 200px;">
        <img src="https://encrypted-tbn0.gstatic.com/images?q=tbn%3AANd9GcR1WuQLHjaoqFLQBVJTPmqVG6WfIwK2jDxf1RAycCQJJhuhjit6&usqp=CAU" alt="Example Image" class="clipped-image">
    </div>
</body>
</html>


10. Design the below image using HTML & CSS.

![](https://2.bp.blogspot.com/-uBWojLXcSFs/Vk31LrbRLJI/AAAAAAAAAtI/UydMrgJ2a94/s1600/1.jpg)
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Image Design</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            display: flex;
            justify-content: center;
            align-items: center;
            height: 100vh;
            margin: 0;
            background-color: #f0f0f0;
        }

        .container {
            text-align: center;
            background-color: #fff;
            padding: 20px;
            border: 2px solid #ddd;
            border-radius: 10px;
            box-shadow: 0 0 10px rgba(0, 0, 0, 0.1);
        }

        .container img {
            max-width: 100%;
            border: 5px solid #ddd;
            border-radius: 10px;
        }

        .title {
            font-size: 24px;
            margin: 20px 0 10px;
        }

        .subtitle {
            font-size: 18px;
            color: #555;
            margin: 10px 0;
        }

        .description {
            font-size: 16px;
            color: #777;
            margin: 10px 0;
        }
    </style>
</head>
<body>
    <div class="container">
        <img src="https://2.bp.blogspot.com/-uBWojLXcSFs/Vk31LrbRLJI/AAAAAAAAAtI/UydMrgJ2a94/s1600/1.jpg" alt="Example Image">
        <div class="title">Sample Title</div>
        <div class="subtitle">Subtitle Here</div>
        <div class="description">This is a description text that provides more details about the content shown above.</div>
    </div>
</body>
</html>

11. Use the required property to reshape a div, as example shown below.

    ![](https://encrypted-tbn0.gstatic.com/images?q=tbn%3AANd9GcSjWqFJvJ6nFFnDbuz2-BOUWcPHZpE0fF2AiWcoBQM6JO-RPm3_&usqp=CAU)
<div class="custom-shape"></div>
.custom-shape {
    width: 300px; /* Adjust width as needed */
    height: 200px; /* Adjust height as needed */
    background-color: #3498db; /* Background color */
    clip-path: polygon(0 0, 100% 0, 80% 100%, 0 100%);
    /* Explanation of clip-path:
       - polygon defines a shape using coordinates
       - Here, it starts at top-left (0 0), goes to top-right (100% 0),
         then to 80% across the width at the bottom-right, and finally
         back to the bottom-left (0 100%).
    */
}

12. Use CSS to set a background image should be centered and should not repeat.
    .background-image {
    background-image: url('path/to/your/image.jpg'); /* Replace with your image path */
    background-size: cover; /* Cover the entire element */
    background-position: center; /* Center the background image */
    background-repeat: no-repeat; /* Do not repeat the background image */
    width: 100%; /* Adjust width as needed */
    height: 400px; /* Adjust height as needed */
}
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Centered Background Image</title>
    <style>
        .background-image {
            background-image: url('path/to/your/image.jpg');
            background-size: cover;
            background-position: center;
            background-repeat: no-repeat;
            width: 100%;
            height: 400px;
        }
    </style>
</head>
<body>

<div class="background-image">
    <!-- Content inside the div with background image -->
</div>

</body>
</html>


14. Write CSS rules to set the direction of the flexible items inside the `<div></div>` element in reverse order.
     .container {
    display: flex; /* Enable flexbox layout */
    flex-direction: row-reverse; /* Arrange items in reverse order horizontally */
    /* If you want items to wrap, you can use flex-wrap */
    flex-wrap: wrap; /* Items wrap onto multiple lines if necessary */
    /* Additional styling as needed */
    justify-content: flex-start; /* Align items to the start of the flex container */
}

.item {
    /* Styling for each flex item */
    width: 100px; /* Example width */
    height: 100px; /* Example height */
    margin: 10px; /* Example margin */
    background-color: #3498db; /* Example background color */
}

<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Flexbox Reverse Order Example</title>
    <style>
        .container {
            display: flex;
            flex-direction: row-reverse;
            flex-wrap: wrap;
            justify-content: flex-start;
            /* Additional styling for the container if needed */
            background-color: #f0f0f0; /* Example background color */
            padding: 20px; /* Example padding */
        }

        .item {
            width: 100px;
            height: 100px;
            margin: 10px;
            background-color: #3498db;
            /* Additional styling for each item if needed */
        }
    </style>
</head>
<body>

<div class="container">
    <div class="item">Item 1</div>
    <div class="item">Item 2</div>
    <div class="item">Item 3</div>
    <div class="item">Item 4</div>
    <div class="item">Item 5</div>
</div>

</body>
</html>


15. Give the `<div>` element an image border using the image "border.png". Slice the image at 30px and stretch it.
    .div-with-border {
    width: 300px; /* Example width */
    height: 200px; /* Example height */
    border-width: 30px; /* Width of the sliced border */
    border-image-source: url('border.png'); /* Path to your border image */
    border-image-slice: 30; /* Slice the border image into 30px sections */
    border-image-repeat: stretch; /* Stretch the border image to fit */
    /* Optional: Adjust padding or margin as needed */
    padding: 20px; /* Example padding */
}

<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Border Image Example</title>
    <style>
        .div-with-border {
            width: 300px;
            height: 200px;
            border-width: 30px;
            border-image-source: url('border.png');
            border-image-slice: 30;
            border-image-repeat: stretch;
            /* Additional styling for the div if needed */
            padding: 20px; /* Example padding */
            background-color: #f0f0f0; /* Example background color */
        }
    </style>
</head>
<body>

<div class="div-with-border">
    <!-- Content inside the div with border image -->
</div>

</body>
</html>

17. Give the `<div>` element a rounded corner (25px radius) on the bottom left side.
    .rounded-corner {
    width: 300px; /* Example width */
    height: 200px; /* Example height */
    border-radius: 0 0 0 25px; /* Top-left, top-right, bottom-right, bottom-left */
    /* Optional: Additional styling */
    background-color: #3498db; /* Example background color */
    color: #ffffff; /* Example text color */
    text-align: center; /* Example text alignment */
    line-height: 200px; /* Example line height for vertical centering */
}

<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Rounded Corner Example</title>
    <style>
        .rounded-corner {
            width: 300px;
            height: 200px;
            border-radius: 0 0 0 25px;
            background-color: #3498db;
            color: #ffffff;
            text-align: center;
            line-height: 200px;
        }
    </style>
</head>
<body>

<div class="rounded-corner">
    Rounded bottom left corner
</div>

</body>
</html>

19. Remove the transparency/opacity of the `<img>` element when the user hovers over it with the mouse pointer.
    <img src="image.jpg" class="image-hover" alt="Image"> .image-hover {
    opacity: 0.7; /* Initial opacity */
    transition: opacity 0.3s ease; /* Smooth transition for opacity change */
}

.image-hover:hover {
    opacity: 1; /* Full opacity on hover */
}

<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Image Opacity on Hover</title>
    <style>
        .image-hover {
            opacity: 0.7;
            transition: opacity 0.3s ease;
            /* Additional styles for image if needed */
            width: 300px; /* Example width */
            height: 200px; /* Example height */
        }

        .image-hover:hover {
            opacity: 1;
        }
    </style>
</head>
<body>

<img src="image.jpg" class="image-hover" alt="Image">

</body>
</html>

20. Position the `<div>` element all the way to the right using absolute positioning.   <div class="absolute-right">Positioned to the right</div>.absolute-right {
    position: absolute;
    top: 0; /* Adjust as needed */
    right: 0; /* Position all the way to the right */
    /* Optional: Additional styling */
    background-color: #3498db; /* Example background color */
    color: #ffffff; /* Example text color */
    padding: 10px; /* Example padding */
}
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Absolute Positioning Example</title>
    <style>
        .absolute-right {
            position: absolute;
            top: 0;
            right: 0;
            background-color: #3498db;
            color: #ffffff;
            padding: 10px;
            /* Additional styles for the div if needed */
        }

        /* Optional: Styles for body or container */
        body {
            position: relative; /* Ensure body or container is positioned for absolute positioning */
            /* Additional styles for body if needed */
        }
    </style>
</head>
<body>

<div class="absolute-right">Positioned to the right</div>

</body>
</html>

21. Add a scrollbar to the `<div>` element. <div class="scrollable-div">
    <!-- Content that may overflow -->
    <p>Lorem ipsum dolor sit amet, consectetur adipiscing elit. Integer nec odio. Praesent libero.</p>
    <!-- More content -->
</div>
.scrollable-div {
    width: 300px; /* Example width */
    height: 200px; /* Example height */
    overflow: auto; /* Add scrollbar when content overflows */
    /* Optional: Additional styling */
    border: 1px solid #ccc; /* Example border */
    padding: 10px; /* Example padding */
}
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Scrollable Div Example</title>
    <style>
        .scrollable-div {
            width: 300px;
            height: 200px;
            overflow: auto;
            border: 1px solid #ccc;
            padding: 10px;
            /* Additional styles for the div if needed */
        }
    </style>
</head>
<body>

<div class="scrollable-div">
    <p>Lorem ipsum dolor sit amet, consectetur adipiscing elit. Integer nec odio. Praesent libero.</p>
    <p>Sed cursus ante dapibus diam. Sed nisi. Nulla quis sem at nibh elementum imperdiet.</p>
    <!-- Add more content as needed -->
</div>

</body>
</html>


22. Set a linear gradient background for the `<div>` element, going from the top to bottom, transitioning from "white" to "red" to "blue" to "green". <div class="gradient-div">
    <!-- Content inside the div -->
</div>
.gradient-div {
    width: 300px; /* Example width */
    height: 200px; /* Example height */
    background: linear-gradient(to bottom, white, red, blue, green);
    /* Additional styling */
    padding: 20px; /* Example padding */
    color: #ffffff; /* Example text color */
    text-align: center; /* Example text alignment */
    line-height: 200px; /* Example line height for vertical centering */
}
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Gradient Background Example</title>
    <style>
        .gradient-div {
            width: 300px;
            height: 200px;
            background: linear-gradient(to bottom, white, red, blue, green);
            padding: 20px;
            color: #ffffff;
            text-align: center;
            line-height: 200px;
            /* Additional styles for the div if needed */
        }
    </style>
</head>
<body>

<div class="gradient-div">
    Gradient background from top to bottom
</div>

</body>
</html>


23. With the transform property, rotate the `<div>` element 45 degrees.
<div class="rotate-div">
    <!-- Content inside the div -->
</div>
.rotate-div {
    width: 200px; /* Example width */
    height: 200px; /* Example height */
    background-color: #3498db; /* Example background color */
    color: #ffffff; /* Example text color */
    text-align: center; /* Example text alignment */
    line-height: 200px; /* Example line height for vertical centering */
    transform: rotate(45deg); /* Rotate the div 45 degrees */
}
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Rotate Div Example</title>
    <style>
        .rotate-div {
            width: 200px;
            height: 200px;
            background-color: #3498db;
            color: #ffffff;
            text-align: center;
            line-height: 200px;
            transform: rotate(45deg);
            /* Additional styles for the div if needed */
        }
    </style>
</head>
<body>

<div class="rotate-div">
    Rotated div
</div>

</body>
</html>


### Additional Try outs

1.

![](https://raw.githubusercontent.com/rvsp/files/master/div-row-cols.png)

2.

![](https://developer.paciellogroup.com/wp-content/uploads/2015/09/regions-typical1.png)

3.

![](https://ps.w.org/pricing-table/assets/screenshot-3.png?rev=1396861)

4.

![](https://s3-us-west-2.amazonaws.com/s.cdpn.io/429997/Screen%20Shot%202016-12-08%20at%2001.02.41.png)

---

## Practice

### Flexbox
https://flexboxfroggy.com/

http://www.flexboxdefense.com/

https://flexbox.malven.co/

https://flukeout.github.io/

https://mastery.games/

### Grid
https://cssgridgarden.com/

https://learncssgrid.com/

https://grid.layoutit.com/

https://grid.malven.co/


