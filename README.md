# 🛍️ shopwave-ui

> A modern, high-performance e-commerce storefront built with Next.js 15 App Router — featuring server components, optimized image delivery, and a seamless shopping experience.

![Next.js](https://img.shields.io/badge/Next.js_15-000000?style=for-the-badge&logo=nextdotjs&logoColor=white)
![TypeScript](https://img.shields.io/badge/TypeScript-007ACC?style=for-the-badge&logo=typescript&logoColor=white)
![Tailwind CSS](https://img.shields.io/badge/Tailwind_CSS-38B2AC?style=for-the-badge&logo=tailwind-css&logoColor=white)
![Vercel](https://img.shields.io/badge/Vercel-000000?style=for-the-badge&logo=vercel&logoColor=white)

---

## 📸 Preview

> _Add a screenshot or screen recording of your app here_
> `![App Preview](./public/preview.png)`

---

## ✨ Features

- 🚀 **Next.js 15 App Router** — Server Components, layouts, and nested routing
- 🛒 **Shopping Cart** — Add, remove, and manage cart items with persistent state
- 🔍 **Product Catalog** — Browse and filter products by category, price, and rating
- 📦 **Product Detail Pages** — Dynamic routes with full product info and image gallery
- 💳 **Checkout Flow** — Multi-step checkout with form validation
- 📱 **Fully Responsive** — Optimized for mobile, tablet, and desktop
- ⚡ **Optimized Performance** — Image optimization via `next/image`, font optimization via `next/font` (Geist)
- 🎨 **Tailwind CSS** — Utility-first styling with consistent design system

---

## 🛠️ Tech Stack

| Layer | Technology |
|---|---|
| Framework | Next.js 15 (App Router) |
| Language | TypeScript |
| Styling | Tailwind CSS |
| Font | Geist (via `next/font`) |
| State Management | Zustand / Context API |
| HTTP Client | Axios / Fetch API |
| Deployment | Vercel |

---

## 📁 Folder Structure

```
shopwave-ui/
├── app/
│   ├── (auth)/
│   │   ├── login/
│   │   └── register/
│   ├── products/
│   │   ├── [id]/
│   │   │   └── page.tsx        # Product detail page
│   │   └── page.tsx            # Product listing page
│   ├── cart/
│   │   └── page.tsx
│   ├── checkout/
│   │   └── page.tsx
│   ├── layout.tsx              # Root layout
│   └── page.tsx                # Home / landing page
├── components/
│   ├── ui/                     # Reusable UI primitives
│   ├── product/                # Product card, gallery, filters
│   ├── cart/                   # Cart drawer, cart item
│   └── layout/                 # Navbar, footer, sidebar
├── lib/
│   ├── api.ts                  # API client / fetchers
│   └── utils.ts                # Utility functions
├── store/                      # Zustand store (cart, auth)
├── types/                      # Global TypeScript types
├── public/                     # Static assets
└── ...config files
```

---

## 🚀 Getting Started

### Prerequisites

- Node.js `>= 18.x`
- npm / yarn / pnpm / bun

### Installation

```bash
# Clone the repository
git clone https://github.com/chaudhary-rishabh/shopwave-ui.git
cd shopwave-ui

# Install dependencies
pnpm install
```

### Environment Variables

Create a `.env.local` file in the root:

```env
NEXT_PUBLIC_API_URL=http://localhost:5000/api
NEXT_PUBLIC_APP_URL=http://localhost:3000
```

> ⚠️ Never commit `.env.local` to version control.

### Run Development Server

```bash
pnpm dev
```

Open [http://localhost:3000](http://localhost:3000) in your browser.

---

## 🔗 Backend

This frontend is paired with **[shopwave-server](https://github.com/chaudhary-rishabh/shopwave-server)** — a REST API built with Node.js / Express handling products, auth, orders, and payments.

---

## 📦 Scripts

| Command | Description |
|---|---|
| `pnpm dev` | Start development server |
| `pnpm build` | Create production build |
| `pnpm start` | Start production server |
| `pnpm lint` | Run ESLint |
| `pnpm type-check` | Run TypeScript compiler check |

---

## 🌐 Deployment

This app is optimized for deployment on **[Vercel](https://vercel.com)**:

```bash
pnpm build
```

Or connect your GitHub repo to Vercel for automatic CI/CD deployments on every push to `main`.

---

## 🤝 Contributing

1. Fork the repo
2. Create your feature branch: `git checkout -b feat/your-feature`
3. Commit your changes: `git commit -m "feat: add your feature"`
4. Push to the branch: `git push origin feat/your-feature`
5. Open a Pull Request

---

## 📄 License

This project is licensed under the **MIT License** — see the [LICENSE](./LICENSE) file for details.

---

<p align="center">Built with ❤️ by <a href="https://github.com/chaudhary-rishabh">Rishabh Chaudhary</a></p>
