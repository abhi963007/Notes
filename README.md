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
- PDF downloads for each programming language
- **NEW**: Detailed course pages with PDF preview functionality

## 🗂️ Project Structure

```
├─ index.html               # Main page (customized with static cards)
├─ python-detail.html       # Python course detail page with PDF preview
├─ javascript-detail.html   # JavaScript course detail page with PDF preview
├─ detail-template.html     # Template for creating new detail pages
├─ how-to-create-detail-pages.html # Guide for creating detail pages
├─ troubleshooting.html     # Troubleshooting guide for link redirections
├─ create-detail-pages.bat  # Batch script to create detail pages for all courses
├─ create-detail-pages.html # Detailed guide for creating detail pages
├─ update-index-links.js    # Node.js script to update index.html links
├─ update-index-links.html  # Guide for updating index.html links
├─ css/                     # Stylesheets
├─ js/                      # JavaScript files
├─ pdf/                     # PDF files for downloading
│   ├─ AlgorithmsNotesForProfessionals.pdf.pdf
│   ├─ AndroidNotesForProfessionals.pdf.pdf
│   └─ ...
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
- **PDF Downloads**: Each card links to a downloadable PDF resource
- **SEO Optimized**: Custom meta tags for better search engine visibility
- **NEW - Detail Pages**: Course detail pages with PDF preview functionality
- **NEW - PDF Preview**: Embedded PDF viewer for previewing content before downloading

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

### PDF Preview Implementation

The detail pages include an embedded PDF viewer using iframe:

```html
<div class="pdf-preview-container">
  <iframe src="pdf/PythonNotesForProfessionals.pdf.pdf" width="100%" height="600px"></iframe>
</div>
```

## 📄 PDF Files Structure

The project includes a collection of programming language PDF guides that can be downloaded directly from the website. Each PDF follows a specific naming convention:

- Format: `[LanguageName]NotesForProfessionals.pdf.pdf` 
- Example: `PythonNotesForProfessionals.pdf.pdf`

**Note**: These PDFs must be placed in the `/pdf` directory for the download functionality to work correctly.

## 🔄 Detail Pages

The project now includes detailed course pages with PDF preview functionality:

- **Python Detail Page**: Preview and download Python PDF notes
- **JavaScript Detail Page**: Preview and download JavaScript PDF notes
- **Detail Template**: Use this template to create additional detail pages
- **How-to Guide**: Step-by-step instructions for creating new detail pages
- **Troubleshooting**: Solutions for common issues with detail page redirections

### Creating Detail Pages for All Courses

To create detail pages for all courses, you can use the provided tools:

1. **Batch Script Method**:
   - Run `create-detail-pages.bat` to create basic detail page copies
   - Edit each generated file to replace Python-specific content

2. **Manual Method**:
   - Follow the instructions in `create-detail-pages.html`
   - Copy `python-detail.html` as a template for each course
   - Update course name, description, category, and PDF paths

3. **Updating Index Links**:
   - Use `update-index-links.js` Node.js script to automatically update all links
   - Or follow the manual instructions in `update-index-links.html`

## 🚀 Running Locally

1. **Clone the repository**:
   ```bash
   git clone https://github.com/yourusername/programming-notes.git
   cd programming-notes
   ```

2. **Ensure PDF files are present**:
   Make sure all the required PDF files are in the `/pdf` directory with the correct naming format.

3. **Start a local server**:
   ```bash
   # Option 1 – Python 3
   python -m http.server 8000
   # then visit http://localhost:8000

   # Option 2 – Node
   npx http-server -p 8000
   ```

4. **Important**: For PDF preview to work correctly, you must use a local server rather than opening HTML files directly.

## 🎨 Customization Options

- **Replace Images**: Add new images to `pdf-images/` directory
- **Modify Categories**: Edit the tab sections in `index.html`
- **Change Styling**: Update the inline `<style>` blocks or CSS files
- **Update PDFs**: Replace PDF files in the `pdf/` directory (maintain the naming convention)
- **Add Detail Pages**: Use the template to create more detailed course pages

## 🔧 Troubleshooting

If you encounter issues with links not redirecting to detail pages:

1. Clear your browser cache
2. Perform a hard refresh (Ctrl+F5 or Cmd+Shift+R)
3. Check the HTML links in index.html
4. Verify the JavaScript redirection code is present
5. See `troubleshooting.html` for detailed solutions

## 📄 License

MIT – free to use, modify, and distribute.
