# Pages Guide

## Homepage (`index.html`)
- **Hero Section**: Uses a background gradient to simulate the banner image area.
- **Product Cards**: Simple boxes with white backgrounds and drop shadows (optional) or borders.

## Search Results (`search.html`)
- **Sidebar**: A fixed-width column on the left for filters.
- **Results List**: A flexible column on the right. Each result is a "Flexbox" container with an image on the left and details on the right.

## Product Detail (`product.html`)
- **Sticky Gallery**: The image on the left stays visible while you scroll (using `position: sticky` if content is long enough).
- **Buy Box**: The box on the far right with the "Add to Cart" button. It uses a fixed width and is crucial for conversion (getting people to buy).

## Cart (`cart.html`)
- Lists items vertically.
- Separation of concerns: The list of items is one block, the "Subtotal" box is another block on the right.

## Sign In (`signin.html`)
- A completely different layout. No complex header/footer.
- Focuses the user's attention purely on the form in the center of the screen.
