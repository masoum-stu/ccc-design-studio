# Custom Carpet Creations — Design Studio

**Client review version** · Interactive bespoke carpet design tool

A professional, single-file web application that lets customers design their carpet live, upload inspiration photos, apply ready-made patterns, and book a free consultation.

---

## What’s included

| File | Purpose |
|------|---------|
| `ccc-design-studio.html` | **Full standalone app** — Design wizard + Order tracking + Admin dashboard |
| `ccc-widget.html` | **Embeddable widget** — Same design engine, ready for iframe / WordPress embed |
| `README.md` | This guide |

Open either HTML file directly in a browser — no build step or server required.

---

## Features (polished for client review)

### Design experience
- **6 carpet styles** — Traditional, Contemporary, Rug, Stairs (runner), Woven, Carved  
  Each style has a distinct border, field and ornament language.
- **Live canvas** — Drag shapes, resize with the corner handle, delete (Delete key or button).
- **14+ shape tools** — Circles, stars, diamonds, hexagons, crescents, boteh, flowers, arches, scroll, etc.
- **Photo upload** — Drop or browse an image; place it on the carpet; mask it as rectangle, circle, oval, diamond, hexagon, octagon, arch or star; colour the photo border.
- **Ready-made patterns** — One-click patterns that change with the selected style.
- **20 colour swatches + custom colour picker**.
- **Material & texture** — Silk, wool, blends, nylon, bamboo silk · Cut pile / Loop / Cut & Loop / Flat weave (with live texture simulation).
- **Size & shape** — Rectangular, square, round, custom; live proportion preview.
- **Undo / Clear / Download PNG** — Undo last layer (Ctrl/Cmd+Z), clear canvas, export the design as a high-quality PNG for the client or workshop.

### Order flow
1. Style & materials  
2. Size & room  
3. Design studio  
4. Customer details (validated)  
5. Consultation booking (video / phone / in-person) + production journey overview  
6. Confirmation with unique reference number  

### Tracking & admin
- **Track order** — Customer enters reference + email.
- **Admin dashboard** (demo password: `admin123`)  
  - Stats overview  
  - Filterable order list  
  - Status updates + notes (visible on the customer tracking page)  
  - Orders stored in `localStorage` (demo / prototype)

---

## How to review / share with the client

### Option A — Instant review
1. Open the GitHub repository.
2. Click **ccc-design-studio.html**.
3. Click the **Raw** button, then open that URL in a new tab  
   *or* download the file and double-click it.

### Option B — GitHub Pages (recommended for a clean link)
1. Go to the repository **Settings → Pages**.
2. Source: Deploy from **main** branch, folder **/ (root)**.
3. After a minute the live site will be at:  
   `https://masoum-stu.github.io/ccc-design-studio/ccc-design-studio.html`

### Option C — Embed the widget on a website
```html
<iframe
  src="https://masoum-stu.github.io/ccc-design-studio/ccc-widget.html"
  width="100%"
  height="900"
  frameborder="0"
  style="border:none;border-radius:12px;overflow:hidden"
  title="Custom Carpet Creations Design Studio">
</iframe>
```

---

## Technical notes for the developer / agency

- **Zero dependencies** — pure HTML / CSS / Canvas 2D / vanilla JS.
- **Responsive** — works on desktop and mobile (touch drag & resize supported).
- **Data** — Orders live in `localStorage` under key `ccc_orders` (demo only).  
  For production: connect the submit step to Formspree, a CRM, or your own API (the widget already has a Formspree placeholder).
- **Admin password** — change the hard-coded check in `admLogin()` before any real use.
- **Branding** — gold / charcoal palette matches a high-end carpet / interiors brand. Easy to re-theme via CSS custom properties at the top of the file.

---

## Suggested next steps after client approval

1. Replace demo admin password and wire real authentication.
2. Connect form submission to email / CRM / Formspree / Zapier.
3. Persist designs (optional) — send canvas PNG + layer JSON with the order.
4. Host on the client’s domain or as a WordPress page.
5. Optional: add account system so customers can save drafts.

---

## Contact for production questions

Custom Carpet Creations  
+44 (0)1737 830 301  

---

*Prepared as a client-ready prototype. Open the HTML file to experience the full design studio.*
