# Pricing Page (Bootstrap Mini Project)

A clean, responsive pricing page built with **Bootstrap 5**, showcasing three subscription tiers — Free, Pro, and Enterprise — in a card-based layout.

## 🚀 Features

- Three-tier pricing layout (Free / Pro / Enterprise)
- Fully responsive grid using Bootstrap's column system
- Card-based design with headers, pricing, feature lists, and call-to-action buttons
- Differentiated button styles to highlight the recommended plan (outline vs. solid)
- No custom CSS required — built entirely on Bootstrap utility classes

## 🛠️ Built With

- **HTML5**
- [Bootstrap 5.3.8](https://getbootstrap.com/) — via CDN (jsDelivr)

## 📁 Project Structure

```
pricing-page/
├── index.html      # Page markup and Bootstrap layout
└── README.md
```

## ⚙️ How It Works

- Each plan is a Bootstrap `.card` wrapped in a responsive column (`col-sm-5 col-md-3`), so cards stack on small screens and sit side by side from `md` breakpoints up.
- `.row.justify-content-center` centers the three cards as a group.
- Each card has a `.card-header` (plan name), `.card-body` with the price (`.card-title`), a `.list-unstyled` feature list, and a plan-specific button.
- The **Pro** and **Enterprise** buttons use `.btn-primary` (solid) to draw more attention than the **Free** plan's `.btn-outline-primary`.

## ▶️ Getting Started

1. Clone or download this project.
2. Open `index.html` directly in any modern browser.
3. No build tools, package manager, or local server needed — Bootstrap is loaded via CDN.

```bash
git clone <your-repo-url>
cd pricing-page
open index.html   # or just double-click the file
```

## 🔧 Customization

| What to change         | Where                                             |
|--------------------------|----------------------------------------------------|
| Plan names & prices     | `<h4>` and `<h1 class="card-title">` in each card |
| Feature list             | `<ul class="list-unstyled">` items per card       |
| Button text/style       | `<button class="btn ...">` per card               |
| Number of plans          | Add/remove `.card.col-sm-*.col-md-*` blocks       |
| Layout spacing           | Bootstrap spacing utilities (`mt-4`, `mb-3`, `me-md-3`) |

## 🐞 Known Issues / To-Do

- The Enterprise card uses `col-sm-10` while Free and Pro use `col-sm-5` — this is likely a typo, since it makes the Enterprise card full-width on small screens instead of matching the other two.
- No `col-lg-*` classes set, so column widths on large screens fall back to the `md` values.
- Cards aren't wrapped in equal-height containers (`d-flex`/`h-100`), so uneven content (e.g. longer feature lists) could make cards different heights.
- No highlighted/"Most Popular" badge on the Pro plan, which is common on pricing pages to nudge conversions.

## 📄 License

This project is open source and available for learning purposes.

## 🙌 Credits

Built with [Bootstrap](https://getbootstrap.com/).
