# Task Eleven: Image Hover Effect

## Objective

Create an HTML page that includes an image element. Implement an effect where the image disappears when the mouse hovers over it and reappears when the mouse is not hovering. This should be done using JavaScript only. Optionally, provide a CSS-only solution as well.

## Steps

1. **Create the HTML File:**
   - In VSCodium, create a file named `index.html`.

2. **Link an Image:**
   - Use an image from the internet. Ensure the image URL is correct.

3. **JavaScript Implementation:**
   - The image should disappear on hover and reappear when the mouse is not in the area.
   - Use JavaScript to achieve this effect.
  
4. **Optional CSS Implementation:**
   - If curious, also provide a CSS-only solution to achieve the same hover effect.
  
5. **Upload to GitHub:**
   - Upload the `index.html` file to the `taskeleven` repository in your GitHub repo.

## JavaScript Implementation

        const imgElement = document.getElementById('hoverImage');

        imgElement.onmouseover = function() {
            imgElement.style.visibility = 'hidden';
        };

        imgElement.onmouseout = function() {
            imgElement.style.visibility = 'visible';
        };

## CSS Implementation

        img:hover {
            visibility: hidden;
        }
