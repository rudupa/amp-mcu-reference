# AMP MCU Roadmap

This roadmap tracks four phases, each with actionable tasks. Use the task links to drive single-session implementation work.

## Phase 1 — Minimal AMP Bring-Up (Fast Path)
- Goal: Bring two cores up independently (Zephyr + bare-metal or Zephyr + Zephyr) with a tiny shared memory channel.
- Tasks: [tasks/phase1/task_p1_01_core0_zephyr.md](tasks/phase1/task_p1_01_core0_zephyr.md), [tasks/phase1/task_p1_02_second_image.md](tasks/phase1/task_p1_02_second_image.md), [tasks/phase1/task_p1_03_core1_bringup.md](tasks/phase1/task_p1_03_core1_bringup.md), [tasks/phase1/task_p1_04_memory_layout.md](tasks/phase1/task_p1_04_memory_layout.md), [tasks/phase1/task_p1_05_boot_core1.md](tasks/phase1/task_p1_05_boot_core1.md), [tasks/phase1/task_p1_06_core1_handling.md](tasks/phase1/task_p1_06_core1_handling.md), [tasks/phase1/task_p1_07_shared_memory.md](tasks/phase1/task_p1_07_shared_memory.md)

## Phase 2 — Structured AMP Boot Manager (Inside Zephyr)
- Goal: Replace ad-hoc bring-up with a reusable boot manager and domain table inside Zephyr.
- Tasks: [tasks/phase2/task_p2_01_boot_manager_module.md](tasks/phase2/task_p2_01_boot_manager_module.md), [tasks/phase2/task_p2_02_domain_struct.md](tasks/phase2/task_p2_02_domain_struct.md), [tasks/phase2/task_p2_03_domain_table.md](tasks/phase2/task_p2_03_domain_table.md), [tasks/phase2/task_p2_04_lifecycle_hooks.md](tasks/phase2/task_p2_04_lifecycle_hooks.md), [tasks/phase2/task_p2_05_error_handling.md](tasks/phase2/task_p2_05_error_handling.md)

## Phase 3 — IPC + Lifecycle Integration
- Goal: Add structured communication and domain lifecycle semantics across domains.
- Tasks: [tasks/phase3/task_p3_01_mailbox_driver.md](tasks/phase3/task_p3_01_mailbox_driver.md), [tasks/phase3/task_p3_02_shared_memory_ipc.md](tasks/phase3/task_p3_02_shared_memory_ipc.md), [tasks/phase3/task_p3_03_lifecycle_events.md](tasks/phase3/task_p3_03_lifecycle_events.md), [tasks/phase3/task_p3_04_debug_endpoints.md](tasks/phase3/task_p3_04_debug_endpoints.md)

## Phase 4 — Standard-Aligned Reference Implementation
- Goal: Produce a publishable, standard-aligned AMP reference with manifests and JSON-driven domains.
- Tasks: [tasks/phase4/task_p4_01_json_schema.md](tasks/phase4/task_p4_01_json_schema.md), [tasks/phase4/task_p4_02_domain_loader.md](tasks/phase4/task_p4_02_domain_loader.md), [tasks/phase4/task_p4_03_domain_manifest.md](tasks/phase4/task_p4_03_domain_manifest.md), [tasks/phase4/task_p4_04_boot_flow_docs.md](tasks/phase4/task_p4_04_boot_flow_docs.md), [tasks/phase4/task_p4_05_publish_reference.md](tasks/phase4/task_p4_05_publish_reference.md)

## Cross-Phase Enhancements
- Priority mailbox enhancement: [tasks/phase2/task_priority_mailbox.md](tasks/phase2/task_priority_mailbox.md)
- Platform porting guides: [tasks/phase2/task_porting_guides.md](tasks/phase2/task_porting_guides.md)
- Phase 1 diagrams (documentation): [tasks/phase1/task_phase1_diagrams.md](tasks/phase1/task_phase1_diagrams.md)

## How to Execute Any Task
1. Understand the task.
2. Follow the plan in the task file.
3. Create or modify required files in the repo.
4. Add or update documentation as specified by the task.
5. Build or lint the project to validate changes.
6. Prepare a pull request description summarizing work and verification.