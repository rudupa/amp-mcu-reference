# AMP MCU Task Index

## Phase 1 – Minimal AMP Bring-Up (Fast Path)
- Pending: [phase1/task_p1_01_core0_zephyr.md](phase1/task_p1_01_core0_zephyr.md)
- Pending: [phase1/task_p1_02_second_image.md](phase1/task_p1_02_second_image.md)
- Pending: [phase1/task_p1_03_core1_bringup.md](phase1/task_p1_03_core1_bringup.md)
- Pending: [phase1/task_p1_04_memory_layout.md](phase1/task_p1_04_memory_layout.md)
- Pending: [phase1/task_p1_05_boot_core1.md](phase1/task_p1_05_boot_core1.md)
- Pending: [phase1/task_p1_06_core1_handling.md](phase1/task_p1_06_core1_handling.md)
- Pending: [phase1/task_p1_07_shared_memory.md](phase1/task_p1_07_shared_memory.md)
- Bonus docs: [phase1/task_phase1_diagrams.md](phase1/task_phase1_diagrams.md)
- Completed: None yet.

## Phase 2 – Structured AMP Boot Manager (Inside Zephyr)
- Pending: [phase2/task_p2_01_boot_manager_module.md](phase2/task_p2_01_boot_manager_module.md)
- Pending: [phase2/task_p2_02_domain_struct.md](phase2/task_p2_02_domain_struct.md)
- Pending: [phase2/task_p2_03_domain_table.md](phase2/task_p2_03_domain_table.md)
- Pending: [phase2/task_p2_04_lifecycle_hooks.md](phase2/task_p2_04_lifecycle_hooks.md)
- Pending: [phase2/task_p2_05_error_handling.md](phase2/task_p2_05_error_handling.md)
- Additional enhancement: [phase2/task_priority_mailbox.md](phase2/task_priority_mailbox.md)
- Additional documentation: [phase2/task_porting_guides.md](phase2/task_porting_guides.md)
- Completed: None yet.

## Phase 3 – IPC + Lifecycle Integration
- Pending: [phase3/task_p3_01_mailbox_driver.md](phase3/task_p3_01_mailbox_driver.md)
- Pending: [phase3/task_p3_02_shared_memory_ipc.md](phase3/task_p3_02_shared_memory_ipc.md)
- Pending: [phase3/task_p3_03_lifecycle_events.md](phase3/task_p3_03_lifecycle_events.md)
- Pending: [phase3/task_p3_04_debug_endpoints.md](phase3/task_p3_04_debug_endpoints.md)
- Completed: None yet.

## Phase 4 – Standard-Aligned Reference Implementation
- Pending: [phase4/task_p4_01_json_schema.md](phase4/task_p4_01_json_schema.md)
- Pending: [phase4/task_p4_02_domain_loader.md](phase4/task_p4_02_domain_loader.md)
- Pending: [phase4/task_p4_03_domain_manifest.md](phase4/task_p4_03_domain_manifest.md)
- Pending: [phase4/task_p4_04_boot_flow_docs.md](phase4/task_p4_04_boot_flow_docs.md)
- Pending: [phase4/task_p4_05_publish_reference.md](phase4/task_p4_05_publish_reference.md)
- Completed: None yet.

## How to Run a Task (single-session scope)
1. Choose a pending task for the target phase.
2. Write a brief plan (bullets, 5-8 steps).
3. Create or modify the required files in the repo.
4. Add or update documentation as specified by the task.
5. Build or lint the project to validate changes.
6. Prepare a pull request description summarizing work and verification.
