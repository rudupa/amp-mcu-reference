# Task: Phase 3 - FreeRTOS Integration

Status: Pending

Description: Provide a FreeRTOS integration path for the AMP platform reference, aligning IPC and lifecycle with RTOS primitives.

Plan:
- Add build glue to consume AMP runtime from FreeRTOS-based projects.
- Implement FreeRTOS-compatible wrappers/adapters for mailbox, semaphores, and shared memory synchronization.
- Provide boot/lifecycle hooks that coordinate with FreeRTOS startup on Core0 and a bare-metal or RTOS Core1.
- Create a sample demonstrating IPC between a FreeRTOS domain and a bare-metal/second RTOS domain.
- Validate on at least one supported board (e.g., RP2350) and capture logs.
- Document integration steps, configuration options, and limitations.

Coding Agent Prompt:
1. Understand the task scope and constraints.
2. Follow the plan above.
3. Create or modify required files in the repo.
4. Add or update documentation as specified by the task.
5. Build or lint the project to validate changes.
6. Prepare a pull request description summarizing work and verification.
