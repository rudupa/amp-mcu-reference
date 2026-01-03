# Task: Phase 3 - Multi-Domain Orchestration

Status: Pending

Description: Add orchestration for multiple domains, including sequencing, dependency handling, and monitoring across mixed profiles.

Plan:
- Extend domain table to express dependencies and startup order; add readiness signals per domain.
- Implement orchestrator that starts domains in order, waits for readiness, and handles failures with retries/teardown.
- Add monitoring hooks (heartbeats/events) to track domain liveness.
- Provide CLI/logging to visualize domain states and transitions.
- Create tests/demos with 3+ domains (e.g., Zephyr + bare-metal + service domain).
- Document orchestration model, configuration options, and recovery behavior.

Coding Agent Prompt:
1. Understand the task scope and constraints.
2. Follow the plan above.
3. Create or modify required files in the repo.
4. Add or update documentation as specified by the task.
5. Build or lint the project to validate changes.
6. Prepare a pull request description summarizing work and verification.
