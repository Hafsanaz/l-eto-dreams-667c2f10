# L'Eto Dreams
# L'ETO Bakeshop

A premium, minimal website for **L'ETO Bakeshop**, a bakery in Attock, Pakistan — built to feel like a luxury European patisserie. Visitors can browse the menu, read reviews, place custom cake enquiries, and order via WhatsApp or phone.

Built with [Lovable](https://lovable.dev) and connected to GitHub for two-way sync.

🔗 **Live site:** [l-eto-dreams.vercel.app](https://l-eto-dreams.vercel.app/)

## ✨ Features

- **City/outlet selector** — landing page to choose from bakery locations (currently Attock, Hazro, Nowshera Cantt, Mardan).
- **Home page** — hero section, featured products, "Why Choose L'ETO," customer favorites, Instagram callout, and a final call-to-action.
- **Menu page** — categorized product catalogue (Cakes, Cheesecakes, Sundaes, Cupcakes, Pastries, and more), styled as a digital version of the bakery's physical menu.
- **Reviews page** — aggregate Google rating (4.3/5, 100+ reviews) with curated customer testimonials and a "Leave a Google Review" link.
- **Contact page** — address, phone/WhatsApp, opening hours, embedded Google Map, social links, and a custom cake enquiry form that sends details via WhatsApp.
- **Cart** — lightweight cart widget for building an order.
- **WhatsApp & click-to-call ordering** — direct `wa.me` links and `tel:` links throughout.

## 🎨 Design System

- **Colors:** Powder Blue (`#D9E1EC`) background, Warm Ivory (`#F8F5F0`) secondary background, Deep Navy (`#173A5E`) primary text/buttons, Soft Gold (`#C9A66B`) accent.
- **Typography:** Playfair Display for headings, Poppins for body text.
- **Aesthetic:** elegant, minimal, warm — intentionally avoids a "corporate" feel, with a small, focused set of pages (Home, Menu, Reviews, Contact only).

## 🛠️ Tech Stack

- **Framework:** [TanStack Start](https://tanstack.com/start) (React 19) with [TanStack Router](https://tanstack.com/router) and [TanStack Query](https://tanstack.com/query)
- **Build tool:** Vite 8
- **Styling:** Tailwind CSS v4
- **UI components:** Radix UI primitives via shadcn-style components (accordion, dialog, dropdown, popover, tabs, tooltip, etc.)
- **Backend/data:** [Supabase](https://supabase.com) (`@supabase/supabase-js`)
- **Forms & validation:** react-hook-form + Zod
- **Other notable libraries:** `lucide-react` (icons), `sonner` (toasts), `embla-carousel-react` (carousels), `recharts` (charts), `date-fns`, `cmdk`, `vaul`
- **Package manager:** Bun (`bun.lock`, `bunfig.toml`)
- **Linting/formatting:** ESLint + Prettier
- **Hosting:** Vercel

## 📁 Project Structure

```
l-eto-dreams/
├── .lovable/          # Lovable project metadata
├── public/            # Static assets
├── src/                # Application source (routes, components, etc.)
├── supabase/           # Supabase config/migrations
├── AGENTS.md           # Notes for AI coding agents working on this repo
├── package.json
├── vite.config.ts
├── tsconfig.json
├── components.json     # shadcn/ui component config
└── README.md
```

## ⚠️ Notes

- **`.env` is committed to this repo.** It currently contains only the Supabase **publishable** (anon) key and project URL — these are designed by Supabase to be exposed on the client side and are safe to ship in a browser bundle, *provided* Row Level Security (RLS) policies are properly configured on the Supabase tables. Even so, committing `.env` files isn't best practice; consider moving these to `.env.local` (gitignored) and relying on your hosting provider's environment variable settings instead, especially if a *service role* or other secret key is ever added later.
- This project is actively synced with **Lovable** — per `AGENTS.md` in the repo, avoid force-pushing, rebasing, or amending already-pushed commits on the connected branch, as it can break the sync and cause lost history in the Lovable editor.

## 🚀 Getting Started

### Prerequisites
- [Node.js](https://nodejs.org/) (for npm) or [Bun](https://bun.sh/) (recommended, matches the repo's lockfile)
- A [Supabase](https://supabase.com) project (if you need your own backend instance rather than using the existing one)

### Setup
```bash
git clone https://github.com/Hafsanaz/l-eto-dreams-667c2f10.git
cd l-eto-dreams-667c2f10
bun install   # or: npm i
```

### Development
```bash
bun run dev   # or: npm run dev
```

### Build & Preview
```bash
bun run build     # or: npm run build
bun run preview   # or: npm run preview
```

### Linting & Formatting
```bash
bun run lint
bun run format
```

## 🔄 Continue Editing in Lovable

This project can also be edited visually in the [Lovable editor](https://lovable.dev/projects/61d9c212-7385-4562-a47c-b4eca194e1ba) — changes made there sync directly back to this repository's `main` branch, and pushes to `main` sync back into Lovable.

## 📍 Current Outlet Info (Attock, flagship)

- **Address:** Opposite Total Parco Petrol Pump, Near Teen Meela Chowk, Attock, Pakistan
- **Phone/WhatsApp:** +92 335 6633668
- **Hours:** Mon–Thu 11:00 AM–11:00 PM · Fri–Sun 11:00 AM–12:00 AM
- **Social:** [Instagram](https://instagram.com/letobakeshop) · [Facebook](https://facebook.com/letobakeshop) · [TikTok](https://www.tiktok.com/@letobakeshop)

## 👤 Author

**Hafsa Naz**
[GitHub Profile](https://github.com/Hafsanaz)

## 📄 License

Add license information here.
