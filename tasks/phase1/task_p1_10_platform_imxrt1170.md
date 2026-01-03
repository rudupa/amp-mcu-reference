# Task: Phase 1 - i.MX RT1170 Platform Expansion

Status: Pending

Description: Port Profile A AMP baseline to NXP i.MX RT1170 dual-core (M7+M4): deterministic boot, shared memory, and minimal IPC primitives.

Plan:
- Define i.MX RT1170 memory map (TCM/OCRAM/AXI) and shared region; set reset vectors and stacks for both cores.
- Add CMake platform file and toolchain settings; provide platform overrides for boot and barriers.
- Implement secondary-core bring-up (M7→M4) with release registers and synchronization.
- Adapt shared memory allocator, mailbox, and semaphore wrappers with cache/AXI considerations.
- Build hello-amp, pingpong, shared-counter for RT1170; verify on hardware or emulation and capture logs.
- Document platform notes, cache/coherency requirements, and known limitations.

Coding Agent Prompt:
1. Understand the task scope and constraints.
2. Follow the plan above.
3. Create or modify required files in the repo.
4. Add or update documentation as specified by the task.
5. Build or lint the project to validate changes.
6. Prepare a pull request description summarizing work and verification.
