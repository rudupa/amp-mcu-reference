# Contributing to AMP Platform Reference

This repository is designed for a hybrid workflow where humans define the
architecture and AI coding agents generate implementation, documentation, and
examples. Contributions from both humans and agents are welcome.

---

## Contribution Model

### 1. Architecture and Semantics (Human‑Led)
Humans define:
- AMP profiles (A/B/C/D)
- boot semantics and domain configuration
- IPC primitives and correctness rules
- isolation and policy models
- safety/cybersecurity requirements

These decisions form the stable contract for all implementations.

---

### 2. Implementation and Documentation (Agent‑Friendly)
Coding agents are encouraged to:
- generate code for runtime modules
- implement IPC primitives
- create examples and tests
- scaffold platform ports
- write documentation pages
- update diagrams and metadata

Tasks should be small, scoped, and self‑contained.

---

## How to Contribute

### Step 1 — Pick or Create an Issue
Issues are labeled for clarity:
- `phase1`, `phase2`, `phase3`, `phase4`
- `ipc`, `boot`, `isolation`, `rtos`, `safety`
- `agent-task` (safe for autonomous execution)

If creating a new issue, include:
- goal
- files to modify/create
- functional requirements
- acceptance criteria

---

### Step 2 — Use the Agent Task Template

Use this template for any task intended for autonomous execution by a coding agent:

# Contributing to AMP Platform Reference

This repository is designed for a hybrid workflow where humans define the
architecture and AI coding agents generate implementation, documentation, and
examples. Contributions from both humans and agents are welcome.

---

## Contribution Model

### 1. Architecture and Semantics (Human‑Led)
Humans define:
- AMP profiles (A/B/C/D)
- boot semantics and domain configuration
- IPC primitives and correctness rules
- isolation and policy models
- safety/cybersecurity requirements

These decisions form the stable contract for all implementations.

---

### 2. Implementation and Documentation (Agent‑Friendly)
Coding agents are encouraged to:
- generate code for runtime modules
- implement IPC primitives
- create examples and tests
- scaffold platform ports
- write documentation pages
- update diagrams and metadata

Tasks should be small, scoped, and self‑contained.

---

## How to Contribute

### Step 1 — Pick or Create an Issue
Issues are labeled for clarity:
- `phase1`, `phase2`, `phase3`, `phase4`
- `ipc`, `boot`, `isolation`, `rtos`, `safety`
- `agent-task` (safe for autonomous execution)

If creating a new issue, include:
- goal
- files to modify/create
- functional requirements
- acceptance criteria

---

### Step 2 — Use the Agent Task Template

Use this template for any task intended for autonomous execution by a coding agent:

Goal:
- What the task should accomplish.
Files:
- List of files to create or modify.
Inputs/Outputs:
- Inputs the module receives.
- Outputs it must produce.
Requirements:
- Functional requirements.
- Constraints (determinism, no dynamic allocation, etc.).
Acceptance Criteria:
- Conditions that must be met for the PR to be accepted.

Agents should produce a PR that fully satisfies the criteria.

---

### Step 3 — Submit a Pull Request
PRs should:
- reference the issue
- include generated code/docs
- pass CI
- include a brief summary of changes

Humans review for:
- correctness
- determinism
- architectural alignment

---

## Coding Style and Structure

- C code must be deterministic and allocation‑free.
- All shared memory structures must be explicitly documented.
- IPC primitives must follow the AMP minimal contract.
- Examples must be reproducible on supported boards.
- Documentation must live under `docs/`.

---

## Multi‑Phase Structure

- **Phase 1:** Minimal AMP contract  
- **Phase 2:** Isolation & policies  
- **Phase 3:** RTOS integration  
- **Phase 4:** Safety & cybersecurity  

Each phase builds on the previous one. Contributions should specify which phase they target.

---

## Platform Support

Board support roadmap (summary):
- Initial boards: RP2040, RP2350, PolarFire SoC Icicle Kit (if available)
- Planned boards: STM32H7 dual-core, TI AM243x, TI AM64x, NXP i.MX 8M Mini/Plus, NXP S32K3, Infineon AURIX TC3xx, Renesas RH850

Phase-by-phase board plan:
- Phase 1 (Minimal AMP Contract, Profile A): initial RP2040, RP2350; planned STM32H7 dual-core
- Phase 2 (Isolation, Policies, Lifecycle, Profile B): initial RP2350, PolarFire SoC; planned TI AM243x, STM32H7, NXP S32K3
- Phase 3 (RTOS Integration + Hybrid SMP/AMP, Profile C): initial PolarFire SoC; planned TI AM64x, NXP i.MX 8M Mini/Plus
- Phase 4 (Safety & Cybersecurity Profiles, Profile D): initial RP2350, PolarFire SoC; planned NXP S32K3, Infineon AURIX TC3xx, Renesas RH850

Platform ports must include:
- memory map
- boot notes
- IPC driver notes
- example validation

---

## Planned Repository Layout (for profiles + boards)

Planned top-level structure to keep profiles and platforms isolated and discoverable:
- main/
- profiles/
	- profile_a/
	- profile_b/
	- profile_c/
	- profile_d/
- platforms/
	- rp2350/
	- rp2040/
	- polarfire/
	- am64x/
	- s32k3/
	- aurix/
	- ...

Why this helps:
- Profiles evolve independently while boards map cleanly to profiles.
- Avoids fragmentation and long-lived branches.
- Contributors know exactly where to add or update support.

---

## Thank You

This project aims to become the canonical reference for vendor‑neutral AMP on MCUs.
Your contributions—human or agent—help move the standard forward.