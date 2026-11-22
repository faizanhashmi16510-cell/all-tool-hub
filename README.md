# AllToolsHub — Complete browser-based project

## Included
- Responsive homepage, search, category filters, light/dark mode
- 50 tool interfaces and client-side implementations
- PDF merge, page extraction/split, page count/metadata, PDF-to-PNG rendering, image-to-PDF
- QR code creation and PNG download
- Image resize, compression, crop and format conversion
- Text, calculator, developer, SEO, converter, color, writing and everyday utilities
- Minimal footer exactly: `© 2026 AllToolsHub`

## Browser libraries
PDF tools use PDF-Lib and PDF.js; QR generation uses QRCode.js. These libraries load from public CDNs, so the first load of PDF/QR tools requires an internet connection. The actual processing runs locally in the browser; files are not uploaded to an AllToolsHub server. All other basic tools are implemented in local JavaScript.

## Test locally
Open `index.html` in a modern browser. If the browser restricts local file APIs, run a static server in this directory (for example `python -m http.server 8000`) and open `http://localhost:8000`.

## Deploy free with Cloudflare Pages
1. Create a GitHub repository named `alltoolshub`.
2. Upload the contents of this folder to the repository root (not the ZIP itself).
3. In Cloudflare dashboard, open **Workers & Pages → Create application → Pages → Connect to Git**.
4. Choose the repository.
5. Framework preset: **None**. Build command: leave blank. Build output directory: `/`.
6. Deploy. Cloudflare assigns a free `*.pages.dev` address.
7. Future pushes to GitHub will redeploy automatically.

No paid hosting or database is required for this static project. A custom domain is optional and generally costs money.

## Before public launch
- Test all tools in current Chrome, Firefox, Safari and mobile browsers.
- Update Privacy/Terms content if you add analytics, ads, cookies or other services.
- Add real contact details if you publish contact information.
- AdSense approval and income are not guaranteed; comply with Google's publisher policies.
