# 📱 PhoneBazaar

A modern, fully responsive marketplace website for buying, selling and trading smartphones. It's built as a **single `index.html` file** with plain HTML, CSS and JavaScript, so there's no framework, no build step and no dependencies.

## ✨ Features

- **Product catalog** with live search, brand filter chips and price sorting
- **Working shopping cart** with a slide-in drawer, remove items, running total and demo checkout
- **Condition grades** (New, Like New, Refurbished) and discount badges on every listing
- **Sections:** Hero, Shop, Why Us, Services, Contact, Footer
- **Validated contact form** with inline error messages
- **Responsive layout** for mobile, tablet and desktop, including a hamburger menu
- **Automatic dark mode** via `prefers-color-scheme`
- **Zero dependencies:** all icons and phone graphics are inline SVG

## 🚀 Getting Started

1. Download or clone this repository.
2. Open `index.html` in any modern browser (Chrome, Edge, Firefox, Safari).

No server, install or build step is needed.

```bash
git clone https://github.com/<your-username>/phonebazaar.git
cd phonebazaar
# then just open index.html
```

## 🛠️ Customization

| What | Where |
|------|-------|
| Products, prices, brands | The `phones` array at the top of the `<script>` block |
| Colors | CSS variables in `:root` (`--brand`, `--brand2`, `--bg`, ...) |
| Brand name and text | Search for `PhoneBazaar` in `index.html` |
| Contact details | The `#contact` section |

To add a phone, add an object to the array:

```js
{ id: 9, n: "Model Name 128GB", b: "Brand", p: 499, o: 699, c: "New", g: ["#5b4bff", "#00c2a8"] }
```

`n` is the name, `b` the brand, `p` the price, `o` the original price, `c` the condition and `g` the two gradient colors.

## 📁 Project Structure

```
phonebazaar/
├── index.html   # markup, styles and scripts in one file
└── README.md
```

## ⚠️ Notes

- Checkout and the contact form are **front-end demos**. Nothing is sent to a server.
- The cart is held in memory and resets on page reload.
- To make it real, connect the form and checkout to a backend or a service such as Formspree, Stripe or Firebase.

## 🧰 Tech Stack

HTML5 · CSS3 (Grid, Flexbox, custom properties) · Vanilla JavaScript (ES6) · Inline SVG

## 📄 License

Released under the MIT License. Free to use, modify and distribute.