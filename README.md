# Rawleaf static store

## Preview on your computer
1. Extract the ZIP into a folder.
2. Double-click `index.html` to open it in Chrome, Edge or Firefox.
3. Keep `css`, `js` and `images` next to the HTML files. No installation, npm or build step is needed.
4. Add a product, open Bag, change quantities, refresh, and complete the checkout form. The final button opens WhatsApp; the customer must send the draft there.

Google Fonts need internet access; system fonts work offline. WhatsApp and UPI apps also need an internet connection/app support. Browser privacy settings can restrict localStorage. For reliable cart storage across pages, test the final hosted site too; local-file storage behavior differs between browsers.

## Edit the store
- Products and prices: `js/products.js`. Replace `images/product-1.jpg` through `product-7.jpg` with real images, and update image descriptions.
- Colours, fonts and responsive layout: `css/style.css`.
- UPI and WhatsApp configuration: constants near the top of `js/main.js`. Contact numbers also appear in HTML pages.
- Homepage copy and static page content: the corresponding `.html` file.
- Offers: set `OFFER_TEXT` and add approved entries to `DISCOUNTS` in products.js. Example: `{ code: 'YOURCODE', percent: 5 }`. No code is enabled by default.
- Reviews: add genuine entries to `REVIEWS` with `name` and `text`.
- Bundles: add entries to `BUNDLES` with `id`, `name`, `description`, `productIds`. Bundles use the sum of individual prices; add a real discount code separately if appropriate.

## Before accepting live orders
Replace product photo placeholders. Add verified ingredients and label directions. Confirm product spelling, approved claims, shipping charges, delivery coverage, return/COD terms and real offers. The prices currently represent product totals only; shipping is confirmed on WhatsApp.

The QR panel is an explicitly labelled, non-scannable placeholder. To use a real QR, obtain the merchant payment QR for `7003185197-2@okbizaxis`, save it in images, and replace the `.qr-placeholder` element in main.js with an `<img>` using descriptive alt text. Copy UPI ID and the UPI app link work without that image. Confirm the final total before payment. This site cannot automatically verify UPI payments or store orders in a central database.

## Static hosting
Upload all extracted files to the root of your GitHub repository, then enable GitHub Pages or connect the repository to your static host. No build command is needed. Connect www.rawleafs.in following the host's domain instructions. Update canonical and Open Graph URLs if using a different domain. No deployment has been performed as part of this delivery.

Every HTML page has a unique title, description, canonical URL and Open Graph title/description. Product and concern pages update their metadata in the browser from the URL parameters. Social crawlers often do not run JavaScript, so product links may show the generic product-page preview. Product-specific WhatsApp previews require separate static HTML files per product (or server rendering). No social image is supplied while real product photos are pending.

## Included files
index.html, shop.html, product.html, cart.html, about.html, contact.html, concern.html, css/style.css, js/main.js, js/products.js, images/, PROJECT_BRIEF.md and this guide. Checkout is part of cart.html; concern.html provides individual concern views using a URL parameter.
