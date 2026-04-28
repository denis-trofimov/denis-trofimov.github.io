---
name: workflow-upstream-upgrade
overview: Bring local GitHub workflows in sync with upstream `HugoBlox/hugo-theme-developer-portfolio` while fixing current runtime/input warnings in your Actions runs.
todos:
  - id: diff-upstream-workflows
    content: Align local workflow action versions with upstream (build/deploy/upgrade).
    status: completed
  - id: fix-pnpm-input-name
    content: Change pnpm input key to package_json_file in upgrade workflow.
    status: completed
  - id: verify-actions-warnings
    content: Run/inspect workflows to confirm warnings are resolved except known upstream Hugo action warning.
    status: completed
isProject: false
---

# Upgrade Workflows From Upstream + Fix Current Warnings

## What I found

- Your local workflows differ from upstream in key action versions:
  - `actions/checkout`: local `v4`, upstream `v6`
  - `actions/setup-go`: local `v5`, upstream `v6`
  - `peter-evans/create-pull-request`: local `v6`, upstream `v7`
- The `Unexpected input(s) 'package_json_path'` warning is in `[/home/denis/p/dev-portfolio/.github/workflows/upgrade.yml](/home/denis/p/dev-portfolio/.github/workflows/upgrade.yml)` and comes from `pnpm/action-setup` expecting `package_json_file`.
- `peaceiris/actions-hugo@v3` still declares `runs: using: node20` upstream, so Node 20 deprecation warnings cannot be fully eliminated without replacing that action.

## Planned changes

- Update `[/home/denis/p/dev-portfolio/.github/workflows/build.yml](/home/denis/p/dev-portfolio/.github/workflows/build.yml)` to match upstream action major versions where applicable:
  - `actions/checkout@v6`
  - `actions/cache@v5`
  - Keep other upstream-aligned behavior unchanged.
- Update `[/home/denis/p/dev-portfolio/.github/workflows/deploy.yml](/home/denis/p/dev-portfolio/.github/workflows/deploy.yml)`:
  - `actions/checkout@v6` (upstream parity).
- Update `[/home/denis/p/dev-portfolio/.github/workflows/upgrade.yml](/home/denis/p/dev-portfolio/.github/workflows/upgrade.yml)`:
  - `actions/checkout@v6`
  - `actions/setup-go@v6`
  - `peter-evans/create-pull-request@v7` (upstream parity)
  - Fix pnpm input from `package_json_path` to `package_json_file` (warning fix).
- Keep `pnpm/action-setup@v4` for parity with upstream unless you want me to intentionally diverge (e.g. `v5`), since upstream still pins `v4`.
- Keep `peaceiris/actions-hugo@v3` for upstream parity and document residual Node 20 warning as upstream limitation.

## Validation steps after edits

- Run a dry verification by checking workflow YAML syntax and action references.
- Trigger `upgrade` workflow manually and confirm:
  - no `Unexpected input(s) 'package_json_path'` warnings,
  - no Node 20 warnings for `checkout`, `setup-go`, `create-pull-request`.
- Trigger `build`/`deploy` path and confirm only potential remaining Node 20 warning is from `peaceiris/actions-hugo@v3`.

## Optional follow-up (if you want zero Node 20 warnings)

- Replace `pea` in build/upgrade with a shell-based Hugo installer step (download release tarball + verify version), remov`ceiris/actions-hugo@v3`ing dependency on a Node20-based JS action.

