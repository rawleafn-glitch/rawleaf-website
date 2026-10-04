# Rawleaf Ecommerce

A mobile-first wellness store for Rawleaf, designed in black, ivory and muted gold. Built with plain HTML, CSS and JavaScript—no frameworks, installation or build step.

## What it includes

- Seven products with prices in Indian Rupees.
- Shop filters, search and price sorting.
- Product and wellness concern pages.
- A cart with quantity controls and browser storage.
- Checkout with COD or UPI and an order draft sent through WhatsApp.
- About and contact pages, FAQs and a floating WhatsApp button.

## Preview the website

Download or clone this repository, then double-click `index.html`. Keep all the folders beside the HTML files. Google Fonts, WhatsApp and UPI app links need internet access.

Cart storage depends on your browser. For reliable storage across pages, also test the hosted website.

## Project files

| File or folder | Purpose |
|---|---|
| `index.html` | Home page |
| `shop.html` | All products and filters |
| `product.html?id=1` | Product details selected by ID |
| `concern.html?category=Sleep` | Products for a wellness concern |
| `cart.html` | Cart and checkout |
| `about.html`, `contact.html` | Brand and contact information |
| `css/style.css` | Colours, fonts and layouts |
| `js/products.js` | Products, prices, offers, reviews and bundles |
| `js/main.js` | Cart, filters and WhatsApp checkout |
| `images/` | Product images and favicon |
| `PROJECT_BRIEF.md` | Approved discovery brief |

## Make changes

Edit `js/products.js` to change products, prices and image descriptions. All seven supplied primary photos are installed. Beta Revive has three secondary gallery images. Edit `css/style.css` to change the design.

Offers, reviews and bundles are empty until real content is supplied. An approved discount can be added to `DISCOUNTS` with a `code` and `percent`. Bundles use the sum of their individual product prices.

## Before taking live orders

Supply verified ingredients and directions, approved claims, shipping charges, delivery coverage and return/COD terms. Confirm product spellings and prices.

The UPI ID is configured. The QR area is a labelled, non-scannable placeholder; replace it with the merchant's real QR image. UPI receipt is checked manually. WhatsApp opens an order draft that the customer must send; the website does not automatically confirm or centrally store orders.

Product totals exclude shipping, which Rawleaf confirms before the order is finalised. Visual testing at 375px is still pending.

## Publish as a static website

This project needs no build command. Publish the repository's root folder with GitHub Pages or another static host. For GitHub Pages, choose the `main` branch and `/ (root)` folder in the repository's Pages settings.

The metadata uses `https://www.rawleafs.in`. Update canonical and Open Graph URLs if using a different domain. Product and concern metadata changes through JavaScript; some social sharing crawlers will show the generic page preview.

## Contact

WhatsApp / call: +91 9038152100

Email: rawleafcare@gmail.com
