# Dolphin Systems — Website

[![Website](https://img.shields.io/badge/Website-dolphinsystems.net-0b7285)](https://dolphinsystems.net)

The website and content platform for **Dolphin Systems**. This repository contains a Next.js application with company pages, product information, a blog, and related site features.

## Built with

- **Next.js 16** (App Router) and **React 19**
- **TypeScript**
- **Tailwind CSS 4** and **Framer Motion**
- **Supabase** for supported data-backed features
- **Cloudflare Tunnel, nginx and PM2** in the project's deployment setup

## Project structure

```text
src/
├── app/          # Pages, layouts and route segments
├── components/   # Reusable interface components
├── lib/          # Shared application utilities
└── types/        # TypeScript type declarations
public/           # Static assets
```

The app contains sections for the company, products, pricing, blog, community, contact and policies. Some administrative features also have their own routes.

## Run locally

**Requirements:** A recent Node.js release compatible with Next.js 16 and npm.

```bash
git clone https://github.com/TheRitikYadav/DolphinSystems.git
cd DolphinSystems
npm ci
npm run dev
```

Open **http://localhost:3000**.

Features backed by Supabase may require local environment configuration; do not commit credentials or `.env.local` to the repository.

## Commands

| Command | Purpose |
| --- | --- |
| `npm run dev` | Start the local development server |
| `npm run build` | Build the production application |
| `npm run start` | Run the built application |
| `npm run lint` | Run ESLint |
| `npm run deploy` | Use this project's environment-specific deployment script |

## Deployment notes

The Next.js configuration uses standalone output. The repository also includes deployment scripts designed for a self-hosted environment. Those scripts depend on infrastructure-specific configuration and should be reviewed before use outside the original environment.

**Project website:** https://dolphinsystems.net

---

*Technical documentation describes the repository implementation; production availability and individual features should be verified before use.*
