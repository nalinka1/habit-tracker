# Habit Tracker

A full-stack habit tracking app, built incrementally as a hands-on learning
project. The frontend is Next.js (App Router, TypeScript, Tailwind); the
backend is a NestJS REST API. Both live together in a single monorepo.

This project starts intentionally small — an in-memory API and a basic UI —
and grows over time: persistence (Prisma + database), authentication,
deployment, and CI/CD are added as deliberate later stages rather than built
upfront. See [ROADMAP.md](./ROADMAP.md) for the full plan.

Built with a feature-branch → pull request → manual review workflow, using
Claude Code as an AI pair-programmer for implementation.

## Stack

- **Frontend:** Next.js (App Router, TypeScript, Tailwind CSS) — `apps/web`
- **Backend:** NestJS (REST API) — `apps/api`
- **Storage:** in-memory for now → SQLite/Postgres later (via Prisma)
- **Node version:** 24.x (Active LTS)

## Project structure

\`\`\`
habit-tracker/
├── apps/
│   ├── web/     # Next.js frontend
│   └── api/     # NestJS backend
├── packages/    # (future) shared TypeScript types
└── ROADMAP.md   # staged build plan
\`\`\`

## Getting started

### Prerequisites
- Node.js 24.x ([nvm](https://github.com/nvm-sh/nvm) or [nvm-windows](https://github.com/coreybutler/nvm-windows) recommended)
- npm

### Run the backend
\`\`\`bash
cd apps/api
npm install
npm run start:dev
\`\`\`
Runs on `http://localhost:3000` by default.

### Run the frontend
\`\`\`bash
cd apps/web
npm install
npm run dev
\`\`\`
Runs on `http://localhost:3000` by default — change one app's port if running both simultaneously.

## Development workflow

1. Create a feature branch: `git checkout -b feature/your-feature-name`
2. Build the feature (using Claude Code or manually)
3. Push the branch and open a pull request
4. Manually review and merge into `master`
5. *(Later stage)* Automated PR review and deploy previews

## Status

🚧 Early stage — scaffold complete, first features in progress. See
[ROADMAP.md](./ROADMAP.md) for what's next.

## In Progress
