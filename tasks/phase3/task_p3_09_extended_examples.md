# Task: Phase 3 - Extended Examples (Zephyr + Bare-Metal)

Status: Pending

Description: Build extended examples demonstrating Zephyr on Core0 with bare-metal or alternate RTOS on Core1, covering IPC and lifecycle flows.

Plan:
- Create example pairing Zephyr (Core0) with bare-metal Core1 using mailbox/semaphore IPC and shared memory.
- Add variant with Zephyr (Core0) plus second RTOS or lightweight loop on Core1 to show hybrid scheduling.
- Include lifecycle hooks (start/stop/reset) and readiness signals in examples.
- Provide build targets and run scripts for supported boards (RP2350, PolarFire, STM32H7 if available).
- Capture expected logs/telemetry and document verification steps.
- Document example structure, configuration overlays, and limitations.

Coding Agent Prompt:
1. Understand the task scope and constraints.
2. Follow the plan above.
3. Create or modify required files in the repo.
4. Add or update documentation as specified by the task.
5. Build or lint the project to validate changes.
6. Prepare a pull request description summarizing work and verification.
