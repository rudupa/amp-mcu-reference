# amp-mcu-reference
Vendor‑neutral AMP reference implementation for dual‑core MCUs — deterministic boot, domain config, minimal IPC, and reproducible examples (Phase 1).

## 📋 Task Documentation

This repository contains actionable task descriptions for enhancing and documenting the AMP MCU reference implementation.

### Quick Start
- **[TASK_INDEX.md](./TASK_INDEX.md)** - Master index of all tasks with selection guide

### Available Tasks

1. **Priority-Based Message Scheduling** (Phase 2 Enhancement)
   - **[TASK_DESCRIPTION.md](./TASK_DESCRIPTION.md)** - Complete specification
   - **[TASK_SUMMARY.md](./TASK_SUMMARY.md)** - Quick reference
   - Scope: ~10 hours | Extends existing amp_mailbox with priority support
   - Addresses Phase 1 limitation: "No priority-based scheduling"

2. **Phase 1 Architecture Diagrams** (Documentation)
   - **[TASK_PHASE1_DIAGRAMS.md](./TASK_PHASE1_DIAGRAMS.md)** - Complete specification
   - Scope: ~11 hours | Create visual documentation (PlantUML/SVG)
   - Deliverables: Architecture, boot sequence, memory layout, IPC flow diagrams

3. **Porting Guides for RP2040 and ESP32-S3** (Platform Expansion)
   - **[TASK_PORTING_GUIDES.md](./TASK_PORTING_GUIDES.md)** - Complete specification
   - Scope: ~17 hours | Comprehensive guides for new platforms
   - Deliverables: RP2040 guide, ESP32-S3 guide, generic porting template

### What Already Exists (Phase 1 - Main Branch)
The main branch contains a complete Phase 1 implementation:
- ✅ Core boot and handoff (`amp_boot`)
- ✅ Shared memory ring buffer (`amp_ringbuf`)
- ✅ Mailbox IPC (`amp_mailbox`)
- ✅ Semaphores (`amp_semaphore`)
- ✅ Three working examples (hello-amp, pingpong, shared-counter)

See [TASK_INDEX.md](./TASK_INDEX.md) for full details on what exists vs. what these tasks add.
