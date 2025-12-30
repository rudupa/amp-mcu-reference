# Task: Phase 1 - Boot Core1 from Core0

Status: Pending

Description: Write vector release, stack, and entry values from Core 0 to start Core 1 and verify the second core runs independently.

Plan:
- Implement the Core 0 routine that writes Core 1 vector release, stack, and entry values.
- Add any required synchronization (delays or flags) before releasing Core 1.
- Boot Core 1 and monitor activity via UART/GPIO to confirm execution.
- Add minimal logging for success/failure and capture timing notes.
- Validate integration with the chosen memory layout and bring-up functions.
- Document the boot sequence steps for reference.

Coding Agent Prompt:
1. Understand the task scope and constraints.
2. Follow the plan above.
3. Create or modify required files in the repo.
4. Add or update documentation as specified by the task.
5. Build or lint the project to validate changes.
6. Prepare a pull request description summarizing work and verification.
