# Task: Phase 3 - Add Domain Lifecycle Events

Status: Pending

Description: Add domain lifecycle events (started, alive heartbeat, faulted, stopped) and wire them into IPC or logging.

Plan:
- Define lifecycle event types and payloads (started, alive/heartbeat, domain faulted, domain stopped, domain booted).
- Implement event emission points in the boot manager and IPC layers.
- Add a lightweight consumer (logger or monitor) to record lifecycle events.
- Provide a heartbeat mechanism to detect liveness across domains.
- Create tests or demos that exercise lifecycle events under normal and fault cases.
- Document the lifecycle event model and expected consumers.

Coding Agent Prompt:
1. Understand the task scope and constraints.
2. Follow the plan above.
3. Create or modify required files in the repo.
4. Add or update documentation as specified by the task.
5. Build or lint the project to validate changes.
6. Prepare a pull request description summarizing work and verification.
