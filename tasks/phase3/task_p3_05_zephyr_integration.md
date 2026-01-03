# Task: Phase 3 - Zephyr Integration

Status: Pending

Description: Integrate the AMP platform reference with Zephyr: drivers, shared memory, mailbox/semaphore, and domain lifecycle hooks.

Plan:
- Add Zephyr modules/CMake glue to build AMP runtime as a Zephyr component.
- Implement Zephyr drivers/adapters for mailbox, shared memory, and semaphores using existing runtime.
- Wire boot manager/domain lifecycle hooks into Zephyr init (SYS_INIT) for Core0.
- Provide Zephyr sample(s) demonstrating IPC and domain bring-up.
- Validate with RP2350 (and other supported boards) under Zephyr; capture logs.
- Document integration steps and configuration options.

Coding Agent Prompt:
1. Understand the task scope and constraints.
2. Follow the plan above.
3. Create or modify required files in the repo.
4. Add or update documentation as specified by the task.
5. Build or lint the project to validate changes.
6. Prepare a pull request description summarizing work and verification.
