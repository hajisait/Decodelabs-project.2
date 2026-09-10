# Project 2: Responsive Web Layout

## 📁 Files Included

- **index.html** - Main HTML structure
- **styles.css** - Complete responsive styling
- **script.js** - Navigation interactivity
- **README.md** - This file

## 🚀 How to Use

1. Create a folder on your computer
2. Place all three files in the same folder
3. Open `index.html` in your browser
4. That's it! The site is fully responsive

## ✅ Requirements Checklist

### Meta & Viewport
- ✓ `<meta charset="UTF-8">`
- ✓ `<meta name="viewport" content="width=device-width, initial-scale=1">`

### Responsive Layout
- ✓ Mobile-first base CSS (starts at 320px)
- ✓ CSS Grid for macro layout (header, main, footer)
- ✓ Flexbox for component-level organization
- ✓ Media queries at 480px, 768px, 1024px, 1440px

### Responsive Navigation
- ✓ Hamburger menu on mobile (< 768px)
- ✓ Horizontal nav on desktop (≥ 768px)
- ✓ Smooth transitions and animations
- ✓ No JavaScript required for basic display (JS enhances)

### Fluid Typography
- ✓ Using `clamp()` for all text sizes
- ✓ `h1`: clamp(1.5rem, 5vw, 3rem)
- ✓ `h2`: clamp(1.25rem, 4vw, 2rem)
- ✓ `p`: clamp(0.95rem, 1.2vw, 1.125rem)

### Proper Spacing & Alignment
- ✓ CSS variables for spacing: `--spacing` and `--spacing-lg`
- ✓ Fluid spacing with clamp()
- ✓ Consistent gaps in grids and flexbox

### Accessibility
- ✓ Min touch target size: 44x44px
- ✓ Focus states visible (blue outline)
- ✓ Support for 500% zoom without overflow
- ✓ WCAG AA compliant
- ✓ Semantic HTML structure
- ✓ ARIA labels on interactive elements

### Additional Features
- ✓ Smooth scrolling for anchor links
- ✓ Hover effects on buttons and cards
- ✓ Print-friendly styles
- ✓ Reduced motion support
- ✓ Container queries ready (future-proof)

## 📱 Responsive Breakpoints

| Device | Width | Changes |
|--------|-------|---------|
| Mobile | 0-480px | Single column, hamburger menu |
| Tablet | 480-768px | 2 columns, menu appears |
| Desktop | 768-1024px | 3+ columns, nav inline |
| Large | 1024px+ | Full layout optimization |
| XL | 1440px+ | Max-width container |

## 🎨 Key Techniques Used

1. **Mobile-First CSS** - Base styles for mobile, enhance with media queries
2. **CSS Grid** - Page layout (header, main, footer)
3. **Flexbox** - Navigation, cards, buttons
4. **Fluid Units** - %, rem, vw, clamp() for smooth scaling
5. **CSS Variables** - Easy theme management
6. **Hamburger Menu** - Click-triggered with JavaScript

## 🔧 Customization

### Change Colors
Edit the `:root` CSS variables:
```css
:root {
    --primary: #2563eb;      /* Blue */
    --secondary: #10b981;    /* Green */
    --dark: #1f2937;         /* Dark Gray */
    --light: #f3f4f6;        /* Light Gray */
}
```

### Adjust Spacing
Modify the spacing variables for tighter/looser layout:
```css
--spacing: clamp(1rem, 2vw, 2rem);      /* 1-2rem */
--spacing-lg: clamp(1.5rem, 4vw, 3rem); /* 1.5-3rem */
```

### Change Logo Text
In `index.html`, find and edit:
```html
<div class="logo">Design Studio</div>
```

### Add Navigation Links
In `index.html`, add to the nav:
```html
<nav id="navMenu">
    <a href="#home">Home</a>
    <a href="#new-section">New Section</a>
</nav>
```

## 📊 CSS Architecture

```
* Reset
├── Root Variables
├── Typography (h1, h2, h3, p)
├── Layout (Grid for page, Flexbox for components)
├── Components
│   ├── Header/Nav
│   ├── Hero
│   ├── Features
│   ├── Projects
│   └── Footer
└── Media Queries (480px, 768px, 1024px, 1440px)
```

## ♿ Accessibility Features

- **Keyboard Navigation**: Tab through all interactive elements
- **Screen Readers**: Semantic HTML + ARIA labels
- **Touch Targets**: All buttons/links are 44x44px minimum
- **Color Contrast**: WCAG AA compliant
- **Focus Indicators**: Clear blue outline on focus
- **Zoom Support**: Works at 200%, 300%, 500% without breaking

## 📈 Performance Tips

1. Images are optimized (use WebP where possible)
2. CSS is single file (no critical CSS split needed)
3. JavaScript is minimal (vanilla JS, no frameworks)
4. No external dependencies (pure HTML/CSS/JS)

## 🐛 Testing

Test your responsive design:
1. **Desktop**: Open in full browser window
2. **Tablet**: Resize to 768px width
3. **Mobile**: Resize to 375px width (iPhone size)
4. **Zoom**: Use Ctrl/Cmd + Plus to test 200%, 300% zoom
5. **Hamburger**: Click the ☰ button on mobile to test menu

## 📚 Resources Referenced

- MDN Web Docs (CSS Grid, Flexbox)
- CSS-Tricks (responsive design patterns)
- Web.dev (accessibility guidelines)
- WCAG 2.1 Standards

## 🎯 Learning Outcomes

After completing this project, you understand:
- ✓ CSS Grid for 2D layouts
- ✓ Flexbox for 1D layouts
- ✓ Fluid typography with clamp()
- ✓ Mobile-first responsive design
- ✓ Hamburger navigation patterns
- ✓ Accessible touch targets
- ✓ CSS variables for theming
- ✓ Media query breakpoints

## 💡 Pro Tips

1. Always test at actual viewport sizes, not just browser resize
2. Design for content breakage, not specific devices
3. Use clamp() instead of fixed media queries when possible
4. Touch targets should be 44x44px minimum (WCAG standard)
5. Hamburger menu is just visual preference; ensure nav works keyboard-only

---

**Created**: 2026 | **Status**: Production Ready ✓
