# Embraced OS — Demo Shell Status

**Repo:** `AHD-Embraced-AI/embraced-os-demo`  
**Build:** Qt Shell 3.0 baseline (2025-11-19)  
**Owner:** AngelHeart Designs – Embraced AI

---

## Current State (Public Demo)

This repo hosts a **demo shell** of Embraced OS:

- ✅ Qt-based desktop shell (Shell 3.0)
- ✅ Full black canvas (no wallpaper yet)
- ✅ Fade-only chrome (top / left / right / bottom)
- ✅ Profile selector (Demo / Founder / Developer)
- ✅ Status / State / Version / Self-test views (UI-driven text)
- ✅ Lightweight Settings stub (profile selector only)
- ⚠️ Engine integration is minimal and safe:
  - Some commands are wired through a thin adapter
  - No Guardian / vault / private internals are exposed

> For details, see [README.md](./README.md).

---

## What Works Today

- Launching the Qt shell locally
- Edge-hover chrome (fade in / fade out)
- Switching between profiles via the top-right dropdown
- Viewing:
  - “Embraced OS is online…” status summary
  - Runtime state summary
  - Version information
  - UI shell self-test message
- Opening the Settings dialog and changing the active profile (UI-level)

---

## What This Repo Does *Not* Contain

- No Guardian policy engine
- No vault or sensitive runtime state
- No production security features
- No full app suite (this is a shell-only demo)

Those live in private, non-public repos.

---

## Roadmap (Public View)

Short term, this demo repo may add:

- Screenshots / short video of the shell
- A basic widget/tiles sample
- A simple “about this demo” overlay
- Minor UX polish (fonts, spacing, focus handling)

Anything involving Guardian, vault, or deeper engine internals will **not** be added here.

---

## How to Help

- Open an issue if:
  - The README or STATUS docs are confusing
  - You hit problems running the demo
  - You have calm-UI / accessibility suggestions
- Please **do not** submit security/engine internals here — this repo is intentionally limited to a safe UI demo.

---

What to tell Echo

From the embraced-os-demo repo root:

# 1) Create STATUS.md with the content above
# (Echo: overwrite STATUS.md if it already exists)

# 2) Stage, commit, and push on the same docs branch
```bash
git add STATUS.md
git commit -m "docs: add STATUS overview for Qt Shell 3.0 demo"
git push origin docs/qt-shell-3-baseline-20251119
```
