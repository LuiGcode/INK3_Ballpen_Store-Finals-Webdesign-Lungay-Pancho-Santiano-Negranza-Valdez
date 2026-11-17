# INK3 — Ballpen E-Commerce Website

A self-contained **client-side academic demonstration** for FEU Diliman **BA0013L — Web Client-Side Scripting**.

## The product concept

Only three fictional products are offered:

| Product | Illustrative price | Positioning |
|---|---:|---|
| Everyday Ballpen | ₱15 | Simple writing essential |
| SmoothWrite Ballpen | ₱35 | Longer writing sessions |
| Signature Ballpen | ₱149 | Premium-inspired option |

All images are custom SVG illustrations (not photos of manufactured inventory). Names, details, prices, and shipping fees are illustrative.

## How to open

1. Extract this folder if using the ZIP archive.
2. Open **index.html** in Chrome, Safari, Firefox, or Edge.
3. Use the top menu to browse **Shop**, **Our story**, **Your bag**, and **Demo checkout**.

No installation, dependency manager, database, or API key is required. JavaScript and browser local storage must be enabled.

To serve locally (optional, recommended for testing):

```sh
cd INK3_Ballpen_Store
python3 -m http.server 8000
```

Visit `http://localhost:8000`.

## Pages

- `index.html` — homepage with a brand hero and featured product collection.
- `shop.html` — all three products, with a price sorting dropdown.
- `product.html?pen=everyday` — individual product description and quantity selector.
- `product.html?pen=smoothwrite` — second product.
- `product.html?pen=signature` — third product.
- `cart.html` — editable cart and running totals.
- `checkout.html` — validation-only demo checkout and simulated confirmation.
- `about.html` — brand overview, demonstration contact form, and FAQs.

## Features implemented

- Responsive layouts for desktop and mobile, with collapsible navigation.
- All product cards and detail pages generated from a single product dataset in `app.js`.
- Add-to-cart, update quantity, remove, and cart count.
- A cart stored in browser `localStorage`, with a limit of 99 units per item.
- Example delivery fee of ₱60, waived when the sample subtotal reaches ₱500.
- Form validation and an **explicitly non-transactional** checkout simulation. No financial integration.
- Front-end contact form demonstration (no network transmission).
- Semantic HTML, alt text, skip link, keyboard operability, and reduced-motion support.

**Important:** This is not a live commerce backend. It does not transmit customer details, take payments, send emails, manage real inventory, or book actual delivery. For testing, use fictional checkout details. No sensitive data should be entered.

## How to edit products

Open `app.js` and locate the `PRODUCTS` array near the top. Change the `name`, `price`, `short`, `description`, `ink`, and other fields as needed. Keep the existing three IDs (`everyday`, `smoothwrite`, `signature`) unless you also adjust any links.

Edit `styles.css` to change colors, typography, and visual layout. The source SVG illustrations are in `assets/`.

## How to publish with a free URL

**Option A — Netlify Drop (simple):**

1. Extract the project ZIP.
2. Visit https://app.netlify.com/drop and sign in if required.
3. Drag the **INK3_Ballpen_Store** folder into the upload area.
4. Open the assigned `*.netlify.app` URL and test the links.

**Option B — GitHub Pages:**

1. Create a new public GitHub repository.
2. Upload the project files to the repository root (make sure `index.html` is at the root).
3. Go to **Settings → Pages** and choose **Deploy from a branch**, branch `main`, folder `/ (root)`.
4. Visit the generated `*.github.io` address after publication and test all pages.

These are instructions, not a claim that the project has already been published.

## How it maps to the final documentation

Your uploaded template requires sections **I–IX**. This site provides material for Introduction (INK3 concept), Objectives (product browsing, sorting, cart, form validation), Significance, Scope and Limitations (especially demo restrictions), Website Design and Development (screenshots of each page), Website Deployment (fill in your real live URL), and Conclusion and Recommendations.

Still to complete yourself: name(s) on the title page, real deployment URL, page screenshots, **Related Studies and Existing Websites** with valid reference links, and **References**. Describe the actual technology used as **HTML, CSS, and JavaScript**, not Wix, unless you rebuild on that platform. Ask the instructor if a website builder is compulsory.

## Suggested screenshots for Section VI

1. Home page (desktop)
2. Shop grid showing exactly three products
3. One individual product detail page
4. Cart with at least one product and quantity controls
5. Demo checkout form
6. Demo order confirmation
7. About/Contact page
8. Mobile homepage or shop view

## Academic integrity and readiness

Project art and copy are original to this prototype. Do not describe the dummy checkout as a real payment gateway, or the non-transmitting contact form as a working delivery mechanism. Don't claim a real business, real inventory, or orders exist.
