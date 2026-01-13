# NexTech Solutions - Advanced HTML & CSS Project

## Project Overview
This project is a fully responsive, multi-page website developed using **pure HTML5 and CSS3**. It adheres to strict technical constraints: no JavaScript, no CSS frameworks (like Bootstrap), and follows a mobile-first design approach.

## Design Choices & CSS Techniques

### 1. CSS Architecture
- **Modular CSS**: Styles are split into `main.css` (variables/typography), `layout.css` (grid/flex structures), and `animations.css`.
- **CSS Variables**: Used `:root` for color palette, spacing, and border-radius to ensure consistency and easy theming.

### 2. Layout & Responsiveness
- **Mobile-First**: Base styles are written for mobile screens, with media queries (`min-width: 768px`) for tablet/desktop overrides.
- **CSS Grid**: Used heavily in the `Services` and `Pricing` pages to create responsive card layouts that automatically adjust columns based on available width (`repeat(auto-fit, minmax(...))`).
- **Flexbox**: Used for the Navbar, About page alignment, and centering elements vertically/horizontally.

### 3. Advanced CSS Features (No JS Hacks)
- **Mobile Navigation**: Implemented using the "Checkbox Hack". A hidden `<input type="checkbox">` toggles the visibility of the menu via the general sibling selector (`~`).
- **Pricing Toggle**: Similar to the navigation, the monthly/yearly price switch is controlled by a checkbox and CSS combinators to hide/show specific `.price` spans.
- **Form Validation**: Used `:valid`, `:invalid`, and `:focus` pseudo-classes to provide real-time visual feedback (green/red borders) on the Contact page.
- **Animations**: Keyframe animations (`@keyframes`) for fade-in and slide-up effects on page load.

### 4. Accessibility
- Semantic HTML tags (`<nav>`, `<main>`, `<footer>`, `<header>`) used throughout.
- Contrast ratios optimized for text readability.
- Form inputs have associated `<label>` elements.

## Challenges Faced
- Implementing the "toggle" logic for pricing without JavaScript was the biggest challenge. It required careful HTML structuring to ensure the checkbox input was a sibling to the content intended to be modified.

## How to Run
1. Unzip the folder.
2. Open `index.html` in any modern web browser.
