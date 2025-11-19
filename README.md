# Embraced OS — Demo Shell

> **Status:** Early prototype • Qt Shell 3.0 baseline • Public demo build  
> **Repo:** `AHD-Embraced-AI/embraced-os-demo`

Embraced OS is a calm, ethics-first desktop layer designed to sit *on top* of existing operating systems.  
This repo is the **public demo shell** — a small, self-contained prototype that shows the direction of the full Embraced OS project without exposing private internals.

This build focuses on:

- A **Qt desktop shell** (Shell 3.0)
- A **black “infinite canvas”** background
- **Fade-only chrome** (top / left / right / bottom)
- A simple **profile system** (Demo / Founder / Developer)
- A thin adapter into the underlying **Embraced engine** for commands
- A **Settings stub** for future customization

---

## What this demo is (and isn’t)

This demo **is**:

- A real Qt application you can run locally
- A visual prototype of the Embraced OS shell
- A safe, public snapshot of the direction:
	- Chrome behavior (fade-only)
	- Profiles
	- Status / state / version views
	- Left/right/bottom chrome behavior
- A “playfield” for people curious about the UI ideas

This demo is **not**:

- The full Embraced OS product
- The private runtime, vault, or Guardian implementation
- A security-hardened system
- A replacement for your current desktop

It’s intentionally small and demo-friendly.

---

## Current UI Features (Qt Shell 3.0 baseline)

### 1. Black Canvas + Chrome Frame

When you launch the shell you see:

- A **full black canvas** (no wallpaper yet)
- **Top, Left, Right, Bottom chrome** that:
	- Stay hidden until your mouse approaches the screen edge
	- **Fade in / fade out** (no jittery sliding)
	- Respect a calm timing profile

This is meant to feel like working on a single, clean, unified surface, not “a window with boxes.”

### 2. Profiles (top-right selector)

Top-right of the shell: a **Profile dropdown**.

Profiles available:

- `Demo`
- `Founder`
- `Developer`

Right now, profiles are:

- **Displayed in the top bar**
- **Stored in runtime state**
- Used to log / drive UI messages and future behavior

Later, profiles will drive:

- Themes
- Chrome behavior (pinned vs auto-hide)
- Default widgets
- Learning behavior

For this demo, profiles are **UI-only** knobs — safe to click, no risk.

### 3. Chrome Regions

The shell has four chrome regions:

- **Top bar:** title + profile selector + basic actions
- **Left bar:** system / status controls (wired to UI views)
- **Right bar:** reserved for widgets / tiles (later phases)
- **Bottom bar:** status line and logs

All four:

- Fade in on edge hover
- Fade out when the pointer leaves the edge
- Keep the canvas itself clean

### 4. Status / State / Version / Self-Test (left rail)

Left chrome includes buttons that currently:

- **Status view**  
	Shows a UI-generated summary like:  
	`Embraced OS is online, state: profile=demo, os=0.5.0, shell=3.0.0, started_at=…`

- **State view**  
	Shows the current runtime state:  
	`runtime state -> profile=demo, os=0.5.0, shell=3.0.0, started_at=…`

- **Version view**  
	Shows the current demo version:  
	`Embraced OS v0.5.0 • Qt Shell 3.0.0 • layout baseline checkpoint.`

- **Self-test**  
	Confirms this is a **UI shell only** build:  
	`UI shell only — engine, chrome, and hub checks are minimal in this build.`

Under the hood:

- These buttons **call into the runtime adapter**, so the path into the engine is live.
- The **text you see is UI-driven**, so it doesn’t depend on private engine internals.

### 5. Settings Stub

There is a lightweight **Settings** dialog:

- Accessible via the left chrome (Settings entry)
- Contains:
	- A **Profile selector** (same choices as the top bar)
	- **Save** and **Close** buttons
- For this demo:
	- Changing the profile here updates the runtime state
	- The dialog is intentionally minimal — it’s a hook for future customization

---

## Engine Integration (public-safe explanation)

The shell talks to a small “engine adapter” which:

- Knows how to:
	- Track the **current profile**
	- Track **OS and shell version**
	- Run commands by ID (e.g., `os.status`, `os.version`, `os.diagnostics`)
- Is intentionally **thin** in this repo:
	- Engine commands are minimal
	- There is no Guardian, vault, or sensitive logic exposed here
	- Diagnostic actions are stubbed or simplified

In logs, you’ll see entries like:

```text
[time] UI: execute command 'os.diagnostics'
[time] STATUS: Ran os.diagnostics

This shows the path is alive without exposing internal implementation.
```

## Roadmap (Public View)
High-level phases (as relevant to this demo):


S1 — Shell & Chrome (current)


Qt shell


Black canvas


Fade-only chrome


Profiles (UI-level)


Status / State / Version / Self-test views


Settings stub




S2 — Guardian & Policy (future, not in this repo)


Policy engine


Ethical guidance


Guardrails around actions



S3+ — Flows, Widgets, SDK, Apps (future)


Flow-based actions


Widgets and tiles on the canvas


Developer SDK


Embraced “Suite” of tools



This repo will stay focused on safe, demo-ready pieces.

## How to Run the Demo (Windows-focused, generic Python)

You should be comfortable with a terminal and Python.
If you’re already using the project’s qt.venv, reuse it — otherwise, make your own venv.


Clone the repo


git clone https://github.com/AHD-Embraced-AI/embraced-os-demo.git
cd embraced-os-demo


Create and activate a virtual environment


On Windows (PowerShell):
python -m venv .venv
.\.venv\Scripts\Activate.ps1

On macOS/Linux:
python -m venv .venv
source .venv/bin/activate


Install dependencies


If the repo has requirements.txt:
pip install -r requirements.txt

(or follow any instructions in requirements-qt.txt / Pipfile if provided.)


Run the Qt shell


python -m embraced_qt.main_qt

You should see:


A black canvas


Edge-fade chrome


“Profile: demo” at startup


Logs in the console like:


[time] CHROME: frame built (fade-only, black canvas)
[time] PROFILE: applied demo to UI
[time] STATUS: Profile active: demo
[time] Embraced Desktop Qt shell started.
[time] STATUS: Ready


Troubleshooting
Nothing appears / app exits immediately


Check console for Python errors or missing packages


Make sure you’re in the venv where dependencies were installed


Import error for embraced_qt


Confirm you’re running from the repo root:


The folder that contains the embraced_qt/ package


Run:
python -m embraced_qt.main_qt


Qt window is visible but chrome not fading


This demo assumes hover near the screen edges to reveal chrome.


Check that:


The app window is active (focused)


Your mouse is at the top/left/right/bottom edges



Contributing (public)
Right now contributions are limited and curated.
You can:


Open issues on this repo for:


Clarity problems in the README


UX feedback about the shell behavior


Questions about how to run the demo



Share ideas for:


Calm UI improvements


Accessibility / low-motion behavior


Profile behavior



Larger engine / Guardian / vault contributions are not accepted here — those live in private repos.

License
See LICENSE in this repo for public usage terms.


If you want a small `STATUS.md` for the repo root (for people who skip the README and go straight to “what’s the deal?”), say so and I’ll give you that as a second file.
