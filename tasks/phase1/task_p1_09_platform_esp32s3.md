# Task: Phase 1 - ESP32-S3 Platform Expansion

Status: Pending

Description: Port the minimal Profile A AMP stack to ESP32-S3 dual-core (Xtensa) using bare-metal or ESP-IDF minimal runtime for deterministic boot and IPC primitives.

Plan:
- Map ESP32-S3 memory regions for Core0/Core1/shared; define reset/entry vectors and stack placements.
- Add CMake/ESP-IDF build integration and platform config; stub platform overrides for boot and barriers.
- Implement secondary-core boot and synchronization flow; ensure deterministic release semantics.
- Adapt shared memory allocator and mailbox/semaphore wrappers with cache coherency handling.
- Build and exercise hello-amp, pingpong, shared-counter on ESP32-S3; record expected serial output.
- Document platform notes, cache/barrier requirements, and constraints for Phase 1.

Coding Agent Prompt:
1. Understand the task scope and constraints.
2. Follow the plan above.
3. Create or modify required files in the repo.
4. Add or update documentation as specified by the task.
5. Build or lint the project to validate changes.
6. Prepare a pull request description summarizing work and verification.
