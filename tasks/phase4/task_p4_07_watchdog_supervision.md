# Task: Phase 4 - Watchdog-Integrated Domain Supervision

Status: Pending

Description: Integrate watchdog-based supervision for domains to ensure deterministic startup and fault containment.

Plan:
- Define watchdog supervision model per domain (kick strategy, timeouts, escalation actions).
- Implement watchdog hooks in domain lifecycle (start/ready/heartbeat/fault) with fail-safe defaults.
- Add recovery paths (reset domain, system reset) and logging for supervision events.
- Provide configuration parameters per platform and per domain profile.
- Create tests/demos that simulate missed heartbeats and confirm supervision actions.
- Document supervision model, configuration, and platform caveats.

Coding Agent Prompt:
1. Understand the task scope and constraints.
2. Follow the plan above.
3. Create or modify required files in the repo.
4. Add or update documentation as specified by the task.
5. Build or lint the project to validate changes.
6. Prepare a pull request description summarizing work and verification.
