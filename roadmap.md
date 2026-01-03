# AMP Platform Reference — Public Roadmap

This repository defines a vendor‑neutral, multi‑phase reference implementation for
Asymmetric Multiprocessing (AMP) on microcontrollers. Each phase builds on the
previous one, evolving from a minimal contract to safety‑ready profiles suitable
for industrial, automotive, and IoT systems.

---

## Phase 1 — Minimal AMP Contract (Profile A)
**Status:** In Progress  
**Goal:** Establish the smallest reproducible AMP baseline for dual‑core MCUs.

### Deliverables
- Deterministic boot flow (Core0 → Core1 handoff)
- Domain configuration schema (`domain.yaml`)
- Shared memory layout + validator
- Minimal IPC primitives:
  - mailbox
  - hardware semaphore wrapper
  - shared‑memory ring buffer
- Example applications:
  - hello‑amp
  - mailbox‑pingpong
  - shared‑memory‑counter
- RP2350 platform notes
- Documentation set (overview, boot flow, IPC, porting guide)
- Basic CI (build + YAML validation)

**Outcome:** A clean, portable Profile A reference implementation.

---

## Phase 2 — Isolation, Policies, and Domain Lifecycle (Profile B)
**Status:** Planned  
**Goal:** Introduce controlled isolation and resource partitioning while keeping the system MCU‑friendly.

### Deliverables
- Memory and peripheral isolation (MPU/PMP/TZ‑M)
- Domain lifecycle management (start/stop/reset)
- Resource partitioning (memory, interrupts, peripherals)
- Lightweight policy engine
- Extended domain schema (isolation levels, resource ownership)
- Compliance tests for Profile B
- Examples demonstrating isolation and recovery

**Outcome:** A robust, deterministic Profile B suitable for industrial MCUs.

---

## Phase 3 — RTOS Integration + Hybrid SMP/AMP (Profile C)
**Status:** Planned  
**Goal:** Bridge MCU AMP semantics with RTOS ecosystems and SoC‑class hybrid architectures.

### Deliverables
- Zephyr integration (drivers, shared memory, mailbox, semaphores)
- Optional FreeRTOS integration
- Hybrid SMP/AMP scheduling model
- Multi‑domain orchestration
- Extended examples:
  - Zephyr on Core0 + bare‑metal Core1
  - RTOS‑to‑bare‑metal IPC
- Platform expansion:
  - STM32H7
  - ESP32‑S3
  - i.MX RT1170

**Outcome:** A flexible Profile C that spans MCU → SoC boundaries.

---

## Phase 4 — Safety & Cybersecurity Profiles (Profile D)
**Status:** Planned  
**Goal:** Provide a safety‑ready AMP profile aligned with ISO 26262 and ISO 21434.

### Deliverables
- Safety profile definition (ASIL‑B/C‑aligned)
- Deterministic startup + fault containment
- Watchdog‑integrated domain supervision
- Traceability matrix for AMP primitives
- Compliance test suite
- Safety documentation:
  - safety manual
  - hazard analysis (HARA‑style)
  - failure mode examples
- Cybersecurity documentation:
  - threat analysis (TARA)
  - secure IPC profiles
  - domain isolation verification

**Outcome:** A credible Profile D suitable for safety‑critical adoption.

---

## Cross‑Phase Infrastructure (Continuous)
- Multi‑profile directory structure
- Unified build system (CMake)
- CI pipelines (build, lint, tests, compliance)
- Documentation site
- Agent‑friendly tasks + issue templates
- Platform expansion (RP2040, STM32H7, ESP32‑S3, i.MX RT1170, PolarFire)

---

## Vision
This repository aims to become the canonical reference implementation for
vendor‑neutral AMP on microcontrollers — a foundation for research, industry
adoption, and future standardization.