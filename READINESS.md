# Readiness: arch-gp-demo

| works | usable | polished | production | operated |
| --- | --- | --- | --- | --- |
| not-met (target) | not-targeted | not-targeted | not-targeted | not-targeted |

Target: works

## Next gaps

- typecheck (failing): Type check passes. Not applicable only when package.json has no typecheck script and the app has no tsconfig.json.
- B1.1 (could-not-tell): Every core flow named in SPEC.md runs end to end.
- B1.3 (no-check): PRODUCT.md names who the app is for and why it exists.

## B1 Purpose and core flows

| item | statement | verify | state | last run |
| --- | --- | --- | --- | --- |
| B1.1 | Every core flow named in SPEC.md runs end to end. | agent | could-not-tell | 2026-11-08 |
| B1.3 | PRODUCT.md names who the app is for and why it exists. | auto | no-check | never |

## B4 Errors and recovery

| item | statement | verify | state | last run |
| --- | --- | --- | --- | --- |
| B4.1 | No uncaught errors on the core flows. | auto | met | 2026-11-08 |

## B11 Security and privacy

| item | statement | verify | state | last run |
| --- | --- | --- | --- | --- |
| B11.1 | No secrets in the client bundle or the repository. | auto | no-check | never |

Generated from `.agents/work/readiness.json` by `Test-ProductReadiness.ps1 -Write`; do not edit. States derive from receipts.

`met` means the app's own command reported success. It does not mean the app is correct or good.

Kind: arch-gp-demo | Generated: 2026-11-08T02:46:31.9221039Z | Input hash: 645a946eff70

## Next (checks, detail)

Stage: works

- typecheck (failing): npm run typecheck - child exited 1

## Refresh

```powershell
& 'C:\Program Files\PowerShell\7\pwsh.exe' -NoProfile -NonInteractive -File ~/.agents/tools/Test-ProductReadiness.ps1 -ProductPath . -Profile .agents/app-profile.json -Check all -Write
```

## Stages (checks, detail)

| stage | state |
| --- | --- |
| works | not-met |
| usable | not-met |
| polished | not-met |
| production | not-met |
| operated | met |

## Checks (detail)

### works

| check | state | last run | exit | note |
| --- | --- | --- | --- | --- |
| build | met | 2026-11-08T02:46:15.3432453Z | 0 |  |
| typecheck | failing | 2026-11-08T02:46:15.805688Z | 1 | child exited 1 |
| console-clean | met | 2026-11-08T02:46:19.2122607Z | 0 |  |

- tests: package.json declares no test script

### usable

| check | state | last run | exit | note |
| --- | --- | --- | --- | --- |
| loading-state | could-not-tell | 2026-11-08T02:46:19.8679236Z | 2 | \{"check":"loading-state","outcome":"could-not-tell","reason":"no .agents/app-selectors.json selector map","findings":\[\]\} |
| empty-state | could-not-tell | 2026-11-08T02:46:20.8464764Z | 2 | \{"check":"empty-state","outcome":"could-not-tell","reason":"no .agents/app-selectors.json selector map","findings":\[\]\} |
| error-state | could-not-tell | 2026-11-08T02:46:22.0421416Z | 2 | \{"check":"error-state","outcome":"could-not-tell","reason":"no .agents/app-selectors.json selector map","findings":\[\]\} |
| not-found-state | could-not-tell | 2026-11-08T02:46:23.082882Z | 2 | \{"check":"not-found-state","outcome":"could-not-tell","reason":"no .agents/app-selectors.json selector map","findings":\[\]\} |
| keyboard-focus | met | 2026-11-08T02:46:25.3618394Z | 0 |  |
| viewport-320-1280 | met | 2026-11-08T02:46:29.1662557Z | 0 |  |
| not-found-page | failing | 2026-11-08T02:46:29.9230714Z | 1 | child exited 1 |

Not applicable: error-capture, structured-logs, cli-conformance, game-playable

### polished

| check | state | last run | exit | note |
| --- | --- | --- | --- | --- |
| design-banned-patterns | failing | 2026-11-08T02:46:30.7074545Z | 1 | child exited 1 |

Not applicable: design-review-dated

### production

| check | state | last run | exit | note |
| --- | --- | --- | --- | --- |
| seo-tags | failing | 2026-11-08T02:46:31.5524881Z | 1 | child exited 1 |

Not applicable: privacy-terms, security-headers, axe, core-web-vitals, log-personal-data

### operated

Not applicable: deployed-url, env-documented, monitoring, restore-path
