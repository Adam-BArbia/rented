# Rented

Rented is the first Tunisian platform that completely reimagines renting. We know the old way — scrolling through endless Facebook groups, haggling in comments, handing over cash to a stranger, and hoping the tool you rented actually works. No contract, no insurance, no delivery. Just stress. Rented changes all of that.

We built Rented to make renting tools and goods as simple, safe, and transparent as possible. Here’s how it works: you open the app or website, browse a growing catalogue of tools and equipment from verified owners across Tunisia, and rent what you need with a few clicks. Every single listing comes from an owner who has passed a rigorous government ID and photo verification, so you know exactly who you’re dealing with. No anonymous profiles, no guesswork.

What happens after you book? We take care of the rest. Rented manages the entire transaction from start to finish - secure in‑app payment, scheduling of a national courier for doorstep delivery, and even the return pickup at the end of the rental period. You never need to meet the owner or handle logistics. We are the trusted middleman in every step.

Before the tool leaves the owner, a unique video verification system kicks in. The owner records a timestamped, coded video proving the item works perfectly. That video becomes the single source of truth if anything goes wrong. If the tool arrives damaged or doesn’t match the description, you don’t pay. If damage happens during your rental, a fair, evidence‑based resolution process protects everyone.

And because every transaction is backed by a legally binding digital contract and comprehensive insurance covering theft, accidental damage, and liability, you are protected in ways no informal arrangement can offer. Rented’s insurance is provided by an established Tunisian insurer, giving you real peace of mind.

For owners, Rented isn’t just a listing board — it’s a complete rental business dashboard. You set your price, we automatically calculate your net earnings after deducting our small commission and insurance fee. You see in real time how many products are rented, which ones are most popular, and where your deliveries are. You never have to chase a client for payment or resolve a dispute alone.

Rented is designed for the everyday Tunisian who wants to access tools without buying them, and for owners who want to earn money from their idle equipment without the headache. It’s renting made effortless: all the trust, all the convenience, none of the hassle.

## Running locally

1. Install dependencies: `npm install`
2. Start dev server: `npm run dev`

## Repository remotes

- Original: https://github.com/Ahmed-Braiek/rentend.git
- Pushed to: https://github.com/Adam-BArbia/rented


## Technical overview

### App

- Single-page React app (TypeScript) built for a streamlined rental experience.
- Routing and data-driven pages live under `src/routes/`.
- UI components are in `src/components/` and `src/components/ui/` (Radix + custom primitives).
- Mock and static data lives under `src/data/` and `src/lib/mock-data.ts`.
- Client state is managed via the app store in `src/lib/store.ts` (Zustand).

### Stack & libraries

- Language: TypeScript
- Framework: React 19
- Bundler/Dev server: Vite
- Router: @tanstack/react-router
- Data fetching / caching: @tanstack/react-query
- State: zustand
- UI primitives: @radix-ui/*, Tailwind CSS
- Icons: lucide-react
- Date utilities: date-fns
- Form handling: react-hook-form

### Project structure (high level)

- `src/routes/` — route files and pages
- `src/components/` — UI and shared components
- `src/lib/` — utilities, store, API and mock-data
- `src/data/` — JSON fixtures used for local development

### Useful scripts

```bash
npm install
npm run dev     # start dev server (vite)
npm run build   # production build
npm run preview # preview production build
npm run lint    # run eslint
npm run format  # run prettier
```

### Notes

- This project includes a video verification concept and a digital-contract workflow in the UI — backend integrations and production-grade insurance handling are out of scope for this frontend skeleton and should be implemented by integrators.
- See `package.json` for exact dependency versions.

---
