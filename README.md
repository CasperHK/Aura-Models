# 靈氣模魂
## ModelArt & Garage Kit E-Commerce Platform 

Welcome to the **ModelArt Platform**, a specialized e-commerce and community-driven marketplace built specifically for model hobbyists, garage kit collectors, pro-painters, and 3D digital sculptors. 

---

## 🌟 Core Features

*   **Advanced Multi-State Product Catalog**: Support for various model states including Fully Painted Masterpieces, Commission Slots, Unpainted Garage Kits (GK), and 3D Printable STL Digital Files.
*   **Multi-Vendor Maker Hub**: Dedicated profiles and dashboards for individual modelers and studios to showcase their portfolios, manage commissions, and track sales.
*   **Immersive Gallery & Detail Views**: High-resolution image galleries with zoom capabilities, 360-degree rotation support, and Work-in-Progress (WIP) story timelines.
*   **Custom Commission System**: Built-in inquiry tools, deposit/final payment workflows, and step-by-step progress trackers for custom builds.
*   **Robust Filtering & Search**: Filter items by scale (e.g., 1/35, 1/144, 1/60), genre (Sci-Fi, Mecha, Military, Anime/GK, Diorama), material (Resin, Plastic, Metal), and availability.

---

## 🛠️ Technology Stack (Recommended)

*   **Frontend**: Next.js / React (for SEO-friendly dynamic galleries and smooth UI transitions) or Vue.js 3.
*   **Backend**: Node.js (NestJS or Express) or Go for high-performance handling of pre-order drops and traffic spikes.
*   **Database & Storage**: PostgreSQL (relational data for orders, users, and multi-variant items) and AWS S3 / Cloudflare R2 (for high-res imagery and digital STL downloads).
*   **Payment & Escrow**: Stripe / PayPal integration supporting split payments and deposit-based billing.

---

## 📂 Project Structure

```text
modelart-platform/
├── client/                 # Frontend application (Next.js / TailwindCSS)
│   ├── public/             # Static assets
│   └── src/
│       ├── components/     # Reusable UI components (ProductCard, Gallery, etc.)
│       ├── pages/          # Route views (Home, Explore, MakerHub, Checkout)
│       └── styles/         # Global styles & Tailwind config
├── server/                 # Backend API (Node.js / Express or NestJS)
│   ├── src/
│   │   ├── modules/        # Feature modules (auth, products, makers, orders)
│   │   └── main.ts         # Application entry point
├── database/               # Migration scripts and seed data
└── docs/                   # API documentation and wireframes
```

---

## 🚀 Getting Started Locally

### Prerequisites
*   Node.js (v18+ recommended)
*   npm or yarn
*   PostgreSQL instance running locally or via Docker

### Installation

1. Clone the repository:
   ```bash
   git clone https://github.com/your-username/modelart-platform.git
   cd modelart-platform
   ```

2. Set up the Backend:
   ```bash
   cd server
   npm install
   cp .env.example .env  # Configure your database credentials
   npm run start:dev
   ```

3. Set up the Frontend:
   ```bash
   cd ../client
   npm install
   cp .env.example .env.local
   npm run dev
   ```

4. Open your browser and navigate to `http://localhost:3000`.

---

## 🤝 Contributing

We welcome contributions from developers, designers, and hobbyists alike! Please check our `CONTRIBUTING.md` guidelines before submitting pull requests.

## 📄 License

This project is licensed under the MIT License - see the `LICENSE` file for details.
