<!---------- Media Queries Notes----------->
Media queries are a powerful feature of CSS that allow developers to apply different styles to a webpage based on the characteristics of the user's device or viewport. They enable responsive design, ensuring that websites look and function well across a variety of screen sizes and devices.


Uses in Website:
- Responsive layout adjustments
- Image optimization for different screen sizes
- Typography adjustments for better readability
- Navigation menu modifications for mobile devices

Syntax:
@media media-type and (condition) {

    /* CSS rules go here */
}

In media queries when we use a fix width and height for an element, it will not be responsive. It will not adjust according to the screen size.
Also media queries sizes are set according to viewport size, so if we use a fix width and height for an element, it will not be responsive. It will not adjust according to the screen size. 
Instead, we can use relative units like %, em, rem, vh, vw to make the element responsive.
    
    