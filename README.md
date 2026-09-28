# 213 RUN

A streetwear shopping experience built around easy product discovery, a clear checkout flow, and a responsive interface.

**Live site:** [Explore 213 RUN](https://run213.vercel.app)

---

## The experience

- Browse products and curated looks.
- Explore product details, including colors, sizes, availability, and images.
- Save favorites and add items to the cart.
- Place an order as a guest or use an account to access orders and other activity.
- Explore RUN CLUB, the community area of the site.

The project also includes an admin dashboard for managing products and orders.

---

## Screenshots

*Screenshots will be added here.*

---

## Tools and what they do

- **Next.js, React, and TypeScript** — build the pages, interactive components, and typed application logic.
- **Tailwind CSS** — style responsive parts of the interface.
- **Firebase** — provides authentication and Firestore data for products, accounts, orders, and other features.
- **Cloudinary** — delivers images for products and community content. Image URLs can be adjusted for different display sizes and formats.
- **Upstash Redis** — supports rate limiting on sensitive actions, including checkout, to reduce repeated or abusive requests.
- **Vercel** — hosts the web application.

---

## Admin and server-side protection

The admin dashboard provides workflows for managing product information and reviewing orders.

Protected admin API routes verify a Firebase ID token **on the server** and check for an admin permission before allowing administrative actions. Product input is validated on the server before it is written to Firestore.

Checkout also goes through a server API route. The server validates the request, applies rate limits, and creates the order. Sensitive service credentials belong in server environment variables rather than frontend code.

---

## Performance, SEO, and analytics

- Product and image delivery are designed with different screen sizes in mind.
- Some product data is cached, and Firestore queries use limits or pagination to control unnecessary reads.
- Public pages include page metadata and social sharing information.
- GA4 helps measure public site activity after the visitor accepts analytics cookies.

---

## My contribution

*I will add a precise description of the parts I worked on here.*

---

## What I learned

*I will add a few specific challenges, decisions, and lessons from the project here.*
