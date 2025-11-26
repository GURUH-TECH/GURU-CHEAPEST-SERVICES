# GURU TECH LAB — Starter Marketing Panel (Legal / Organic Services)

This repository is a starter full-stack project for **GURU TECH LAB**: a marketing / social-media services panel focused on **legal, organic services** (social media management, content creation, ad campaign management, analytics, SEO, influencer coordination). **This project does NOT provide, support, or automate fake followers, bot engagement, or any activity that violates platform Terms of Service.**

## What's included
- `backend/` — Node.js + Express API with auth, services, orders, Stripe webhook skeleton, and database migrations (Postgres via Knex).
- `frontend/` — React (Vite) + Tailwind CSS minimal dashboard and pages (Home, Login, Dashboard, Order).
- `.env.sample` — environment variables to configure services.
- `README` with deployment notes and recommended workflow.

## Quick start (development)

### Backend
```bash
cd backend
cp .env.sample .env
# edit .env to set DATABASE_URL, JWT_SECRET, STRIPE keys and FRONTEND_URL
npm install
# create DB & run migrations (requires Postgres)
# Example using psql:
#   psql $DATABASE_URL -f migrations/001_init.sql
npm run dev
```

### Frontend
```bash
cd frontend
cp .env.sample .env
npm install
npm run dev
```

## Deployment
Recommended:
- Host backend on Render (Web Service) with a managed Postgres.
- Host frontend on Netlify or Render (static site).
- Set Stripe webhook endpoint to `https://<your-backend>/api/webhooks/stripe`.

## Important
This starter intentionally avoids any automation for fake engagement. Use it to sell or manage legitimate marketing services.

