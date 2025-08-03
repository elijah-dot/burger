# Burger Restaurant Website

##### Elijah Mwangi Wangu

## Project Overview

A modern, responsive website for a burger restaurant featuring an attractive landing page, menu showcase, and customer engagement features. The site emphasizes visual appeal with high-quality images and a clean, user-friendly interface.

## 📚 Documentation

- **[API Documentation](API_DOCUMENTATION.md)** - Comprehensive guide to all HTML components, CSS classes, and functionality
- **[Component Reference](COMPONENT_REFERENCE.md)** - Quick reference guide for developers with templates and examples

## 🌟 Features

- **Responsive Design**: Optimized for smartphones, tablets, desktops, and laptops
- **Visual Menu**: Interactive burger menu with high-quality product images
- **Hero Section**: Eye-catching landing area with call-to-action
- **Brand Identity**: Professional logo and consistent styling
- **Contact Integration**: Email subscription and contact information
- **Mobile App Promotion**: Dedicated section for mobile applications

## 🏗️ Project Structure

```
burger/
├── index.html              # Main HTML file with complete website structure
├── style.css               # Stylesheet with component-specific styling
├── README.md               # Project documentation (this file)
├── API_DOCUMENTATION.md    # Comprehensive API and component documentation
├── COMPONENT_REFERENCE.md  # Quick reference guide for developers
└── assets/                 # Image assets and media files
    ├── logo.png           # Restaurant logo
    ├── [CITYPNG 1.png     # Hero section background image
    ├── SeekPng 2.png      # Burger menu item images
    ├── SeekPng 3.png      # (SeekPng 2-6 for different menu items)
    ├── SeekPng 4.png
    ├── SeekPng 5.png
    ├── SeekPng 6.png
    ├── double-check1.png  # Promotional product images
    ├── double-check2.png
    ├── mobile1.png        # Mobile app promotional images
    └── mobile2.png
```

## 🚀 Quick Start

### Installation Requirements

- Any modern computing device (smartphones, tablets, desktops, laptops)
- Internet connection for FontAwesome icons
- Web browser with HTML5 and CSS3 support

### Running the Website

1. Clone or download the project files
2. Ensure all files maintain the directory structure shown above
3. Open `index.html` in any modern web browser
4. The website will load with full functionality

### For Development

```bash
# Navigate to project directory
cd burger/

# Open with live server (if using VS Code Live Server extension)
# Right-click index.html -> "Open with Live Server"

# Or simply open in browser
open index.html  # macOS
start index.html # Windows
xdg-open index.html # Linux
```

## 🎨 Design System

### Color Palette
- **Primary Accent**: Goldenrod (`color: goldenrod`)
- **Hero Background**: Orange (`background-color: orange`)
- **Text**: Default black/dark colors

### Typography
- **Headers**: Various sizes (h1, h2) for hierarchy
- **Body Text**: Standard paragraph styling
- **Brand Name**: Special styling with accent color on "ger" in "Burger"

### Layout System
- **Flexbox**: Primary layout method for responsive design
- **Float-based**: Secondary positioning for specific elements
- **Table Layout**: Navigation menu structure

## 📱 Component Overview

### Header Components
- **Logo Container**: Restaurant branding
- **Navigation Bar**: Main site navigation (Home, Offers, Contact, About)
- **Brand Title**: "Burger" with styled accent

### Content Sections
- **Hero Section**: Main landing area with call-to-action
- **Features**: Quality Burgers, Fast Delivery, Delicious Meals
- **Menu Showcase**: Visual display of burger options
- **Promotional Areas**: Special offers and mobile app promotion
- **Footer**: Site navigation and email subscription

### Interactive Elements
- **Order Button**: Primary call-to-action in hero section
- **Email Subscription**: Newsletter signup form
- **Navigation Links**: Main menu navigation

## 🔧 Technology Stack

- **HTML5**: Semantic markup and structure
- **CSS3**: Modern styling with flexbox and responsive design
- **FontAwesome Pro 5.10.0**: Icon library for enhanced UI
- **Image Assets**: PNG format for high-quality visuals

## 🌐 Browser Compatibility

| Browser | Version | Support Level |
|---------|---------|---------------|
| Chrome | 60+ | Full Support |
| Firefox | 55+ | Full Support |
| Safari | 12+ | Full Support |
| Edge | 79+ | Full Support |
| IE | 11 | Partial Support |

## 📈 Performance Considerations

### Current Performance
- **Image Assets**: Large PNG files may impact loading times
- **External Dependencies**: FontAwesome Pro CDN dependency

### Optimization Recommendations
- Convert large images to WebP format
- Implement image lazy loading
- Minify CSS for production
- Add responsive image sizes
- Consider local font hosting

## 🔍 SEO Features

- **Meta Tags**: Proper viewport and compatibility meta tags
- **Semantic HTML**: Structured content for search engines
- **Image Alt Text**: Placeholder for accessibility (needs improvement)
- **Page Title**: Descriptive title for search results

## ♿ Accessibility Status

### Current Implementation
- Basic HTML structure
- Image placeholders (alt attributes empty)

### Recommendations for Improvement
- Add descriptive alt text to all images
- Implement proper form labels
- Use semantic HTML5 elements (`<nav>`, `<main>`, `<section>`)
- Add keyboard navigation support
- Ensure proper color contrast ratios

## 🔧 Development Guidelines

### Adding New Menu Items
```html
<div class="section [number]">
    <img src="./assets/SeekPng [X].png" height="60px" alt="[Product Name]">
    <h1>[Product Title]</h1>
    <p>[Product Description]</p>
</div>
```

### Extending Navigation
```html
<th>[New Menu Item]</th>
```

### Creating New Sections
```html
<div class="[section-class]">
    <h1 class="[styling-class]">[Section Title]</h1>
    <p>[Section Content]</p>
</div>
```

## 📝 Contributing

1. Follow the existing HTML structure and CSS class naming conventions
2. Maintain responsive design principles
3. Add proper alt text to new images
4. Test across multiple browsers and devices
5. Update documentation when adding new components

## 📄 License

MIT License

Copyright (c) [2022] [Elijah Mwangi]

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all
copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
SOFTWARE.

## 👨‍💻 Author Information

**Elijah Mwangi**  
Email: [elijahwangu91@gmail.com](mailto:elijahwangu91@gmail.com)

---

For detailed technical documentation, please refer to:
- [API Documentation](API_DOCUMENTATION.md) for comprehensive component details
- [Component Reference](COMPONENT_REFERENCE.md) for quick development reference
