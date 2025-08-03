# Component Reference Guide

## Quick Component Lookup

### Layout Components

| Component | Class | Purpose | Location |
|-----------|-------|---------|----------|
| Header Container | `.cars` | Top-level header layout | Lines 15-43 |
| Logo Container | `.top-feature .logo` | Logo positioning | Lines 17-20 |
| Brand Title | `.centreone` | Restaurant name display | Lines 21-23 |
| Navigation | `.nav_bar` | Main menu navigation | Lines 24-41 |
| Content Container | `.container` | Main content wrapper | Lines 44-67 |
| Hero Section | `.description` | Landing area with CTA | Lines 50-65 |

### Content Components

| Component | Class | Purpose | Content Type |
|-----------|-------|---------|--------------|
| Features Section | `.one` | Service highlights | Quality, Speed, Taste |
| Menu Header | `.section.one` | Menu title section | "OUR MENU" |
| Menu Items | `.section.two` - `.seven` | Individual burger items | Product showcases |
| Promotional | `.page.one`, `.page.two` | Special offers | Product highlights |
| Footer | `.last.page` | Site navigation & signup | Links & email form |

## CSS Class Reference

### Display Classes
```css
.cars          /* display: flex; padding-right: 30px */
.one           /* display: flex */
```

### Positioning Classes
```css
.top-feature .logo       /* float: left; clear: both */
.container .description .B   /* float: right; clear: both; height: 600px */
```

### Styling Classes
```css
.top-feature .centreone h2 > span   /* color: goldenrod */
.container .description .B          /* background-color: orange */
.cars .nav_bar table               /* text-indent: 80px */
.container .description .specialone /* margin-top: 70px */
```

## Component Templates

### Standard Menu Item Template
```html
<div class="section [number]">
    <img src="./assets/SeekPng [X].png" height="60px" alt="[Product Name]">
    <h1>[Product Title]</h1>
    <p>[Product Description]</p>
</div>
```

### Feature Section Template
```html
<div class="[feature-class]">
    <h1 class="[styling-class]">[Feature Title]</h1>
    <p>[Feature Description]</p>
</div>
```

### Navigation Item Template
```html
<th>[Menu Item Name]</th>
```

### Image Container Template
```html
<div class="image [number]">
    <img src="./assets/[image-name].png" alt="[Description]">
</div>
```

## Image Asset Specifications

### Required Image Formats
- **Logo**: PNG format, appropriate for header display
- **Menu Items**: PNG format, 60px height recommended
- **Hero Images**: Large format PNG, 600px+ height
- **Promotional**: PNG format, variable sizes

### Image Naming Convention
- Menu items: `SeekPng [number].png`
- Promotional: `double-check[number].png`
- Mobile apps: `mobile[number].png`
- Hero: `[CITYPNG 1.png`

## Form Component Specifications

### Email Input (Current Implementation)
```html
<input type="enter your email">
```

### Email Input (Recommended Implementation)
```html
<input type="email" placeholder="Enter your email" required>
<button type="submit">Subscribe</button>
```

### Button Components
```html
<!-- Primary CTA -->
<button>Order now.</button>

<!-- Form Submit -->
<button type="submit">[Action Text]</button>
```

## Responsive Design Considerations

### Mobile-First Approach
```css
/* Base styles for mobile */
.cars {
    display: flex;
    flex-direction: column; /* Stack on mobile */
}

/* Tablet and up */
@media (min-width: 768px) {
    .cars {
        flex-direction: row; /* Side by side on larger screens */
    }
}
```

### Image Responsiveness
```css
.container .description .B {
    max-width: 100%;
    height: auto; /* Maintain aspect ratio */
}
```

## Accessibility Implementation

### Alt Text Standards
```html
<!-- Good -->
<img src="./assets/logo.png" alt="Burger Restaurant Logo">
<img src="./assets/SeekPng 2.png" alt="Double Cheeseburger with Fries">

<!-- Current (Needs Improvement) -->
<img src="./assets/logo.png" alt="">
```

### Semantic HTML Structure
```html
<!-- Recommended Navigation -->
<nav class="nav_bar">
    <ul>
        <li><a href="#home">Home</a></li>
        <li><a href="#offers">Offers</a></li>
        <li><a href="#contact">Contact</a></li>
        <li><a href="#about">About</a></li>
    </ul>
</nav>

<!-- Current Implementation -->
<div class="nav_bar">
    <table>
        <tr>
            <th>Home</th>
            <th>offers</th>
            <th>Contact</th>
            <th>About</th>
        </tr>
    </table>
</div>
```

### Form Labels
```html
<!-- Recommended -->
<label for="email">Subscribe to our newsletter:</label>
<input type="email" id="email" placeholder="Enter your email" required>

<!-- Current -->
<h2>subscribe to our page</h2>
<input type="enter your email">
```

## Browser Support Matrix

| Feature | IE11 | Edge | Chrome | Firefox | Safari |
|---------|------|------|--------|---------|--------|
| Flexbox | ✓ | ✓ | ✓ | ✓ | ✓ |
| CSS3 Properties | Partial | ✓ | ✓ | ✓ | ✓ |
| FontAwesome | ✓ | ✓ | ✓ | ✓ | ✓ |

## Performance Optimization Checklist

### Image Optimization
- [ ] Convert large PNGs to WebP format
- [ ] Implement lazy loading for below-fold images
- [ ] Add responsive image sizes
- [ ] Compress images without quality loss

### CSS Optimization
- [ ] Minify CSS for production
- [ ] Remove unused CSS rules
- [ ] Optimize font loading
- [ ] Use CSS sprites for small icons

### HTML Optimization
- [ ] Validate HTML markup
- [ ] Optimize heading hierarchy
- [ ] Add proper meta tags
- [ ] Implement structured data

## Component Extension Examples

### Adding a New Menu Category
```html
<div class="section eight">
    <img src="./assets/SeekPng 7.png" height="60px" alt="Chicken Burger">
    <h1>Chicken Deluxe</h1>
    <p>Grilled chicken breast with fresh lettuce, tomatoes, and our special sauce.</p>
</div>
```

### Creating a Special Offers Section
```html
<div class="offers-section">
    <h2 class="C">Special Offers</h2>
    <div class="offer-item">
        <h3>Weekend Special</h3>
        <p>Buy 2 burgers, get 1 free drink!</p>
        <button>Claim Offer</button>
    </div>
</div>
```

### Adding Social Media Links
```html
<div class="social-links">
    <h3>Follow Us</h3>
    <a href="#" aria-label="Facebook"><i class="fab fa-facebook"></i></a>
    <a href="#" aria-label="Twitter"><i class="fab fa-twitter"></i></a>
    <a href="#" aria-label="Instagram"><i class="fab fa-instagram"></i></a>
</div>
```

## Troubleshooting Common Issues

### Image Not Loading
1. Check file path: `./assets/` vs `/assets/`
2. Verify image exists in assets folder
3. Check file permissions
4. Validate image format

### Layout Breaking
1. Validate CSS syntax
2. Check for unclosed HTML tags
3. Verify class names match CSS
4. Test flexbox support

### Form Not Working
1. Add proper `action` and `method` attributes
2. Include form validation
3. Add server-side processing
4. Test input types

This component reference provides quick access to all structural elements and implementation patterns used throughout the burger restaurant website.