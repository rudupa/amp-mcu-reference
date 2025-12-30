# Task: Phase 2 - Define Minimal Domain Struct

Status: Pending

Description: Define a minimal domain struct with core id, entry address, stack base/size, and shared memory base to support the boot manager.

Plan:
- Design the minimal domain struct fields (core_id, entry, t_stack, t_tstack, shmem_base/size).
- Add the struct definition to a shared header for boot manager and callers.
- Populate an initial domain instance for Core 1 using the Phase 1 layout.
- Wire the struct usage into the boot manager API and validation.
- Add a small test or example showing domain struct consumption.
- Document the struct fields and constraints.

Coding Agent Prompt:
1. Understand the task scope and constraints.
2. Follow the plan above.
3. Create or modify required files in the repo.
4. Add or update documentation as specified by the task.
5. Build or lint the project to validate changes.
6. Prepare a pull request description summarizing work and verification.
