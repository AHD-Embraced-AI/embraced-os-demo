# Embraced OS - Interactive Demo

**AHD - Embraced AI • ©2025 AngelHeart Designs**

This guide demonstrates what Embraced OS can do through example commands and their outputs.

---

## Launch Options

Embraced OS provides two interfaces:

**Desktop GUI** - Command center with cyberpunk theme, sidebar navigation, real-time ethics tracking

**CLI Shell** - Terminal-based interface with natural language commands

Both interfaces run the same 14-layer EGAE engine underneath.

---

## Demo Commands

### System Commands

#### Check Version
```
embraced> os.version
```
**Output:**
```
Version: v0.1.0-alpha  (commit: ee7716b2)
Architecture: 14-layer AI-native EGAE
Layers: L1, L2, L3, L4, L5, L6, L7, L8, L9, L10, L11, L12, L13, L14  ✅
```

#### System Status
```
embraced> os.status
```
**Output:**
```
System Status: OPERATIONAL
Core spine L1-L14 online
Known actions: 21 registered
Last action: os.version (0.12s ago)
```

#### Self-Test
```
embraced> os.selftest
```
**Output:**
```
Running diagnostics...
✅ L1 Runtime: OK
✅ L8 Vault: OK  
✅ L12 Ethics: OK
Result: 3/3 checks PASSED
```

---

### Learning & Analytics

#### Usage Patterns
```
embraced> learn.patterns
```
**Output:**
```
Usage Statistics:
  os.version: 47 times (last: 12s ago)
  os.status: 23 times (last: 5m ago)
  learn.patterns: 8 times (last: now)
  
Top channels:
  shell: 52 invocations
  gui: 18 invocations
  
Most active hour: 14:00-15:00 (23 actions)
```

#### Recommendations
```
embraced> learn.recommend
```
**Output:**
```
Based on usage patterns:
  
Frequently used:
  - os.version (47 times) → Consider adding to favorites
  - os.status (23 times) → Create keyboard shortcut
  
Suggested shortcuts:
  - v → os.version
  - s → os.status
  - p → learn.patterns
```

---

### Creativity & Content Generation

#### System Overview
```
embraced> create.overview
```
**Output:**
```
Embraced OS - System Overview
Generated: 2025-11-17 01:45:00

Core Architecture:
  - 14-layer EGAE stack
  - 21 registered actions
  - Ethics-first design
  - Local-only execution

Top Actions:
  1. os.version (47 uses)
  2. os.status (23 uses)
  3. learn.patterns (8 uses)

System Health:
  ✅ All layers operational
  ✅ Ethics engine active
  ✅ Vault responding
```

#### Action Cheat-Sheet
```
embraced> create.cheatsheet
```
**Output:**
```
Embraced OS Quick Reference

SYSTEM
  os.version     Show version and layer status
  os.status      Display system operational state
  os.selftest    Run diagnostic checks (3 tests)

LEARNING
  learn.patterns      View usage statistics
  learn.recommend     Get personalized suggestions

CREATIVITY
  create.overview     Generate system summary
  create.cheatsheet   This cheat-sheet

FLOWS
  conductor.flows     List available workflows
  conductor.run       Execute multi-step flow

ETHICS
  ethics.status       Check ethics engine state
  ethics.evaluate     Dry-run ethics check

CONTRIBUTIONS
  contrib.list        Show stored ideas
  contrib.add         Submit new idea
  contrib.show        View contribution details
```

---

### Flow Orchestration

#### List Available Flows
```
embraced> conductor.flows
```
**Output:**
```
Available Flows:
  
system.full-overview
  Steps: 4
  Duration: ~2s
  Description: Complete system diagnostic and summary
  
system.diagnostics
  Steps: 2  
  Duration: ~1s
  Description: Quick health check
```

#### Run a Flow
```
embraced> conductor.run system.full-overview
```
**Output:**
```
Flow: system.full-overview
Mode: ADVISORY (non-blocking)

Step 1/4: os.selftest
  ✅ L1 Runtime: OK
  ✅ L8 Vault: OK
  ✅ L12 Ethics: OK
  Ethics: ALLOW (low-risk system query)
  
Step 2/4: os.status
  System Status: OPERATIONAL
  Ethics: ALLOW (low-risk system query)
  
Step 3/4: learn.patterns
  Usage Statistics: 21 actions tracked
  Ethics: ALLOW (read-only analytics)
  
Step 4/4: create.overview
  Overview generated (247 chars)
  Ethics: ALLOW (deterministic content generation)

Flow complete: 4/4 steps executed
Total time: 1.84s
```

---

### Ethics & Compliance

#### Ethics Status
```
embraced> ethics.status
```
**Output:**
```
Ethics Engine Status: ACTIVE
Mode: ADVISORY (non-blocking)
Last evaluation: 3s ago

Recent Decisions:
  ✅ os.version → ALLOW (low-risk system query)
  ✅ learn.patterns → ALLOW (read-only analytics)
  ✅ create.overview → ALLOW (deterministic generation)

Risk Categories:
  LOW_RISK: 18 actions
  MEDIUM_RISK: 0 actions
  HIGH_RISK: 0 actions
```

#### Dry-Run Ethics Check
```
embraced> ethics.evaluate ai.think test query
```
**Output:**
```
Ethics Evaluation (dry-run):
Command: ai.think test query
Category: MEDIUM_RISK
Decision: ALLOW_WITH_WARNING
Reasoning: AI invocation with user oversight; transparent local execution
```

---

### Contributions

#### List Ideas
```
embraced> contrib.list
```
**Output:**
```
Stored Contributions:
  [1] Desktop GUI theme customization
  [2] Export vault to encrypted backup
  [3] Voice command interface

Total: 3 contributions
```

#### Add New Idea
```
embraced> contrib.add Plugin marketplace|Community extension system
```
**Output:**
```
Contribution stored:
  ID: 4
  Title: Plugin marketplace
  Description: Community extension system
  Timestamp: 2025-11-17 01:48:00
```

#### View Contribution
```
embraced> contrib.show 4
```
**Output:**
```
Contribution #4
Title: Plugin marketplace
Description: Community extension system
Submitted: 2025-11-17 01:48:00
Status: PENDING_REVIEW
```

---

### AI Integration (Local)

#### Natural Language Query
```
embraced> ai.think how does the ethics engine work?
```
**Output:**
```
The ethics engine (L12) evaluates every action before execution.

Process:
1. Receives command from L1 Runtime
2. Categorizes risk level (LOW/MEDIUM/HIGH)
3. Applies policy rules
4. Generates decision with reasoning
5. Returns to runtime for logging

Mode: ADVISORY (non-blocking in v0.1)
Transparency: Full decision logs in vault
```

---

### Memory & Notes

#### Store Note
```
embraced> memory.note demo tested successfully
```
**Output:**
```
Note stored in vault.
Namespace: notes
Key: note_1731814080
Content: demo tested successfully
```

#### Retrieve Note
```
embraced> memory.note get demo
```
**Output:**
```
Matching notes:
  [1] demo tested successfully (2s ago)
```

#### List All Notes
```
embraced> memory.note list
```
**Output:**
```
All stored notes:
  [1] demo tested successfully
  [2] meeting on Monday
  [3] v0.1.0-alpha released

Total: 3 notes
```

---

## Desktop GUI Features

The desktop interface provides:

**Top Bar:**
- Version button
- Self-Test button
- Help button
- Clear console
- Exit

**Left Sidebar** (Quick Actions):
- **SYSTEM**: Status, Version, Self-Test
- **LEARNING**: Usage Patterns, Recommendations
- **CREATIVITY**: Overview, Cheat-Sheet
- **FLOWS**: List Flows, Full Overview Flow
- **ETHICS**: Ethics Status
- **CONTRIBUTIONS**: List Ideas

**Main Console:**
- Color-coded output
- Command history (↑/↓ arrows)
- Blinking cursor with terminal glow
- Purple accent theme

**Bottom Status Bar:**
- Left: Last command + execution status
- Right: Real-time ethics level + reasoning

**Live Ethics Tracking:**
Every sidebar button click or typed command shows ethics decision instantly in status bar.

---

## Sample Session

```
embraced> os.version
Version: v0.1.0-alpha (commit: ee7716b2)
Architecture: 14-layer AI-native EGAE
Layers: L1-L14 ✅

embraced> os.selftest
✅ 3/3 checks PASSED

embraced> learn.patterns
Usage: os.version (47x), os.status (23x)

embraced> conductor.run system.diagnostics
Step 1/2: os.selftest → ✅
Step 2/2: os.status → ✅
Flow complete: 2/2 steps (0.94s)

embraced> ethics.status
Ethics Engine: ACTIVE
Recent: 4 ALLOW decisions (all low-risk)

embraced> contrib.add Better docs|Expand user guide
Contribution #5 stored

embraced> memory.note session complete
Note stored
```

---

## Key Takeaways

**What you see:**
- Natural language commands
- Structured, deterministic outputs
- Real-time ethics tracking
- Full decision transparency
- Local-only execution

**What you don't see:**
- Cloud API calls (there are none)
- Hidden background processes (event spine is transparent)
- Black box decisions (every action logged + explained)
- User profiling (analytics track actions, not people)

**This is ethical AI in action.**

---

## Questions?

For partnership, licensing, or investment inquiries:

**Email**: michael.sthigpen@gmail.com  
**Support**: https://paypal.me/michaelsthigpen

---

**AHD - Embraced AI • ©2025 AngelHeart Designs**

Built with principles. Designed for trust. Powered by 14 layers.
