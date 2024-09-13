# # Task Nine

This task demonstrates how to make an image disappear when the mouse hovers over it and reappear when the mouse moves away. The hover effect is achieved using both **JavaScript** and **CSS**.

In this implementation:
- When the mouse pointer is placed over the image, the image becomes invisible.
- When the mouse pointer leaves the image area, the image reappears.

The JavaScript code uses `onmouseover` and `onmouseout` events to toggle the image's visibility. Similarly, the CSS `:hover` pseudo-class is applied to hide the image during the hover event.

### Code Example:

The HTML file includes both the necessary JavaScript and CSS to make this effect work:

```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Image Hover Effect</title>
    <style>
        /* Hide the image when hovered */
        img:hover {
            visibility: hidden;
        }
    </style>
</head>
<body>
    <h1>Hover over the image to make it disappear!</h1>
    <img id="hoverImage" src="https://via.placeholder.com/150" alt="Sample Image">

    <script>
        // Get the image element by its ID
        const img = document.getElementById('hoverImage');

        // Function to hide the image on mouse over
        img.onmouseover = function() {
            img.style.visibility = 'hidden';
        };

        // Function to show the image on mouse out
        img.onmouseout = function() {
            img.style.visibility = 'visible';
        };
    </script>
</body>
</html>
