# Task: Phase 3 - Implement Mailbox Driver

Status: Pending

Description: Implement a mailbox driver using RP2040/RP2350 hardware semaphores or mailboxes to support inter-core messaging.

Plan:
- Review available hardware mailboxes/semaphores on RP2040/RP2350 and choose the mechanism.
- Design a minimal mailbox driver API suited for inter-core messages.
- Implement send/receive paths with basic flow control.
- Add synchronization (barriers/IRQs) as required by the hardware.
- Create a smoke test or sample exchanging messages between cores.
- Document usage and configuration knobs.

Coding Agent Prompt:
1. Understand the task scope and constraints.
2. Follow the plan above.
3. Create or modify required files in the repo.
4. Add or update documentation as specified by the task.
5. Build or lint the project to validate changes.
6. Prepare a pull request description summarizing work and verification.
