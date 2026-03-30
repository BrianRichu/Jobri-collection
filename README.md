
# Jobri Collection

Jobri Collection is a fashion eCommerce web application built for a real business. The project initially started with **plain HTML, CSS, and JavaScript** to build a solid foundation in core frontend concepts.

The application is to later **transition to React (Vite-powered)** to improve scalability, maintainability, and performance through a modern component-based architecture.

The long-term objective remains unchanged: full ownership of the platform—no outsourcing, no black-box logic, and complete control over performance, architecture, and feature development.


## Live Preview

The current production version (plain JavaScript) is deployed on Vercel:

**Live URL:** [https://jobri-shop.vercel.app/](https://jobri-shop.vercel.app/)


## Evolution of the Project

### Phase 1 — Vanilla JavaScript (Completed)

* Built core eCommerce functionality from scratch
* Implemented manual state management
* Structured modular JavaScript architecture
* Focused on understanding DOM manipulation and logic flow

### Phase 2 — React Migration (In Progress)

* Refactoring UI into reusable components
* Transitioning from manual DOM updates to state-driven rendering
* Improving performance and code organization
* Preparing integration with backend APIs

---


## Tech Stack

### Current (Production)

* **HTML5** – Semantic structure
* **CSS3** – Styling and responsiveness
* **JavaScript (ES6)** – Application logic and state management

### New Stack (Migration)

* **React** – Component-based UI
* **Vite** – Fast development server and build tool

### Planned Backend Stack

* **REST APIs** – Products, cart, orders, users
* **Node.js / Firebase** – Backend services and authentication
* **Payment API** – Secure checkout processing

---

## Project Structure

### Legacy Structure (Vanilla JS)

```
jobri-collection/  
├── data/  
│ ├── products.js  
│ ├── cart.js  
│ └── deliveryOptions.js
├── scripts/  
│ ├── checkout/  
│ │  ├── orderSummary.js  
│ │  └── paymentSummary.js  
│ ├── checkout.js
│ ├── index.js
│ └── productsPage.js  
├── styles/  
│ ├── jobri.css
│ ├── checkout.css  
│ └── products.css
├── images/  
├── jobri.html  
├── checkout.html
├── products.html  
└── README.md
```


## Features

- Landing page with featured products, categories, and promotional slider
- Products page with search, pagination, and add-to-cart buttons
- Product detail page with description, add-to-cart action, and FAQ accordion
- Persistent cart using `localStorage`
- Checkout page with order summary, delivery fee, total calculation, and WhatsApp order redirect
- Mobile menu and responsive header behavior on scroll


## How It Works

- Product data is stored in `data/products.js`
- `scripts/productsPage.js` renders product cards and pagination, and handles search and add-to-cart actions
- `scripts/productDetail.js` loads a product by its `id` URL parameter and displays full details
- `data/cart.js` persists cart contents in `localStorage` and exposes functions to add, remove, and clear cart items
- `scripts/checkout.js` and `scripts/checkout/orderSummary.js` render cart contents, calculate totals, and redirect the user to WhatsApp with a formatted order message
- `data/deliveryOptions.js` calculates delivery dates and adds shipping fees

## Getting Started

1. Open in your browser.
2. Navigate to `view products` to browse the available products.
3. Click a product image to view its detail page.
4. Use the Add to Cart buttons to save items to the cart.
5. Visit `checkout using the cart icon` to review your order and place it via WhatsApp.


## Purpose of This Project

* Build deep understanding of frontend fundamentals before frameworks
* Transition to modern React architecture with clarity
* Develop a real-world, production-ready eCommerce platform
* Maintain full control over system design and performance

---

## Known Limitations (Current State)

* No backend or database (yet)
* No authentication system
* No payment gateway integration

These are intentional and will be addressed in the upcoming phases.

---


## Notes

- Cart contents persist between page reloads via `localStorage`
- Checkout currently builds a WhatsApp message and redirects the user to WhatsApp Web or the WhatsApp mobile app
- Only one delivery option is currently configured in `data/deliveryOptions.js`

## Author

Brian Mwangi
Frontend Web Developer
Founder — Jobri Collection

---

## Status

🚧 Active development