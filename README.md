# Nice Gadgets — Product Catalog

A responsive e-commerce catalog application for browsing phones, tablets, and accessories, viewing product specifications, managing favorites and shopping cart items, and filtering/paginating products via URL query parameters. Built with React, TypeScript, and modular SCSS.

## Live Preview

- [Live Demo](https://oksana-zakharevych.github.io/nice-gadgets-catalog/)

## Design Reference

- [Figma Design](https://www.figma.com/design/T5ttF21UnT6RRmCQQaZc6L/Phone-catalog--V2--Original?node-id=0-1&p=f&t=sC3i0yxigH9Bjs09-0)[cite: 18]

## Technologies Used

- React
- TypeScript
- SCSS / CSS Modules
- Swiper
- Vite

## Getting Started

1. Clone the repository:

```bash
git clone [https://github.com/oksana-zakharevych/nice-gadgets-catalog.git](https://github.com/oksana-zakharevych/nice-gadgets-catalog.git)
cd nice-gadgets-catalog
```

2. Install dependencies:

```bash
npm install
```

3. Run the project locally:

```bash
npm start
```

## Features

- **Home Page (`/`)**: Hero banner slider with auto-advance and manual navigation, *Brand new models* and *Hot prices* product carousels powered by Swiper, and category navigation cards.
- **Category Pages (`/phones`, `/tablets`, `/accessories`)**: Product listings with loading states, error handling with retry, sorting (`Newest`, `Alphabetically`, `Cheapest`) synchronized with URL query params, and pagination (`page` and `perPage`).
- **Product Details Page (`/product/:productId`)**: Interactive gallery, variant selectors (colors and capacities), product description, tech specs, breadcrumbs, back navigation, random suggested products, and a *Product was not found* fallback.
- **Shopping Cart (`/cart`) & Favorites (`/favorites`)**: State persisted in `localStorage` with live header counters, item quantity controls, automatic total calculation, and checkout confirmation flow.
- **Not Found Fallback**: Dedicated `NotFoundPage` for unmatched routes with a link back to the home page.
