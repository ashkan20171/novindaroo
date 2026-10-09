<div align="center">

# 💊 NovinDaroo — Bilingual Digital Pharmacy Experience

**A design-led healthcare storefront portfolio, built with accessible vanilla web technologies.**

English-first · فارسی / RTL · 3D-inspired visuals · Product discovery · Wishlist · Optional AI backend

![HTML5](https://img.shields.io/badge/HTML5-Semantic-E34F26?logo=html5&logoColor=white) ![CSS3](https://img.shields.io/badge/CSS3-Responsive-1572B6?logo=css3&logoColor=white) ![JavaScript](https://img.shields.io/badge/JavaScript-Vanilla-F7DF1E?logo=javascript&logoColor=black) ![Node.js](https://img.shields.io/badge/Node.js-Optional_Backend-339933?logo=nodedotjs&logoColor=white)

</div>

## ✨ Project overview

NovinDaroo explores the intersection of **healthcare UX, accessible commerce and internationalization**. It is a multi-page portfolio demonstration rather than a licensed online pharmacy. The interface defaults to English and supports Persian with direction-aware RTL/LTR layouts.

## Product highlights

| Experience | Implementation |
|---|---|
| 🌍 Localization | English default, Persian toggle, direction switching; some legacy content remains untranslated |
| 🛍️ Storefront | Product catalog, search/filter/sort, detail view, browser-based cart |
| ❤️ Saved products | LocalStorage wishlist |
| ⌨️ Quick navigation | Ctrl/Cmd+K bilingual searchable navigation dialog |
| 🎨 Visual design | Healthcare color system, responsive cards, local 3D-inspired SVG backgrounds, light/dark UI |
| 💬 Assistant | Rule-based demo and optional Node.js API integration; live AI requires a server-side API key |
| ♿ Accessibility | Semantic markup, keyboard navigation, focus management, reduced-motion support |
| 🔐 Trust | Explicit demo disclosures and privacy page |

## 🧱 Architecture

```text
index.html / shop.html / other pages
├── css/          # Base design + progressive enhancements
├── js/           # Catalog, i18n, UI interactions and stage modules
├── images/       # Local visual assets
├── assets/       # Icons and 3D-inspired background artwork
└── server/       # Optional Node.js chat API
```

The project intentionally uses **HTML, CSS and vanilla JavaScript** on the client. No frontend build step is required.

## 🚀 Run locally

**Frontend only** (Python 3):

```bash
python -m http.server 8000
```

Visit `http://localhost:8000`. For the optional chat backend (Node.js 20+):

```bash
node server/server.js
```

Visit `http://localhost:3000`. To enable AI responses, configure `OPENAI_API_KEY` as an environment variable **on the server**, not in client JavaScript. Without it, chat is demo-only.

## 🧪 Quality checks

```bash
for file in js/*.js server/*.js; do node --check "$file"; done
```

Also manually verify EN/FA switching, desktop/mobile navigation, cart, wishlist, quick navigation (Ctrl/Cmd+K), and keyboard-only use. Automated end-to-end browser coverage is not yet complete.

## 🩺 Responsible scope

**Portfolio demo only.** There is no verified pharmacy license, real payment processor, fulfillment service, or secure prescription-processing workflow. Do not submit real patient information. The assistant is not a medical professional and must not be used for diagnosis or prescribing. See [SECURITY.md](SECURITY.md).

## 🗺️ Roadmap

- Complete translation of all legacy and dynamic content
- Add automated cross-browser and accessibility testing
- Consolidate incremental CSS/JS modules into maintainable components
- Add authenticated commerce APIs and compliant prescription workflows *only after regulatory and security review*
- Add CI quality gates, performance budgets and production monitoring

## 🤝 Engineering & collaboration

Built as a portfolio case study in responsive frontend engineering, localization and thoughtful healthcare UX. Contributions are welcome; see [CONTRIBUTING.md](CONTRIBUTING.md).

---

**Suggested repository:** `novindaroo-digital-pharmacy-platform`  
**GitHub About:** `Bilingual EN/FA digital pharmacy portfolio | Responsive HTML, CSS & JavaScript, RTL/LTR, 3D-inspired UI, wishlist, accessible UX & optional Node.js AI assistant.`
