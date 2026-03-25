
# FairWay Foundation 🏌️‍♂️

A subscription-based golf charity platform combining performance tracking, monthly prize draws, and charitable giving. Built as part of the Digital Heroes Full-Stack Development Trainee Selection Process.

🌐 **Live Website**: [fair-way-foundation-client.vercel.app](https://fair-way-foundation-client-hakdc3be1-asmitshukls-projects.vercel.app)

---

## 📋 Overview

FairWay Foundation is a modern web application where golfers subscribe, enter their Stableford scores, participate in monthly prize draws, and contribute to charities they care about. The platform is designed to feel emotionally engaging — leading with charitable impact, not sport.

---

## ✨ Features

**For Users**
- Monthly & yearly subscription plans via Stripe
- Golf score entry (Stableford format, rolling 5-score system)
- Monthly prize draw participation (3, 4, and 5-number match tiers)
- Charity selection and contribution management
- User dashboard with subscription status, scores, draw history, and winnings

**For Admins**
- Full user & subscription management
- Draw configuration (random or algorithmic), simulation, and publishing
- Charity directory management
- Winner verification and payout tracking
- Reports and analytics

---

## 🛠️ Tech Stack

| Layer | Technology |
|---|---|
| Frontend | React + Vite + TypeScript |
| Backend | Node.js + Express + TypeScript |
| Database | MongoDB Atlas |
| Payments | Stripe |
| Auth | JWT |
| Monorepo | pnpm workspaces + Turborepo |
| Deployment | Vercel (client) + Railway (backend) |

---

## 📁 Project Structure

```
FairWay-Foundation/
├── apps/
│   ├── client/          # Vite React frontend
│   └── backend/         # Express API server
├── packages/
│   ├── db/              # Shared database models
│   ├── ui/              # Shared UI components
│   └── typescript-config/
├── pnpm-workspace.yaml
└── turbo.json
```

---

## 🚀 Getting Started

### Prerequisites
- Node.js 20+
- pnpm 9+
- MongoDB Atlas account
- Stripe account

### Installation

```bash
git clone https://github.com/Asmitshukl/FairWay-Foundation.git
cd FairWay-Foundation
pnpm install
npm run dev
```

### Environment Variables

Create `apps/backend/.env`:

```env
PORT=3000
MONGO_URI=your_mongodb_connection_string
JWT_SECRET=your_jwt_secret
JWT_EXPIRES_IN=7d
STRIPE_SECRET_KEY=your_stripe_secret_key
STRIPE_PRICE_MONTHLY=your_monthly_price_id
STRIPE_PRICE_YEARLY=your_yearly_price_id
STRIPE_WEBHOOK_SECRET=your_webhook_secret
CLIENT_URL=http://localhost:5173
POOL_CONTRIBUTION_PER_USER=5
```

Create `apps/client/.env`:

```env
VITE_API_URL=http://localhost:3000/api
```

---

## 🧪 Test Checklist

- ✅ User signup & login
- ✅ Subscription flow (monthly and yearly)
- ✅ Score entry — 5-score rolling logic
- ✅ Draw system logic and simulation
- ✅ Charity selection and contribution calculation
- ✅ Winner verification flow and payout tracking
- ✅ User Dashboard — all modules functional
- ✅ Admin Panel — full control and usability
- ✅ Responsive design on mobile and desktop

---

## 📜 License

ISC

---
