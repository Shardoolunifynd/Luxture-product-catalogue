# Product Catalogue Web App

This is a modern, interactive product catalogue web application built with HTML, JavaScript, and Tailwind CSS. It fetches product data from a Google Sheet (via a published Apps Script web API) and displays it in a searchable, sortable, and paginated table. The app is designed to be mobile-friendly, accessible, and works offline as a Progressive Web App (PWA).

## Features

- **Live Product Data:** Fetches products from a Google Sheet using a public API endpoint.
- **Search & Sort:** Search products by name and sort by price or points.
- **Pagination:** Easily navigate large product lists.
- **Modal Details:** Click a product row to view details in a modal popup.
- **Responsive Design:** Looks great on desktop and mobile.
- **Dark Mode:** Toggle between light and dark themes.
- **Export CSV:** Download the current product list as a CSV file.
- **Offline Support:** Uses a service worker to cache assets and data for offline viewing.
- **Accessibility:** Keyboard navigation and ARIA attributes for better accessibility.
- **PWA Ready:** Includes a manifest and can be installed on mobile devices.

## Files

- `index.html` — Main application UI and logic.
- `service-worker.js` — Service worker for offline/PWA support.
- `manifest.json` — Web app manifest for PWA installability.
- `README.md` — This documentation file.

## How to Use

1. **Open `index.html` in your browser.**
   - The app will fetch product data from the configured Google Sheets API URL.
2. **To enable offline support:**
   - Open the app in your browser and allow the service worker to register.
   - You can then access the app even without an internet connection.
3. **To deploy/share:**
   - Host the files (`index.html`, `service-worker.js`, `manifest.json`) on any static web host (GitHub Pages, Netlify, Vercel, etc.).
   - Share the hosted URL with others.

## Customization

- **Change Data Source:**
  - Update the `SHEET_API_URL` in `index.html` to point to your own Google Sheets Apps Script web app.
- **Branding:**
  - Edit the manifest and HTML for your own icons, colors, and titles.

## Requirements

- Modern web browser (Chrome, Edge, Firefox, Safari)
- Internet connection for first load (offline support after first visit)

## Credits

- [Tailwind CSS](https://tailwindcss.com/) for styling
- Google Sheets for backend data

---

For any issues or feature requests, please contact the project maintainer.
