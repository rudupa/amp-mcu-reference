# Task: Phase 1 - Add Simple Shared Memory Region

Status: Pending

Description: Reserve a small shared RAM block and implement a trivial mailbox or flag for minimal shared communication between cores.

Plan:
- Reserve a small shared memory block in RAM for inter-core communication.
- Implement a simple mailbox or flag protocol for Core 0 and Core 1 to exchange a value.
- Add memory barriers or volatile access as needed for correctness.
- Integrate a tiny send/receive demo in both cores to prove data moves.
- Validate that the shared region does not overlap with code or stacks.
- Document the shared region address and usage.

Coding Agent Prompt:
1. Understand the task scope and constraints.
2. Follow the plan above.
3. Create or modify required files in the repo.
4. Add or update documentation as specified by the task.
5. Build or lint the project to validate changes.
6. Prepare a pull request description summarizing work and verification.
