

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
- **Evidence** Preliminary Test-ProductReadiness -Check all -Write (profile reader/web/public/prototype): stage works not-met, target works. Top gaps: typecheck (tsc TS2882 on side-effect import './styles.css'; no vite/client types), B1.1 (SPEC.md core flows never run end to end by an agent; SPEC.md is absent or a template), B1.3 (PRODUCT.md is the unfilled template; names no audience or purpose).
- **Fix Recommendation** Work READINESS.md top-down: add vite/client types so npm run typecheck passes, fill PRODUCT.md (audience and purpose) and SPEC.md core flows, then run and receipt them. READINESS.md is the live gap list; this record is a pointer, not a copy.
- **Fix Location** READINESS.md Next gaps; tsconfig.json / src/vite-env.d.ts; PRODUCT.md; SPEC.md
- **Fix Rationale** Stage works needs a green typecheck, a stated purpose and the core flows proven; later stages follow the order in READINESS.md.
- **CannotFixHere** sweep files the app's own gaps record into its lane worktree by design
- **Queue** .agents/work/imports/intake/queue--20261108T024457500Z--390bf93fb6dc49bc9746f3f776971850.json
<!-- agent-harness:intake:v1:end -->
