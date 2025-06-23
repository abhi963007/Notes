# Course Cards Demo

This project is an exported **Webflow** landing page that has been customized to showcase **48 course cards**, each displaying a unique local image with full visibility and an interactive hover-lift effect.

## Contents

```
├─ index.html               # Main page (edited)
├─ pdf-images/              # 48 local course thumbnails (png / webp)
│   ├─ 01_Grow.png
│   ├─ 02_Grow.png
│   └─ ...
└─ README.md                # You are here
```

### Key Customizations

* **JavaScript** dynamically clones the default 6 Webflow cards up to 48 and assigns images sequentially from `pdf-images`.
* **CSS** guarantees every image is fully visible (`object-fit: contain`) and gives each card a smooth hover animation (`translateY + scale + shadow`).
* Hero buttons, footer buttons, and several non-essential sections were hidden / removed to simplify the demo.

## Running Locally

1. **Clone / copy** this folder to your machine (everything is self-contained).
2. Open `index.html` directly in a modern browser **or** start a tiny web server:

   ```bash
   # Option 1 – Python 3
   python -m http.server 8000
   # then visit http://localhost:8000

   # Option 2 – Node (npm install -g http-server)
   http-server -p 8000
   ```

> A local server is recommended if you run into any CORS or path issues.

## Customisation

* **Replace Images**: Drop new files into `pdf-images/` and keep exactly 48. Names can be anything; the script picks them up in directory order.
* **Adjust Hover Style**: Edit the inline `<style>` block near the top of `index.html`, lines containing `.courses-card:hover`.
* **Change Card Count**: In the same JS block (`window.onload` handler) change the value `desiredTotal = 48`.

## Dependencies

None – everything is plain HTML/CSS/JS.  No build step required.

## License

MIT – free to use, modify, and distribute.
