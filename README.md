# Moni Dresses Client

Customer/B2C application. Production hostname: `shop.monidresses.com`.

This repository is separate from Admin, Branch, Creator, Team, Wholesale, and backend repositories.

## Architecture
- Customer authentication: Firebase Auth
- Customer data/orders: Firestore
- Payments: Razorpay through Firebase Cloud Functions
- Shipping: Shiprocket through Firebase Cloud Functions
- Admin-controlled catalog/site configuration: Firestore

## Routes
- `/` — customer home
- `/shop.html` — catalog
- `/product.html?id=<productId>` — product details
- `/cart.html` — cart
- `/checkout.html` — checkout
- `/orders.html` — customer orders
- `/account.html` — customer account
- `/login.html` — authentication

Never place Razorpay secrets, Shiprocket credentials, or Firebase Admin credentials in this repository.
