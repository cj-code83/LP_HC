# Loss Prevention Behaviour Check

A retail compliance audit app for store leaders. Run structured loss prevention audits across 6 categories, score them with a weighted system, and track trends over time.

## Run & Operate

- `npm run dev` — start the dev server (port 3000)
- `npm run build` — build for production
- `npm run preview` — preview the production build

## Stack

- React 18 + Vite 5
- TypeScript
- Tailwind CSS v4
- Recharts (trend chart)
- localStorage (no backend — all data persists in-browser)

## Where things live

- `src/lib/questions.ts` — the full question bank (edit to add/remove/modify questions)
- `src/lib/storage.ts` — localStorage read/write utilities
- `src/pages/Dashboard.tsx` — dashboard with stats, trend chart, audit history
- `src/pages/Audit.tsx` — the audit form (questions by category)
- `src/pages/Results.tsx` — results view with score, breakdown, pass/fail lists
- `src/components/Header.tsx` — sticky header with navigation and dark mode toggle

## Scoring

- Green ≥ 80%, Amber ≥ 70%, Red < 70%
- Critical questions (weight 2) count double
- N/A answers are excluded from scoring

## User preferences

_Populate as you build._
