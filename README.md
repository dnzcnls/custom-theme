# Maison Noir — Shopify Theme

A luxurious black-and-white editorial theme inspired by Chanel and Prada.

## Importing

1. Compress the contents of this folder into a `.zip` (already provided as `maison-noir-theme.zip`).
2. In Shopify admin: **Online Store → Themes → Add theme → Upload zip file**.
3. Once uploaded, click **Customize** to open the theme editor.

## After import — required setup

### 1. Create the pages used by the navigation
In **Online Store → Pages**, create the following pages (the title is what matters; let Shopify auto-generate the handle):

| Title           | Handle (auto) | Template to assign     |
|-----------------|---------------|------------------------|
| Boutique        | `boutique`        | `page.boutique`        |
| Ready-to-Wear   | `ready-to-wear`   | `page.ready-to-wear`   |
| Joaillerie      | `joaillerie`      | `page.joaillerie`      |
| Journal         | `journal`         | `page.journal`         |
| About           | `about`           | `page.about`           |

For each page, on the right side under **Theme template**, pick the matching template.

### 2. Customer accounts (for Sign In / Register)
The login and register pages use Shopify's native customer forms. They only work when customer accounts are enabled:

- **Settings → Customer accounts → Show login link in the header and at checkout**.
- For the classic forms used by this theme, choose **Legacy / Classic accounts**.

### 3. Edit products without a Shopify catalog
The home page and Boutique / Ready-to-Wear / Joaillerie pages use the **Product showcase** section. Each product is a **block** you can edit directly in the theme editor:

- Upload an image, set the category, name, price, and link.
- Optionally connect the block to a real Shopify product (so the link and price stay in sync).

### 4. Customize anything else
Everything is editable in **Customize**:
- Header announcements and nav links
- Hero image and CTAs
- Editorial split cards
- Manifesto quote
- Feature banner
- Services grid
- Footer columns

## File map

```
assets/         CSS, JS, and editorial / product placeholder images
config/         Theme settings
layout/         theme.liquid global shell
locales/        Translation strings
sections/       Editable sections (hero, product-showcase, editorial-split, …)
snippets/       Reusable partials (icons, product-card, meta-tags)
templates/      JSON templates: index, product, cart, page.boutique, page.about, …
```
