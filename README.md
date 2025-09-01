Project overview

A production‑ready React e‑commerce frontend featuring product browsing, search with debounce, cart and checkout flows, authentication, and order views. It integrates with a REST backend, persists sessions and cart state via localStorage, and uses a component library for rapid UI development and responsive design.
Features

    Product listing, detail pages, and related items with client routing for seamless navigation.

Debounced search and filters to reduce API load and enhance responsiveness under typing.

Cart management (add/update/remove), order placement views, and conditional rendering for auth‑gated routes.

Authentication flow with persisted identity using localStorage for returning visitors.

Reusable components, refs for imperative interactions, and lifecycle patterns for effects/data sync.

Responsive layouts leveraging a third‑party component library and utility classes to ensure consistency across devices.
Tech stack

    React, React Router, JavaScript/TypeScript.

REST API integration via fetch/axios; optional react-query hooks for server state.

UI: Material UI/Ant Design/Chakra or Tailwind CSS; CSS modules or utility classes.

Storage: localStorage for session/cart.

Tooling: Node.js, npm, setup.sh for environment bootstrap.
Monorepo structure (example)

    backend/ — Node/Express service with routes for products, auth, cart, orders.

frontend/ — React app with pages, components, and API clients.
Prerequisites

    Node.js LTS and npm installed; bash-compatible shell to run setup.sh.

Setup and run

    Make setup executable and run:

    chmod +x setup.sh.

./setup.sh.

    Backend:

    cd backend.

npm install.

npm start (or npm run dev).

    Frontend:

npm install.

npm run start (or npm run dev based on tooling).

Update environment variables (e.g., API_BASE_URL, AUTH_SECRET, STRIPE_PUBLIC_KEY if applicable) in .env files per service before starting.
