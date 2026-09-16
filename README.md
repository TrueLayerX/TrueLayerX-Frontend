# TrueLayerX Frontend

Business dashboard for the TrueLayerX revenue attestation protocol. Connect revenue sources, trigger attestations, and view on-chain proof history.

## Tech Stack

- **React 18** + **TypeScript**
- **Vite** for build and dev server
- **React Router** for navigation

## Prerequisites

- Node.js 18+
- npm or yarn

## Setup

```bash
# Install dependencies
npm install

# Start development server (http://localhost:5173)
npm run dev
```

The dev server proxies `/api` to `http://localhost:3000` (backend). Start the backend for full functionality.

## Scripts

| Command   | Description              |
|----------|--------------------------|
| `npm run dev`    | Start Vite dev server   |
| `npm run build`  | Production build        |
| `npm run preview`| Preview production build|
| `npm run lint`   | Run ESLint              |

## Project structure

```
truelayerx-frontend/
├── src/
│   ├── components/   # Layout, shared UI
│   ├── pages/        # Dashboard, Attestations
│   ├── App.tsx
│   ├── main.tsx
│   └── index.css
├── public/
├── index.html
├── package.json
├── tsconfig.json
└── vite.config.ts
```

## Environment

Create `.env` (optional) for API base URL override:

```
VITE_API_URL=http://localhost:3000
```

## Merging to remote

This directory is a separate git repository. To push to your remote:

```bash
git remote add origin <your-frontend-repo-url>
git push -u origin main
```
