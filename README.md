# Krishi Mitra — Hobby Agriculture Dashboard

A personal hobby project exploring a React interface for an agricultural assistant, with crop diagnosis, local sourcing, market prices, crop planning and government-scheme exploration.

## Interface

- Crop-image selection and a sample diagnosis report.
- Agricultural-supply search and example store cards.
- Market-price charts and example sell/wait recommendations.
- Crop-strategy forms and a sample investment/allocation plan.
- Searchable scheme cards and details.
- An animated Three.js background and responsive navigation.

**Status:** frontend demonstration. Diagnosis, stores, prices and crop plans are populated from mock data in `src/pages/`; the simulated agent-status display is also presentation logic. This repository does not contain a diagnostic model, live market feed or agent backend. Displayed confidence scores, returns and scheme details are illustrative sample content.

## Run locally

Use Node.js 20+ and npm:

```sh
git clone https://github.com/Lakshaypal/hobby-agri-dashboard.git
cd hobby-agri-dashboard
npm ci
npm run dev
```

Open the URL printed by Vite.

```sh
npm run build
npm run preview
npm run lint
```

Production output is written to `dist/`. Hosting must send browser routes such as `/diagnosis` and `/market` to `index.html`.

## Structure

```text
src/App.tsx                 Routes and application shell
src/pages/                  Agricultural-assistant screens and sample data
src/components/layout/      Navigation and shared layout
src/components/3d/          Background scene
src/components/ui/          Interface primitives and status display
```

Built with React 18, TypeScript, Vite, Tailwind CSS, shadcn/Radix primitives, Framer Motion and Three.js.
