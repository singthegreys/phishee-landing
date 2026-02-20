## Phishee Landing Page

This repository contains a simple static landing site for Phishee, built as plain HTML that pulls in Tailwind CSS from a CDN.

### Prerequisites

- **Browser**: Any modern browser (Chrome, Edge, Firefox, Safari).
- **Optional (for running a local server)**:
  - **Python 3** (comes preinstalled on most macOS machines), or
  - **Node.js** (if you prefer using an npm-based static server).

### Option 1 – Open directly in the browser

1. Clone or download this repository to your machine.
2. In Finder or your file explorer, open the project folder.
3. Double-click `index.html` to open it in your browser.
4. Use the navigation in the header to access:
   - `glossary.html` (Cybersecurity 101 for HR)
   - `request-access.html` (Request Early Access form)

This is the quickest way to preview the site; all assets (like Tailwind) are loaded via CDN.

### Option 2 – Run a simple local server (recommended)

Running a local HTTP server avoids issues some browsers have with local file URLs and makes the site behave more like a real deployment.

#### Using Python 3

From the project root (`phishee-landing`):

```bash
cd /Users/paulaauchterlonie/Desktop/Phishee/phishee-landing  # or your cloned path
python3 -m http.server 8000
```

Then open `http://localhost:8000/index.html` in your browser.

#### Using Node.js (npx serve)

If you have Node.js installed:

```bash
cd /Users/paulaauchterlonie/Desktop/Phishee/phishee-landing  # or your cloned path
npx serve .
```

Then open the URL printed in the terminal (typically `http://localhost:3000` or similar) and navigate to `index.html`.

### Files in this project

- **`index.html`**: Main landing page.
- **`glossary.html`**: Cybersecurity 101 for HR glossary/flashcard page.
- **`request-access.html`**: Simple early access request form.
- **`logo.png`**: Logo used in the navigation and forms (make sure this file exists alongside the HTML files).

### Deployment

Because this is a static site, you can deploy it to any static hosting service (e.g. GitHub Pages, Netlify, Vercel, S3 + CloudFront) by uploading these files as-is.

