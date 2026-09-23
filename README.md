# Vortex Business Management System — FULL CODE

This folder contains the complete frontend source code for a GitHub Pages test build.

## Files

- `index.html` — complete HTML entry point
- `styles.css` — complete responsive user interface styling
- `app.js` — complete application logic
- `README.md` — setup instructions
- `.nojekyll` — GitHub Pages helper

## Features implemented

### Business account
- Create business account
- Shop/business name
- Owner name
- Phone
- Password
- Confirm password
- Login using shop name + password
- Show/hide password

### Inventory
- Products
- Barcode / QR identifier
- SKU
- Buying price
- Selling price
- Quantity
- Minimum stock
- Branch
- Low-stock status
- New stock receiving
- Dead-stock calculation

### Scanner
- Phone-camera barcode/QR scanning
- Product lookup
- Create a product from an unknown scanned code
- Add scanned product directly to a sale

### POS
- Barcode/QR product lookup
- Shopping cart
- Quantity controls
- Customer selection
- Payment method
- Automatic stock deduction
- Sale record
- Receipt generation

### Printing
- Sales receipts
- Daily sales report
- Monthly sales report
- Yearly sales report
- All sales report
- Current inventory report
- Dead-stock report
- Stock-transfer report
- Stock-transfer receipt

### Business management
- Customers
- Suppliers
- Purchases/new stock
- Branches
- Employees
- Expenses
- Activity log

## How to upload to GitHub

Upload these files to the ROOT of your GitHub repository:

```text
index.html
styles.css
app.js
README.md
.nojekyll
```

Do not put `index.html` inside another folder.

Then:

1. Open GitHub repository Settings.
2. Open Pages.
3. Under Build and deployment select `Deploy from a branch`.
4. Select branch `main`.
5. Select `/ (root)`.
6. Save.
7. Wait for GitHub Pages to publish.

## Camera scanner requirement

The camera scanner normally requires a secure context. GitHub Pages uses HTTPS, so the published website is suitable for camera testing. The browser will ask for camera permission.

## Important production warning

This is a complete frontend testing application, but it is NOT a secure production backend.

For production:
- Do not store passwords in localStorage.
- Use Supabase Auth or another secure authentication provider.
- Use a real database.
- Add row-level tenant security.
- Store every business record with a business/tenant ID.
- Add employee roles and permissions.
- Validate all transactions on the server.
- Generate secure receipt/report IDs server-side.
- Protect administrative functions.
- Add server-side audit logs.

The GitHub Pages version intentionally uses localStorage so it can run without a backend while you test the entire user interface and business workflow.
