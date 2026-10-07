# Nova — Modern Landing Page

A modern, clean, and fully responsive landing page built with **HTML and CSS only** (no JavaScript, no frameworks).

## Preview

The page includes four main sections:

- **Navbar** — fixed, blurred, with animated link underlines
- **Hero** — headline, badge, and call-to-action buttons
- **Features** — three cards in a responsive grid
- **Contact / CTA** — call-to-action with email link

## Project Structure

```
Landing_Page/
├── index.html   # Page markup
├── style.css    # All styling (design tokens, layout, responsive rules)
└── README.md
```

## Getting Started

No build step or dependencies required.

1. Clone or download the project.
2. Open `index.html` in any modern browser.

Or serve it locally:

```bash
# Using Python
python -m http.server 8000

# Using Node.js
npx serve
```

Then visit `http://localhost:8000`.

## Customization

Colors, spacing, and radii are defined as CSS custom properties in `:root` at the top of `style.css`. Change them there to re-theme the whole page:

```css
:root {
    --color-primary: #2563eb;
    --container-width: 1140px;
    --radius-lg: 18px;
    /* ... */
}
```

Update the contact email in `index.html`:

```html
<a href="mailto:your-email@example.com" class="btn btn-primary">Contact Us</a>
```

## Responsive Design

The layout adapts at two breakpoints in `style.css`:

- **`max-width: 768px`** — navbar stacks, feature cards become a single column, hero buttons stretch full width
- **`max-width: 420px`** — tighter nav spacing and full-width buttons

## Browser Support

Works in all modern browsers (Chrome, Firefox, Edge, Safari).

## License

Free to use for personal and commercial projects.
