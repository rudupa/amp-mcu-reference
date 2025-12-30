# Task: Phase 2 - Add Lifecycle Hooks

Status: Pending

Description: Add lifecycle hooks (start, stop, reset) to the boot manager to manage domain lifecycles cleanly.

Plan:
- Define lifecycle hook interfaces for start, stop, and reset operations.
- Integrate hook invocation into the boot manager flow for domains.
- Track domain state transitions and guard against invalid transitions.
- Add minimal logging and metrics for lifecycle events.
- Create a small test/demo invoking lifecycle hooks for a domain.
- Document lifecycle semantics and expected states.

Coding Agent Prompt:
1. Understand the task scope and constraints.
2. Follow the plan above.
3. Create or modify required files in the repo.
4. Add or update documentation as specified by the task.
5. Build or lint the project to validate changes.
6. Prepare a pull request description summarizing work and verification.
