# Deployment

This Vite single-page demo is ready for Vercel. The rewrite in `vercel.json` keeps QR-linked paths inside the app rather than returning a 404.

Once the demo has passed its local checks, publish from its own Git repository (not the `agent-harness` worktree):

```powershell
gh repo create douglaspmcgowan/arch-gp-demo --public --source . --remote origin --push
vercel --prod --yes
```

Both GitHub and Vercel were authenticated as `douglaspmcgowan` when this file was prepared. Do not copy `.vercel/`, `node_modules/`, or build output into the repository.
