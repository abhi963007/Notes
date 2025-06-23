# Programming Notes Learning Platform 🚀

[![Netlify Status](https://api.netlify.com/api/v1/badges/c01bd484-92c9-4659-9620-189f92100c96/deploy-status)](https://app.netlify.com/sites/programmingnotess/deploys)
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)

## 🔗 Live Demo

**[https://programmingnotess.netlify.app/](https://programmingnotess.netlify.app/)**

![Screenshot](https://i.imgur.com/Jf2O7la.png)

## 📝 Project Overview

This project is an exported **Webflow** landing page that has been customized to showcase **48 course cards**, each featuring programming language tutorials with:

- Full visibility course thumbnails
- Interactive hover-lift effects
- Mobile-responsive design
- Category-based filtering system

## 🗂️ Project Structure

```
├─ index.html               # Main page (customized with static cards)
├─ css/                     # Stylesheets
├─ js/                      # JavaScript files
├─ pdf-images/              # 48 course thumbnails
│   ├─ AlgorithmsGrow.png
│   ├─ AndroidGrow.png
│   └─ ...
└─ README.md                # Project documentation
```

## ✨ Key Features

- **Static Course Cards**: 48 pre-rendered course cards replacing dynamic loading
- **Category Tabs**: Filter courses by programming languages, data analytics, web development, etc.
- **Responsive Design**: Optimized for desktop and mobile with custom dropdown navigation
- **Visual Effects**: Smooth hover animations with scale and shadow effects
- **SEO Optimized**: Custom meta tags for better search engine visibility

## 🛠️ Technical Implementation

### Styling Highlights

```css
/* Card hover animation */
.courses-card:hover {
  transform: translateY(-8px) scale(1.02);
  box-shadow: 0 12px 24px rgba(0,0,0,0.15);
}

/* Mobile responsive tabs */
@media screen and (max-width: 767px) {
  .tabs-menu {
    position: relative;
    display: block;
    width: 100%;
    max-width: 300px;
    margin: 0 auto 20px;
    z-index: 1000;
  }
}
```

## 🚀 Running Locally

1. **Clone the repository**:
   ```bash
   git clone https://github.com/yourusername/programming-notes.git
   cd programming-notes
   ```

2. **Start a local server**:
   ```bash
   # Option 1 – Python 3
   python -m http.server 8000
   # then visit http://localhost:8000

   # Option 2 – Node
   npx http-server -p 8000
   ```

## 🎨 Customization Options

- **Replace Images**: Add new images to `pdf-images/` directory
- **Modify Categories**: Edit the tab sections in `index.html`
- **Change Styling**: Update the inline `<style>` blocks or CSS files

## 📄 License

MIT – free to use, modify, and distribute.
