# AGENTS.md — updates

**This repository is public.** It is the investor-facing record of what Volve Vision ships:
changelog, roadmap, per-product history and monthly updates. It contains no source code.

## Before writing anything here

Follow `Volve-Vision/updates-playbook`. It holds the procedure, the safety rules (what may never be
published), the style rules and the templates. The short version:

- Never paste a commit message through. Every line is rewritten for a reader outside the company.
- No stack, no vendors, no hostnames, no internal service names, no security mechanisms, no metrics
  beyond catalogue scale.
- Release status comes from the stores and live services, never from git history.
- `updates-playbook/scripts/preflight.sh` must exit zero before anything is pushed.
- Show the owner the full text and wait for an explicit yes before publishing.

Publishing is permanent: git history keeps a leaked detail even after the file is deleted.

## Organisation rules

- Map of every repository, its checkout and its deploy target: **`Volve-Vision/volve-handbook`**.
- If you create, rename, transfer or archive a repository, run `~/Volve/bin/volve-repo-map` and
  commit the handbook **in the same session**. The map is generated, never hand-edited.
- Remotes are `https://VolveVision@github.com/Volve-Vision/<repo>.git`; `gh` picks the account
  automatically through `~/Volve/bin/gh`.
- Never deploy, restart a service or touch production data without the owner asking in this session.
