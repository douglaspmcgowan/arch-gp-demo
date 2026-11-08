

<!-- agent-harness:intake:v1:start -->
## Intake - filed by agents working on other projects

> An agent that finds something wrong here while working elsewhere records it and does
> not fix it. This block is where those records land; this project's own agent triages
> them, promotes what it takes to TASK.md, and deletes nothing to make a count look
> better. Written by ``Add-ProjectIntake.ps1`` -- add items with that tool rather than by
> hand, so the id-collision check and the format actually hold.
### app-standard-gaps

**App Standard gaps: stage works, target works**

- **Filed** 2026-11-08 by an agent working on app-standard-sweep
- **Relationship** defect - **Value** medium - **Risk** low
- **Evidence** Test-ProductReadiness -Check all -Write against the deployed site https://arch-gp-demo.vercel.app (profile reader/web/public/prototype): stage works not-met, target works. Top gaps: typecheck (npm run typecheck missing; tsc fails TS2882 on side-effect import './styles.css'), B1.1 (no SPEC.md naming core flows; agent walk of TASK.md flows at 1440 and 390 px recorded could-not-tell), B1.3 (PRODUCT.md is the unfilled template).
- **Fix Recommendation** Work READINESS.md top-down: add a "typecheck": "tsc --noEmit" script to package.json and src/vite-env.d.ts containing /// <reference types="vite/client" /> to fix TS2882; write SPEC.md naming the core flows (field-to-source highlight, graph browse, part QR, maintenance-loop explainer) and rerun the B1.1 walk; fill PRODUCT.md with audience and purpose. READINESS.md is the live gap list; this record is a pointer, not a copy.
- **Fix Location** package.json scripts; src/vite-env.d.ts; SPEC.md; PRODUCT.md; READINESS.md Next gaps
- **Fix Rationale** Stage works needs a green typecheck, a stated purpose and the core flows proven; later stages follow the order in READINESS.md.
- **CannotFixHere** sweep files the app's own gaps record into its lane worktree by design
- **Queue** .agents/work/imports/intake/queue--20261108T024457500Z--390bf93fb6dc49bc9746f3f776971850.json
<!-- agent-harness:intake:v1:end -->
