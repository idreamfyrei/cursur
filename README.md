# Cursor Landing Page Recreation

A recreation of the Cursor IDE landing page, showcasing modern web design techniques and responsive layouts using onlt HTML and CSS.

> Few sections changes on 5th Feb, 2026 after the landing page was completed, so there are chances you might notice a difference in images

## Table of Contents

- [Sections Recreated](#sections-recreated)
- [Typography](#typography)
- [Color Palette](#color-palette)
- [Design Features](#design-features)
- [File Structure](#file-structure)
- [Technical Implementation](#technical-implementation)
- [Key Learnings](#key-learnings)
- [Screenshots](#screenshots)

## Deployment
To check the live deployment: click [here](https://cursur.vercel.app/)

## Sections Recreated

### 1. **Navigation Bar**
- Fixed sticky navigation that stays at the top while scrolling
- Dropdown menus for "Features" and "Resources"
- Action buttons: "Sign in" (secondary) and "Download" (primary)
- Hover effects on all interactive elements

### 2. **Hero Section**
- Large, impactful headline emphasizing productivity and AI coding
- Primary CTA button: "Download for macOS"
- Full-width hero image showcasing the product interface
- Generous padding and spacing for visual impact

### 3. **Brand Trust Section**
- Social proof statement: "Trusted every day by millions of professional developers"
- Grid of 8 company logos (Stripe, OpenAI, Linear, Datadog, Nvidia, Figma, Ramp, Adobe)
- Each logo contained in a bordered card with consistent sizing

### 4. **Product Features Section**
Three feature showcases with alternating layouts:

#### "Agent turns ideas into code"
- 1:2 grid layout (text left, image right)
- Description of AI capabilities
- CTA link to learn more

#### "Magically accurate autocomplete"
- 2:1 grid layout (media left, text right)
- Video demonstration with autoplay
- Fallback image for unsupported browsers

#### "Everywhere software gets built"
- 1:2 grid layout (text left, image right)
- Ecosystem integration messaging
- Consistent styling with first card

### 5. **Testimonials Section**
- Section header: "The new way to build software"
- Grid of 6 testimonial cards featuring:
  - Quote from user
  - User name and title
  - Company affiliation

### 6. **Features Grid Section**
- Title: "Stay on the frontier"
- 3-column grid of feature cards
- Each card includes image, description, and CTA link

### 7. **Changelog Section**
- Recent updates and version releases
- Each entry shows:
  - Version number (in pill-style badge)
  - Release date
  - Update title

### 8. **Career Section**
- Large feature card with image
- Company mission statement
- "Join Us" CTA link
- 1:2 grid layout

### 9. **Recent Highlights Section**
- Full-width section with distinct background
- 1:2 grid layout:
  - Left: "Recent highlights" label
  - Right: 3 blog post cards
- Each card shows:
  - Post title
  - Brief description
  - Category and date metadata
- Hover effects on cards
- "View more posts" link

### 10. **Download CTA Section**
- Large, centered section
- Prominent heading: "Try Cursor now."
- Primary download button

### 11. **Footer**
- 5-column grid with navigation links:
  - Product
  - Resources (with external link arrows)
  - Company
  - Legal
  - Connect (social media)
- Footer bottom section:
  - Copyright and SOC 2 certification
  - Theme toggle buttons (desktop, light, dark)
  - Language selector dropdown with 4 languages

---

## Typography

### Primary Font
**CursorGothic** (Custom font loaded via @font-face)
- File: `CursorGothic_Regular.woff2`
- Weight: 400 (Regular)
- Font-style: normal
- Font-display: swap

### Fallback Stack
```css
font-family: "CursorGothic", system-ui, -apple-system, BlinkMacSystemFont, sans-serif;
```

### Font Sizes Used

| Element | Font Size | Line Height | Letter Spacing |
|---------|-----------|-------------|----------------|
| Hero H1 | 34px | 1.25 | -0.015em |
| Download H2 | 4.5rem (72px) | 1.25 | -0.015em |
| Section H3 | 1.375rem (22px) | 1.25 | -0.011em |
| Section H4 | 1rem (16px) | 1.35 | - |
| Navigation | 1.125rem (18px) | 1.5rem | 0.01em |
| Body Text | 1rem-1.375rem | 1.25 | -0.011em |
| Small Text | 0.875rem (14px) | 14px | - |

### Font Weight
- font-weight: 100 (thin/hairline weight)
- font-weight: 400 (normal text)
- font-weight: 500 (Semi-bold text)
- This creates the distinctive, refined aesthetic of the design

---

## Color Palette

### Background Colors
```css
--primary-background-color: #14120b      /* Main dark background */
--secondary-background-color: #1b1913    /* Card backgrounds */
--secondary-background-color-light: #222018  /* Hover states */
--tertiary-background-color: #323c3e     /* Video section background */
--quaternary-background-color: #201e18   /* Highlight cards */
--quaternary-background-color-hover: #46454335  /* Card hover */
```

### Text Colors
```css
--primary-font-color: #f5f2f2            /* Main text - off-white */
--primary-font-color-hover: #bbb6b6      /* Secondary text - gray */
--font-color-action: #f54e00             /* CTA/links - orange */
--font-color-action-hover: #b43e07       /* CTA hover - dark orange */
--secondary-font-color: #14120b          /* Text on light backgrounds */
```

### Border Colors
```css
--border-color: #3f3e38                  /* Primary borders */
--border-color-light: #3f3e3867          /* Subtle borders (with alpha) */
```

### Color Usage

**Primary Orange (#f54e00)**
- All CTA links and actionable text
- Hover states transition to darker orange (#b43e07)
- Used consistently for "Learn more →" links

**Dark Theme**
- Rich, warm dark palette (browns/blacks)
- Creates sophisticated, professional aesthetic
- High contrast for text readability

---

## Design Features

### Interactive Elements

**Hover Effects:**
- Navigation links fade to gray on hover
- Dropdown menus appear with smooth transitions
- Cards elevate with background color changes
- Links show animated arrows (→ or ↗)
- Buttons have subtle opacity/color changes

**Dropdown Menus:**
- Appear on hover with fade-in effect
- Box shadow for depth: `0 10px 40px rgba(0, 0, 0, 0.6)`
- Minimum content width for readability
- Two-column layout for Resources

**Cards:**
- Rounded corners: 8px (consistent throughout)
- 1px borders with semi-transparent color
- Hover states with background color transitions
- Consistent padding and spacing

### Layout Techniques

**Grid Systems:**
- Product sections use CSS Grid with varying ratios:
  - 1:2 ratio for text-left layouts
  - 2:1 ratio for text-right layouts
- Testimonials: 3-column grid
- Features: 3-column grid
- Footer: 5-column grid

**Spacing:**
- Consistent padding: 5.3125rem (85px) horizontal
- Section gaps: 4.1875rem to 7rem vertical
- Card gaps: 0.625rem to 5.625rem
---

## File Structure

```
cursor-landing-page/
├── index.html                  # Main HTML structure
├── style.css                   # All styling and layout
├── resource/
│   ├── fonts/
│   │   └── CursorGothic_Regular.woff2
│   ├── logos/                  # Company logos (SVG)
│   ├── Miscellaneous Media     # Media used on landing page
└── README.md                   # Documentation
```

---

## Key Design Principles

### 1. **Consistency**
- Uniform spacing and rhythm throughout
- Consistent border radius (8px for cards)
- Repeating color palette
- Standard button styles

### 2. **Visual Weight**
- Light font weight (100) creates elegance
- Large headings command attention
- White space provides breathing room

### 3. **User Experience**
- Clear visual hierarchy guides the eye
- Interactive elements have obvious affordances
- Smooth transitions reduce jarring changes
- Logical content flow from hero to CTA

### 4. **Brand Identity**
- Custom CursorGothic font reinforces brand
- Signature orange (#f54e00) for actions
- Dark, sophisticated color scheme
- Clean, modern aesthetic


## Getting Started


1. **Clone or download this repository**
   ```bash
   git clone https://github.com/idreamfyrei/cursur.git
   cd cursur
   ```

2. **Open the project**
   - Simply open `index.html` in your browser, or
   - Use a local server:
     ```bash
     # Node.js (with http-server)
     npx http-server
     ```

3. **View in browser**
   - Navigate to `http://localhost:8000`

   You can use `Live Server` to view index.html on Browser.

---

## Key Learnings

#### HTML 
- Semantic HTML5 elements (`<nav>`, `<main>`, `<section>`, `<article>`, `<header>`, `<footer>`)
- Proper heading hierarchy (h1-h5)
- Accessible link structure
- Video element with multiple fallbacks
- Meta tags for viewport and charset
- Importing external icons through links

#### CSS Techniques
- **CSS Custom Properties (var)** for theme management
- **CSS Grid** for complex two-dimensional layouts
- **Flexbox** for one-dimensional layouts and alignment
- **Position Sticky** for fixed navigation
- **Pseudo-elements** (`::after`) for decorative effects
- **@font-face** for custom typography
- **Grid Template Columns** with fractional units
- **Dropdown**- CSS enabled dropdown menu
- **Text transition on Hover**- Append symbols or text transition on hover
- **calc()**- use of calc in projects

#### Design Patterns
- Sticky navigation pattern
- Hero section with CTA
- Social proof (brand logos)
- Feature showcase sections
- Testimonial cards
- Changelog timeline
- Footer navigation sitemap
- Theme toggle UI 

**Material Symbols:**
Icons are loaded from Google Fonts CDN:
```html
<link href="https://fonts.googleapis.com/css2?family=Material+Symbols+Outlined" rel="stylesheet">
```

**Video Assets:**
The Section3.mp4 video demonstrates the autocomplete feature. It autoplays, is muted, and loops for optimal UX.

**External Links:**
All links use `href="#"` as placeholders. In production, these would link to actual pages.

---


## Screenshots

- Nav and Hero Section
<img width="1470" height="956" alt="Screenshot 2026-02-07 at 11 47 28 AM" src="https://github.com/user-attachments/assets/4aa2b597-8db8-40f8-af3c-a5ac7bc08d69" />

- Hero Section Consumer Organisations
<img width="1470" height="956" alt="Screenshot 2026-02-07 at 11 48 00 AM" src="https://github.com/user-attachments/assets/d79df3bb-1c42-4bf4-b1bb-8add86298fa0" />

- Feature section cards
  <img width="1470" height="956" alt="Screenshot 2026-02-07 at 11 49 42 AM" src="https://github.com/user-attachments/assets/8adec0cd-c2f0-4bb6-912d-cf24fabed18d" />
  <img width="1470" height="956" alt="Screenshot 2026-02-07 at 11 50 14 AM" src="https://github.com/user-attachments/assets/15132ef9-c59c-4510-990e-c50f96d25290" />
  <img width="1470" height="956" alt="Screenshot 2026-02-07 at 11 50 33 AM" src="https://github.com/user-attachments/assets/5fa37c6a-bd40-4e8f-bc19-bb47e8732ec6" />

- Testimonials
  <img width="1470" height="956" alt="Screenshot 2026-02-07 at 11 50 55 AM" src="https://github.com/user-attachments/assets/bb288310-96ed-466e-8570-10dd50558bd6" />

- Features CTA
<img width="1470" height="956" alt="Screenshot 2026-02-07 at 11 51 26 AM" src="https://github.com/user-attachments/assets/fbd540e2-03f8-49dc-b122-35fe61cca124" />

- Changelog and Join us
  <img width="1470" height="956" alt="Screenshot 2026-02-07 at 11 52 24 AM" src="https://github.com/user-attachments/assets/d289b189-0c58-4d9b-9ee6-66afd17187c5" />

- Recent Highlights
  <img width="1470" height="956" alt="Screenshot 2026-02-07 at 11 52 54 AM" src="https://github.com/user-attachments/assets/3e488bea-be87-41f9-9905-32bfdd44dad1" />

- CTA and Footer
  <img width="1470" height="956" alt="Screenshot 2026-02-07 at 11 53 32 AM" src="https://github.com/user-attachments/assets/9b16ab7b-1e8a-4616-8b5a-e99e61acf41a" />

---
##  Acknowledgments

- Design inspiration: [Cursor.com](https://cursor.com/)
- Icons: [Google Material Symbols](https://fonts.google.com/icons)
- Font: Cursor Gothic from Cursor
---



**This is a recreation of the Cursor IDE landing page for educational purposes. Original design by Cursor.**
