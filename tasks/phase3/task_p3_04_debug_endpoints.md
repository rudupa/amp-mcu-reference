# Task: Phase 3 - Add Debug Endpoints

Status: Pending

Description: Provide debug endpoints (UART per domain, shared memory logs, optional SWO/ITM) to observe IPC and lifecycle behavior.

Plan:
- Select debug transports (UART per domain, shared memory log buffer, optional SWO/ITM on RP2350).
- Implement logging hooks in mailbox/IPC and lifecycle event paths.
- Provide a minimal CLI or log dumper to inspect shared memory logs.
- Add configuration switches to enable/disable debug endpoints.
- Validate logging from both domains under normal traffic.
- Document how to use the debug endpoints during bring-up.

Coding Agent Prompt:
1. Understand the task scope and constraints.
2. Follow the plan above.
3. Create or modify required files in the repo.
4. Add or update documentation as specified by the task.
5. Build or lint the project to validate changes.
6. Prepare a pull request description summarizing work and verification.
