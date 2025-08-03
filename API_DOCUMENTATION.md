# Burger Restaurant Website - API Documentation

## Table of Contents
1. [HTML Structure Components](#html-structure-components)
2. [CSS Classes and Styling API](#css-classes-and-styling-api)
3. [Navigation Components](#navigation-components)
4. [Content Sections](#content-sections)
5. [Image Assets](#image-assets)
6. [Form Elements](#form-elements)
7. [Usage Examples](#usage-examples)

## HTML Structure Components

### Header Section (`<head>`)
**Description**: Contains meta information and external resources
**Location**: Lines 4-12 in `index.html`

```html
<head>
    <meta charset="UTF-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Burgers</title>
    <link rel="stylesheet" href="style.css">
    <link rel="stylesheet" href="https://pro.fontawesome.com/releases/v5.10.0/css/all.css">
</head>
```

**Dependencies**:
- `style.css` - Local stylesheet
- FontAwesome Pro 5.10.0 - Icon library

---

### Main Container (`div.cars`)
**Description**: Top-level container for header navigation and branding
**Location**: Lines 15-43 in `index.html`
**CSS Class**: `.cars`

```html
<div class="cars">
    <div class="top-feature">
        <div class="logo">
            <img src="/assets/logo.png" alt="">
        </div>
        <div class="centreone">
            <h2>Bur<span>ger</span></h2>
        </div>
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
    </div>
</div>
```

**Child Components**:
- `div.top-feature` - Header wrapper
- `div.logo` - Logo container
- `div.centreone` - Brand title
- `div.nav_bar` - Navigation menu

---

### Content Container (`div.container`)
**Description**: Main content area with hero section
**Location**: Lines 44-67 in `index.html`
**CSS Class**: `.container`

```html
<div class="container">
    <div class="description">
        <div>
            <img class="B" src="./assets/[CITYPNG 1.png" alt="">
        </div>
        <div class="specialone">
            <h1>Rain or shine,</h1>
            <h1>its time to dine</h1>
            <p>We cook & deliver the tastiest burgers</p>
            <p>right away to your designated location.</p>
            <button>Order now.</button>
        </div>
    </div>
</div>
```

**Child Components**:
- `div.description` - Hero section wrapper
- `img.B` - Hero image
- `div.specialone` - Hero text content
- `button` - Call-to-action button

---

## CSS Classes and Styling API

### Layout Classes

#### `.cars`
**Purpose**: Flexbox container for header layout
**Properties**:
- `display: flex`
- `margin-left: 0px`
- `padding-right: 30px`

**Usage Example**:
```html
<div class="cars">
    <!-- Header content -->
</div>
```

#### `.top-feature .logo`
**Purpose**: Logo positioning
**Properties**:
- `float: left`
- `clear: both`

#### `.top-feature .centreone h2 > span`
**Purpose**: Brand name accent color
**Properties**:
- `color: goldenrod`

**Usage Example**:
```html
<div class="centreone">
    <h2>Bur<span>ger</span></h2>
</div>
```

#### `.cars .nav_bar table`
**Purpose**: Navigation menu spacing
**Properties**:
- `text-indent: 80px`

#### `.one`
**Purpose**: Flexbox layout for sections
**Properties**:
- `display: flex`

#### `.container .description .B`
**Purpose**: Hero image styling
**Properties**:
- `height: 600px`
- `float: right`
- `clear: both`
- `background-color: orange`

#### `.container .description .specialone`
**Purpose**: Hero text positioning
**Properties**:
- `margin-top: 70px`

---

## Navigation Components

### Primary Navigation (`div.nav_bar`)
**Description**: Main website navigation menu
**Structure**: Table-based layout
**Menu Items**:
- Home
- Offers  
- Contact
- About

**Implementation**:
```html
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

### Footer Navigation (`div.last.page`)
**Description**: Secondary navigation in footer
**Location**: Lines 170-185

**Menu Items**:
- Home
- Services
- About
- Contact

**Implementation**:
```html
<div class="last page">
    <h2>Sitemap</h2>
    <ul>
        <li>Home</li>
        <li>services</li>
        <li>About</li>
        <li>Contact</li>
    </ul>
</div>
```

---

## Content Sections

### Hero Section
**Class**: `div.description`
**Purpose**: Main landing area with call-to-action
**Components**:
- Hero image (`img.B`)
- Headline text
- Description paragraphs
- Order button

### Features Section
**Classes**: `div.one`, `div.C`, `div.special`
**Purpose**: Highlight key restaurant features
**Features**:
- Quality Burgers
- Fast Delivery  
- Delicious Meals

### Menu Section
**Purpose**: Display burger menu items
**Sections**:
- `div.section.one` - Menu header
- `div.section.two` through `div.section.seven` - Menu items

**Menu Item Structure**:
```html
<div class="section [number]">
    <img src="./assets/SeekPng [number].png" height="60px" alt="">
    <h1>Double Burger</h1>
    <p>Lorem ipsum description...</p>
</div>
```

### Promotional Sections
**Classes**: `div.page.one`, `div.page.two`
**Content**:
- "The Double Decker" promotion
- Mobile app promotion

---

## Image Assets

### Logo
**File**: `/assets/logo.png`
**Usage**: Header logo
**Dimensions**: Standard logo size
**Format**: PNG

### Hero Image
**File**: `./assets/[CITYPNG 1.png`
**Usage**: Main hero section background
**Class**: `.B`
**Styling**: `height: 600px`, orange background

### Menu Item Images
**Files**: `SeekPng 2.png` through `SeekPng 6.png`
**Usage**: Menu item illustrations
**Dimensions**: `height="60px"`
**Format**: PNG

### Promotional Images
**Files**:
- `double-check1.png`, `double-check2.png` - Product showcase
- `mobile1.png`, `mobile2.png` - Mobile app promotion

---

## Form Elements

### Email Subscription
**Location**: Footer section (`div.email`)
**Purpose**: Newsletter signup

**Implementation**:
```html
<div class="email">
    <h2>subscribe to our page</h2>
    <input type="enter your email">
</div>
```

**Note**: Input type should be corrected to `type="email"` for proper functionality.

### Order Button
**Location**: Hero section
**Purpose**: Primary call-to-action

**Implementation**:
```html
<button>Order now.</button>
```

---

## Usage Examples

### Creating a New Menu Item
```html
<div class="section eight">
    <img src="./assets/new-burger.png" height="60px" alt="New Burger">
    <h1>New Burger Name</h1>
    <p>Description of the new burger item...</p>
</div>
```

### Adding a Feature Section
```html
<div class="feature-section">
    <h1 class="C">New Feature</h1>
    <p>Feature description text...</p>
</div>
```

### Implementing Proper Email Input
```html
<div class="email">
    <h2>subscribe to our page</h2>
    <input type="email" placeholder="Enter your email" required>
    <button type="submit">Subscribe</button>
</div>
```

---

## Accessibility Recommendations

1. **Alt Text**: Add descriptive alt text to all images
2. **Semantic HTML**: Use proper heading hierarchy (h1 > h2 > h3)
3. **Navigation**: Implement proper navigation with `<nav>` elements
4. **Forms**: Add proper labels and validation to form inputs
5. **Focus Management**: Ensure keyboard navigation works properly

---

## Browser Compatibility

**Supported Features**:
- Flexbox layout (IE10+)
- CSS3 properties
- HTML5 semantic elements

**External Dependencies**:
- FontAwesome Pro 5.10.0 (requires license)

---

## Performance Considerations

1. **Image Optimization**: Large PNG files should be optimized or converted to WebP
2. **CSS Minification**: Minify CSS for production
3. **Asset Loading**: Consider lazy loading for images
4. **CDN**: Use CDN for FontAwesome instead of Pro version if license allows

---

This documentation covers all public components, styling APIs, and structural elements of the burger restaurant website. For implementation details or modifications, refer to the specific line numbers provided in each section.