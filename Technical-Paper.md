# Browser Rendering

## What is Browser Rendering ??
- Browser rendering is the process of bringing code into a visually-rendered webpage.
- Users do not see code in their "browsers" (Safari, Mozilla, Chrome, Brave); users see in their browsers data retrieved in a view designed by the coder. 

## How does the process of browser rendering work ??

1. When a user requests a webpage, the browser gets associated HTML-CSS-JavaScript files from the server.
2. It then parses the HTML to build a Document Object Model (DOM) and the CSS to create a CSS Object Model (CSSOM).
3. These two models are then combined so that the content comes as desired to be shown by the designer of the content.
4. The browser then "paints" or draws the contents onto the screen based on the render structure.
This entire sequence is what we refer to as browser rendering.

## What rendering engines are used in different browsers ??
Various browsers use different rendering engines:

- Internet Explorer: Trident
- Firefox: Gecko
- Safari: WebKit
- Chrome and Opera (version 15+): Blink, which is a fork of WebKit.

### Explain the rendering process detail.
- Parsing HTML and Creating the DOM: The rendering engine starts parsing the HTML document and builds the DOM (Document Object Model), which is a tree structure of HTML elements.
- Parsing CSS and Creating the CSSOM: Style data from both external CSS files and <style> elements in HTML is parsed. The CSS is used along with visual instructions to create another tree structure, known as the CSSOM.
- Building the Render Tree: The DOM and CSSOM trees combine to form the render tree, containing all the visible elements with visual attributes like colors and dimensions. These elements are laid out in the correct order to display on the screen.
- Layout (Reflow): The rendering engine assigns each node in the render tree exact coordinates to determine its placement on the screen.
- Painting: The render tree is then traversed, and each node is painted onto the screen using the browser's UI backend layer.
- This process happens progressively. For a smoother user experience, browsers attempt to display content on the screen as quickly as possible rather than waiting for the entire HTML file to be parsed.
-  As a result, portions of the page are displayed as they become ready, allowing rendering to continue while the remaining content is fetched from the network.

## References
1. Google
2. Quora
3. LogRocket blog
4. Medium
