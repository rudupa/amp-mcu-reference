# Task: Phase 1 - STM32H7 Platform Expansion

Status: Pending

Description: Bring up the minimal Profile A AMP stack on STM32H7 dual-core MCU (M7+M4): boot handoff, shared memory, mailbox/semaphore basics, and validation examples.

Plan:
- Define STM32H7 memory map and shared region for Profile A; document boot/reset vectors for both cores.
- Add CMake platform entry and toolchain tweaks for STM32H7; wire minimal BSP stubs.
- Implement core boot handoff (Core0→Core1) with vector release and synchronization barriers.
- Adapt shared memory allocator, mailbox, semaphore wrappers to STM32H7 constraints (cache/TCM as needed).
- Build and run hello-amp, pingpong, and shared-counter on STM32H7; capture logs.
- Document platform notes and known limitations for Phase 1.

Coding Agent Prompt:
1. Understand the task scope and constraints.
2. Follow the plan above.
3. Create or modify required files in the repo.
4. Add or update documentation as specified by the task.
5. Build or lint the project to validate changes.
6. Prepare a pull request description summarizing work and verification.
