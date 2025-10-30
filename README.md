# RVService.app

Dealer-branded RV service platform: mobile scheduling, loyalty, parts, and AI support.  
Built with **Next.js + TypeScript**, **TailwindCSS**, **shadcn/ui**, and **lucide-react**.

## ✨ Features
- **Service Scheduling:** Book appointments in-app with preferred dates/techs
- **Loyalty & Rewards:** Earn points on service/parts; redeem for perks
- **Parts & Accessories:** Browse + add-to-cart; dealer-controlled catalog
- **AI Technician Support:** 24/7 guided troubleshooting + call-to-service
- **Dealer Branding:** White-label theming, logos, and content
- **Analytics (opt-in):** Usage insights to improve retention and revenue

> The starter UI includes hero, feature cards, and modals (Appointments, Rewards, Parts, Support, Cart) with shadcn/ui & lucide-react icons.

## 🪙 Tech Stack
- **Framework:** Next.js (App Router) + TypeScript
- **Styling:** TailwindCSS + shadcn/ui
- **Icons:** lucide-react
- **State/Context:** React Context for cart and modals
- **Build/Format:** ESLint, Prettier, TypeScript strict

## 💻 Project Structure (suggested)
```
src/
  app/                # Next.js App Router (or pages/ if you're on Pages Router)
    layout.tsx
    page.tsx         # landing / feature cards / modals
  components/
    Header.tsx
    HeroSection.tsx
    FeatureCard.tsx
    modals/
      AppointmentModal.tsx
      RewardsModal.tsx
      PartsModal.tsx
      SupportModal.tsx
      CartModal.tsx
    ui/              # shadcn/ui components
  contexts/
    CartContext.tsx
  lib/
    utils.ts
public/
  images/
```

## 🚀 Getting Started

### 1) Install
```bash
pnpm install   # or npm i / yarn
```

### 2) Dev server
```bash
pnpm dev
```
Visit http://localhost:3000

### 3) Environment variables (create `.env.local`)
```
# Optional (examples—add only what you actually use)
NEXT_PUBLIC_APP_NAME=RVService.app
# TWILIO_*, STRIPE_*, DATABASE_URL, etc. when you wire integrations
```

## 🛍️ Code you have
You can drop your main landing page at `src/app/page.tsx` (App Router) or `src/pages/index.tsx` (Pages Router).  
Your current component includes Header, Hero, Feature cards, and modals using shadcn/ui & lucide-react.

## 👐 Integrations (roadmap)
- Payments (Stripe)
- SMS/Voice (Twilio) for reminders & AI support handoff
- Calendar sync (Google Calendar/Microsoft)
- Dealer DMS connector (export/import first, API later)

## 🤓 Scripts
```json
{
  "scripts": {
    "dev": "next dev",
    "build": "next build",
    "start": "next start",
    "lint": "next lint",
    "format": "prettier --write ."
  }
}
```

## 💪 License
MIT — see [LICENSE](./LICENSE).

## 💖 Contributing
Issues and PRs are welcome. Please use the templates in `.github/` and follow the guidelines in [CONTRIBUTING.md](./CONTRIBUTING.md).

## 📧 Support
Open an issue or email support@rvservice.app
