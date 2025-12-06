# HTML Structure Guide

## General Layout
Most pages follow a standard "Holy Grail" or vertically stacked layout:
1.  **Header**: The top navigation bar found in `header.css` and repeated in every HTML file.
2.  **Main**: The unique content for that specific page, wrapped in a `<main>` tag.
3.  **Footer**: The bottom links found in `footer.css` and repeated in every HTML file.

## Key Components

### The Navigation Bar (`header.css`)
We use Flexbox (`display: flex`) extensively here to align items horizontally.
- `.navbar-main`: The black top bar. It uses `justify-content: space-between` or flex-grow to distribute space.
- `.nav-search`: Uses flex-grow to take up all available remaining width between the logo and the account links.

### The Grid System
On the homepage (`index.html`), we use CSS Grid (`display: grid`) for the product cards.
```css
.product-grid {
    display: grid;
    grid-template-columns: repeat(4, 1fr); /* 4 equal columns */
    gap: 20px;
}
```
This is a powerful way to create responsive layouts. As the screen gets smaller, we use `@media` queries to change the number of columns from 4 to 3, then 2, then 1.

### Forms
The Search Bar and Sign-In page use standard HTML `<form>` elements.
- `<input type="text">`: For text entry.
- `<button>`: For submitting the form.
- `<select>`: For dropdown menus.
