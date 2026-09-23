# Vortex Business Management System — GitHub Pages Test

This is a frontend-only prototype designed to run on GitHub Pages.

## Included

- Business registration
- Business-name + password login
- Password confirmation during registration
- Dashboard
- Products and stock
- Barcode/QR camera scanner
- Product lookup by scanned code
- Point-of-sale sales flow
- Automatic stock reduction after a completed sale
- Receipt generation and browser printing
- Daily, monthly and yearly sales reports
- Stock-transfer records and printable transfer report
- Customers
- Branches
- Activity log
- Local browser persistence with localStorage

## Important

This version is a **testing prototype only**. Because GitHub Pages is static hosting, there is no secure server/database/authentication layer in this version. Business passwords and data are stored in the browser's localStorage.

For production, replace the demo authentication/database with Supabase or another secure backend. Passwords must never be stored as plain text.

## GitHub Pages

1. Create a GitHub repository.
2. Upload `index.html`, `styles.css`, `app.js`, and `README.md`.
3. Push to the default branch.
4. Open repository Settings → Pages.
5. Select GitHub Actions or Deploy from branch according to your repository setup.
6. Open the generated HTTPS Pages URL.
7. Camera scanning requires a secure context such as HTTPS and browser camera permission.

The scanner libraries are loaded from public CDNs. For a fully self-contained deployment, download/pin the libraries and serve them locally.
