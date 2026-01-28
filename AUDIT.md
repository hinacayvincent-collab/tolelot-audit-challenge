## HTML Issues

1. Incorrect CSS file name capitalization
   The stylesheet is linked using Style.CSS, which may not match the actual file name, and this is a problem because most web servers are case-sensitive and the CSS file will not load if the capitalization is incorrect; to resolve this, I will rename the file to style.css and update the link to match exactly.
2. Space in the linked HTML file name
   The anchor tag links to a file named LOGIN Page.html, which contains a space, and this is problematic because spaces can cause broken links and are considered poor practice in web development; I will rename the file to login-page.html and update the link accordingly.
   3.The “Get Started” button does not have a specified type or functionality, which is a problem because it does not perform any action and may confuse users; I will define its type or change it into a link that navigates to another page.
3. Incorrect heading and content order
   The paragraph appears before the “About Us” heading, which is incorrect because headings should introduce the content that follows and help with accessibility; I will move the heading above the paragraph it describes.
4. The HTML document is missing the <!DOCTYPE html> declaration at the top, which is a problem because without it the browser may render the page in quirks mode, leading to inconsistent behavior and layout issues across different browsers; to fix this, I will add <!DOCTYPE html> as the first line of the document to ensure proper HTML5 rendering.

## CSS Issues

1. All <div> elements are given a red background and white text, which makes the whole page look the same and hard to read because there is no visual separation between sections; to improve this, I will remove the global <div> styling and apply colors only to specific sections using classes.
2. Button has no interaction feedback
   The button has very basic styling and does not respond visually when hovered over, which can make it feel unresponsive to users; I will add hover and focus effects so users can tell when the button is interactive.
3. Inconsistent spacing and structure
   Spacing throughout the page is handled in an inconsistent way, which makes the layout feel messy and harder to maintain; I will clean this up by using a consistent spacing system and better layout structure.
4. Outdated layout technique for the cards
   The cards are laid out using inline-block, which works but is harder to manage and not ideal for modern layouts; I will switch to a more modern layout method like Flexbox to make the cards easier to align and maintain.
5. Using fixed margins to position content
   The .about section is pushed over using a large fixed left margin, which causes layout problems on smaller screens and makes the page look broken on different devices; I will change this to a more flexible layout method so the page adjusts properly to different screen sizes.

## Git / Structure Issues

1. Inconsistent and unclear file naming, File names like Style.CSS, LOGIN Page.html, and HeroImage.JPG use mixed capitalization and spaces, which is an issue because it can cause confusion, broken links, and platform-specific bugs when working with Git; the fix is to use consistent, lowercase, dash-separated file names.
2. The project appears to place HTML, CSS, and image files together without a clear folder structure, which is a problem because it makes the project harder to navigate, scale, and maintain; to fix this, the project should be organized into folders such as css/, images/, and separate HTML files at the root level.
3. Images and other assets are not stored in a dedicated folder, which makes paths harder to manage and increases the chance of broken links as the project grows; creating an assets/ or images/ folder improves clarity and maintainability.
