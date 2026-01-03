# AMP MCU Task Index

## Phase 1 – Minimal AMP Bring-Up (Fast Path)
- Pending: [phase1/task_p1_01_core0_zephyr.md](phase1/task_p1_01_core0_zephyr.md)
- Pending: [phase1/task_p1_02_second_image.md](phase1/task_p1_02_second_image.md)
- Pending: [phase1/task_p1_03_core1_bringup.md](phase1/task_p1_03_core1_bringup.md)
- Pending: [phase1/task_p1_04_memory_layout.md](phase1/task_p1_04_memory_layout.md)
- Pending: [phase1/task_p1_05_boot_core1.md](phase1/task_p1_05_boot_core1.md)
- Pending: [phase1/task_p1_06_core1_handling.md](phase1/task_p1_06_core1_handling.md)
- Pending: [phase1/task_p1_07_shared_memory.md](phase1/task_p1_07_shared_memory.md)
- Pending: [phase1/task_p1_08_platform_stm32h7.md](phase1/task_p1_08_platform_stm32h7.md)
- Pending: [phase1/task_p1_09_platform_esp32s3.md](phase1/task_p1_09_platform_esp32s3.md)
- Pending: [phase1/task_p1_10_platform_imxrt1170.md](phase1/task_p1_10_platform_imxrt1170.md)
- Bonus docs: [phase1/task_phase1_diagrams.md](phase1/task_phase1_diagrams.md)
- Completed: None yet.

## Phase 2 – Structured AMP Boot Manager (Inside Zephyr)
- Pending: [phase2/task_p2_01_boot_manager_module.md](phase2/task_p2_01_boot_manager_module.md)
- Pending: [phase2/task_p2_02_domain_struct.md](phase2/task_p2_02_domain_struct.md)
- Pending: [phase2/task_p2_03_domain_table.md](phase2/task_p2_03_domain_table.md)
- Pending: [phase2/task_p2_04_lifecycle_hooks.md](phase2/task_p2_04_lifecycle_hooks.md)
- Pending: [phase2/task_p2_05_error_handling.md](phase2/task_p2_05_error_handling.md)
- Pending: [phase2/task_p2_06_memory_peripheral_isolation.md](phase2/task_p2_06_memory_peripheral_isolation.md)
- Pending: [phase2/task_p2_07_resource_partitioning.md](phase2/task_p2_07_resource_partitioning.md)
- Pending: [phase2/task_p2_08_policy_engine.md](phase2/task_p2_08_policy_engine.md)
- Pending: [phase2/task_p2_09_profileB_compliance_tests.md](phase2/task_p2_09_profileB_compliance_tests.md)
- Additional enhancement: [phase2/task_priority_mailbox.md](phase2/task_priority_mailbox.md)
- Additional documentation: [phase2/task_porting_guides.md](phase2/task_porting_guides.md)
- Completed: None yet.

## Phase 3 – IPC + Lifecycle Integration
- Pending: [phase3/task_p3_01_mailbox_driver.md](phase3/task_p3_01_mailbox_driver.md)
- Pending: [phase3/task_p3_02_shared_memory_ipc.md](phase3/task_p3_02_shared_memory_ipc.md)
- Pending: [phase3/task_p3_03_lifecycle_events.md](phase3/task_p3_03_lifecycle_events.md)
- Pending: [phase3/task_p3_04_debug_endpoints.md](phase3/task_p3_04_debug_endpoints.md)
- Pending: [phase3/task_p3_05_zephyr_integration.md](phase3/task_p3_05_zephyr_integration.md)
- Pending: [phase3/task_p3_06_freertos_integration.md](phase3/task_p3_06_freertos_integration.md)
- Pending: [phase3/task_p3_07_hybrid_smp_amp_scheduler.md](phase3/task_p3_07_hybrid_smp_amp_scheduler.md)
- Pending: [phase3/task_p3_08_multi_domain_orchestration.md](phase3/task_p3_08_multi_domain_orchestration.md)
- Pending: [phase3/task_p3_09_extended_examples.md](phase3/task_p3_09_extended_examples.md)
- Completed: None yet.

## Phase 4 – Standard-Aligned Reference Implementation
- Pending: [phase4/task_p4_01_json_schema.md](phase4/task_p4_01_json_schema.md)
- Pending: [phase4/task_p4_02_domain_loader.md](phase4/task_p4_02_domain_loader.md)
- Pending: [phase4/task_p4_03_domain_manifest.md](phase4/task_p4_03_domain_manifest.md)
- Pending: [phase4/task_p4_04_boot_flow_docs.md](phase4/task_p4_04_boot_flow_docs.md)
- Pending: [phase4/task_p4_05_publish_reference.md](phase4/task_p4_05_publish_reference.md)
- Pending: [phase4/task_p4_06_safety_profile_definition.md](phase4/task_p4_06_safety_profile_definition.md)
- Pending: [phase4/task_p4_07_watchdog_supervision.md](phase4/task_p4_07_watchdog_supervision.md)
- Pending: [phase4/task_p4_08_traceability_matrix.md](phase4/task_p4_08_traceability_matrix.md)
- Pending: [phase4/task_p4_09_compliance_test_suite.md](phase4/task_p4_09_compliance_test_suite.md)
- Pending: [phase4/task_p4_10_safety_docs.md](phase4/task_p4_10_safety_docs.md)
- Pending: [phase4/task_p4_11_cybersecurity_docs.md](phase4/task_p4_11_cybersecurity_docs.md)
- Completed: None yet.

## How to Run a Task (single-session scope)
1. Choose a pending task for the target phase.
2. Write a brief plan (bullets, 5-8 steps).
3. Create or modify the required files in the repo.
4. Add or update documentation as specified by the task.
5. Build or lint the project to validate changes.
6. Prepare a pull request description summarizing work and verification.
