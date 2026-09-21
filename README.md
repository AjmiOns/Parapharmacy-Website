# 🧴 Parapharmacy Website

A responsive **parapharmacy e-commerce front-end** built with **HTML, CSS, JavaScript and Bootstrap**.

The project provides a complete multi-page user interface for discovering health and wellness products, browsing product categories, viewing product details, managing a shopping cart, checking out, signing in, reading customer reviews, and contacting the store.

> **Project type:** Front-end / static web application  
> **Status:** UI prototype — no server-side backend or database is currently connected.

---

## 📸 Overview

**Parapharmacy Website** is designed as a modern online storefront for a parapharmacy. The interface focuses on a clean shopping experience, responsive layouts, product presentation, and easy navigation between the main customer journeys.

### Main pages

- 🏠 **Home** — Landing page with featured content and product highlights
- ℹ️ **About** — Store presentation and available services
- 🛍️ **Shop** — Product catalogue with categories
- 📦 **Product Details** — Detailed product presentation
- 🛒 **Cart** — Shopping cart interface
- 💳 **Checkout** — Customer/order information form
- 🔐 **Login** — Authentication interface
- ⭐ **Reviews** — Customer reviews and multimedia content
- 📍 **Contact** — Contact form and interactive map
- 🔜 **Coming Soon** — Promotional / upcoming-product page

---

## ✨ Features

### 🛍️ E-commerce interface

- Product catalogue
- Product categories
- Product detail pages
- Shopping cart interface
- Checkout interface
- Product search UI
- Product reviews
- Customer account/login interface

### 🎨 UI / UX

- Responsive layout
- Mobile-friendly navigation
- Bootstrap-based components
- Product cards and promotional sections
- Font Awesome icons
- Consistent navigation and footer
- Hover and transition effects
- Health & wellness oriented visual design

### 📍 Contact & location

- Contact form
- Interactive map using **Leaflet**
- OpenStreetMap tile layer
- Store location marker

### 🎬 Multimedia

- Product images
- Product demonstration videos
- Customer review media

---

## 🛠️ Technology Stack

| Technology | Purpose |
|---|---|
| **HTML5** | Page structure and semantic markup |
| **CSS3** | Custom styling and responsive presentation |
| **JavaScript** | Client-side interactions |
| **Bootstrap 5** | Responsive UI and components |
| **jQuery** | DOM utilities and template interactions |
| **Font Awesome** | Icons |
| **Slick Carousel** | Product/image carousel components |
| **Leaflet** | Interactive map |
| **OpenStreetMap** | Map tiles |
| **Google Fonts / Roboto** | Typography |

---

## 📁 Project Structure

```text
Parapharmacy-Website/
│
├── assets/
│   ├── css/
│   │   ├── bootstrap.min.css
│   │   ├── custom.css
│   │   ├── fontawesome.css
│   │   ├── fontawesome.min.css
│   │   ├── slick.min.css
│   │   ├── slick-theme.css
│   │   ├── templatemo.css
│   │   └── ...
│   │
│   ├── js/
│   │   ├── bootstrap.bundle.min.js
│   │   ├── jquery-1.11.0.min.js
│   │   ├── jquery-migrate-1.2.1.min.js
│   │   ├── slick.min.js
│   │   ├── templatemo.js
│   │   └── custom.js
│   │
│   ├── img/
│   │   ├── product images
│   │   ├── promotional images
│   │   └── review videos
│   │
│   └── webfonts/
│
├── index.html
├── about.html
├── shop.html
├── shop-single.html
├── cart.html
├── checkout.html
├── login.html
├── review.html
├── contact.html
├── coming.html
├── chekout.html
└── README.md
```

> `chekout.html` is a duplicate/legacy checkout page kept in the current project. `checkout.html` is the main checkout page.

---

## 🚀 Getting Started

### 1. Clone the repository

```bash
git clone https://github.com/AjmiOns/Parapharmacy-Website.git
```

### 2. Open the project

```bash
cd Parapharmacy-Website
```

### 3. Run the website

This is a static front-end project, so no Node.js installation or backend server is required for the basic version.

You can open:

```text
index.html
```

directly in a browser.

### Recommended: VS Code + Live Server

For a better development workflow, open the project in **Visual Studio Code** and use the **Live Server** extension.

Then launch:

```text
index.html
```

through Live Server.

---

## 🔄 Main User Flow

```text
Home
  │
  ├── About
  ├── Shop
  │     │
  │     └── Product Details
  │             │
  │             └── Add to Cart
  │
  ├── Reviews
  ├── Contact
  ├── Login
  │
  └── Cart
        │
        └── Checkout
```

---

## 🧩 Architecture

The current version follows a simple **static multi-page architecture**:

```text
Presentation Layer
        │
        ├── HTML pages
        ├── CSS / Bootstrap
        └── JavaScript
                │
                └── Browser
```

There is currently **no API layer, database, authentication service, payment gateway, or server-side business logic** connected to the project.

This makes the project suitable as a front-end prototype and provides a clean foundation for a future full-stack implementation.

---

## 🔐 Security

The project is currently front-end only.

### Important

Do not commit:

- API keys
- private access tokens
- database credentials
- `.env` files containing secrets
- administrator credentials
- private configuration files

For browser-side services that require public keys, use provider-supported public tokens and configure the appropriate domain/restriction settings.

---

## ⚠️ Current Limitations

The current repository is primarily a **front-end prototype**.

The following features require backend integration to become production-ready:

- User registration and authentication
- Persistent shopping cart
- Product inventory
- Order management
- Payment processing
- Database storage
- Server-side form processing
- Real customer reviews
- Real-time order tracking
- Secure user sessions

The forms and e-commerce pages currently represent the **user interface and navigation flow**, rather than a complete production e-commerce backend.

---

## 🗺️ Future Roadmap

### Phase 1 — Front-end improvements

- [ ] Improve accessibility
- [ ] Standardize CSS across all pages
- [ ] Remove duplicate/legacy files
- [ ] Improve responsive behavior
- [ ] Add form validation
- [ ] Improve SEO metadata
- [ ] Optimize images and videos

### Phase 2 — JavaScript functionality

- [ ] Dynamic product filtering
- [ ] Functional search
- [ ] Dynamic cart management
- [ ] Quantity updates
- [ ] LocalStorage cart persistence
- [ ] Checkout validation

### Phase 3 — Full-stack architecture

- [ ] REST API
- [ ] Database integration
- [ ] User authentication
- [ ] Product management
- [ ] Inventory management
- [ ] Order management
- [ ] Admin dashboard
- [ ] Payment integration

### Phase 4 — Production readiness

- [ ] Automated testing
- [ ] CI/CD pipeline
- [ ] Environment configuration
- [ ] Security hardening
- [ ] Performance optimization
- [ ] Production deployment

---

## 💻 Development Workflow

Recommended Git workflow:

```bash
git checkout -b feature/feature-name
```

Make your changes, then:

```bash
git add .
git commit -m "feat: add feature description"
git push origin feature/feature-name
```

For maintenance or fixes:

```bash
git checkout -b fix/issue-description
```

### Commit convention

Recommended Conventional Commits format:

```text
feat: add product filtering
fix: correct checkout form validation
style: improve product card layout
refactor: reorganize JavaScript functions
docs: update README
perf: optimize product images
```

---

## 🌐 Repository

**GitHub:**  
https://github.com/AjmiOns/Parapharmacy-Website

---

## 👩‍💻 Author

**Ajmi Ons**

GitHub:  
https://github.com/AjmiOns

---

## 📄 License

No explicit license has been added to the repository yet.

If this project is intended to be reused or distributed publicly, consider adding an appropriate open-source license such as **MIT**.

---

## 🙏 Acknowledgements

This project uses resources and libraries including:

- [Bootstrap](https://getbootstrap.com/)
- [jQuery](https://jquery.com/)
- [Font Awesome](https://fontawesome.com/)
- [Leaflet](https://leafletjs.com/)
- [OpenStreetMap](https://www.openstreetmap.org/)
- [Google Fonts](https://fonts.google.com/)

---

## ⭐ Project Goals

The goal of this project is to build a clean and responsive parapharmacy storefront while practicing:

- Front-end web development
- Responsive UI design
- Multi-page website architecture
- E-commerce user flows
- Git and GitHub version control
- Project organization
- Preparation for future full-stack development
