# Roadmap

A staged, incremental plan. Each stage is a deliberate, standalone milestone —
not everything is built upfront.

## Build stages

- [x] Stage 1: Scaffold Next.js (`apps/web`) + NestJS (`apps/api`)
- [ ] Stage 2: NestJS — basic habits CRUD API (in-memory storage)
- [ ] Stage 3: Next.js — habits UI calling the API
- [ ] Stage 4: Add persistence (SQLite/Postgres via Prisma)
- [ ] Stage 5: Add authentication
- [ ] Stage 6: Deploy (Vercel for web, Railway/Render for api)

## Automation stages

- [ ] Stage 7: Claude Code GitHub Action — automated PR review (comment-only)
- [ ] Stage 8: Auto-merge once checks pass
- [ ] Stage 9: Other automations — deploy previews per PR, test generation,
      scheduled issue triage

## Workflow (current)

Feature branch → Claude Code implements → PR opened → manual review → merge
into `master`.
