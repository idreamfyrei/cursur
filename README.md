# Cursor Clone: Landing Page

A static landing page of Cursor using only HTML and CSS. The project is an attempt to learn the flow of landing page and learn HTML and CSS techniques. 

## Overview

This is an attempt to recreate Cursor's marketing website, showcasing an AI powered code editor. The project uses pure HTML and CSS to replicate the landing page. The landing page is not responsive.


##  Project Structure

```
cursur
├── index.html              # HTML structure
├── style.css               # Styling
└── resource/              # Assets folder
|   ├── fonts/             # Font used
|   ├── logos/             # Company logos
|   ├── devs/              # Testimonial avatars
|   └── images and media files
└── README.md              # Documentation
```

##  Getting Started

### Prerequisites
- A modern web browser (Chrome, Firefox, Safari, Edge)
- A local web server 

### Installation


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

   or

   [Live Link](https://cursur.vercel.app/)

## 🎓 Learning Points

This project helped to learn:

### HTML 
- Semantic HTML5 elements (`<nav>`, `<main>`, `<section>`, `<article>`, `<header>`, `<footer>`)
- Proper heading hierarchy (h1-h5)
- Accessible link structure
- Video element with multiple fallbacks
- Meta tags for viewport and charset
- Importing external icons through links

### CSS Techniques
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

### Design Patterns
- Sticky navigation pattern
- Hero section with CTA
- Social proof (brand logos)
- Feature showcase sections
- Testimonial cards
- Changelog timeline
- Footer navigation sitemap
- Theme toggle UI (structure only)


## ⚠️ Known Limitations

- **No JavaScript** - Interactive features like theme toggle and language selector are UI-only
- **Desktop-focused** - Not optimized for devices
- **Static Content** - No dynamic data loading
- **Video Requirement** - Video playback may require a local server
- **External Dependencies** - Relies on Google Fonts for Material Symbols

##  Acknowledgments

- Design inspiration: [Cursor.sh](https://cursor.sh)
- Icons: Google Material Symbols
- Font: Cursor Gothic from Cursor
