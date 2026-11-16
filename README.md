# dūmu aparāti — personal store app

A private, local-first clothing inventory and sales tracker built as a Progressive Web App.

## Features
- Product catalogue with photos, categories, SKU and descriptions
- Size/colour variants with stock, purchase cost and sale price
- Record sales and automatically reduce stock
- Delete a sale and return its quantity to stock
- Expense tracking
- Revenue, gross profit, net profit, stock value and best-seller summaries
- JSON backup export and import
- Installable on iPhone from Safari when hosted over HTTPS

## Run locally
For a quick preview, open `index.html` in a modern browser. For install/offline support, serve it over HTTPS (or localhost).

## Publish free with GitHub Pages
1. Create a GitHub account and a new **public** repository (for example `dumu-aparati`).
2. Upload all files in this folder to the repository root.
3. In the repository, open **Settings → Pages**.
4. Under Build and deployment, choose **Deploy from a branch**, select `main` and `/ (root)`, then Save.
5. Wait for GitHub Pages to publish the site. The address will look like `https://YOUR-USERNAME.github.io/dumu-aparati/`.
6. On your iPhone, open that address in **Safari** → Share → **Add to Home Screen**.

## Important data note
This first version stores data in IndexedDB inside the browser on the device. It does not sync between devices and is not a cloud database. Use **Backup** regularly and keep the downloaded JSON file somewhere safe. If Safari website data is cleared, locally stored records may be lost. The app has no login or multi-user access control, so do not put sensitive customer/payment details into it.

## Notes
- All amounts are EUR.
- Stock is maintained per size/colour variant.
- Product photos are resized before being stored. Keep photos reasonably small.
- Profit calculations use the product's current purchase cost when shown in sales totals; for best accounting accuracy, preserve historical costs if you later change a variant's cost. A future version can store cost snapshots per sale.
