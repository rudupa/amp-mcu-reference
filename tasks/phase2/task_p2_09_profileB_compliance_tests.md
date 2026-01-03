# Task: Phase 2 - Profile B Compliance Tests

Status: Pending

Description: Build a compliance test suite for Profile B (isolation + lifecycle) to validate memory, peripheral, and lifecycle policies.

Plan:
- Define compliance criteria for Profile B (isolation rules, lifecycle transitions, resource partitioning).
- Implement automated tests for memory/IRQ/peripheral isolation (positive and negative cases).
- Add lifecycle tests covering start/stop/reset flows and invalid transitions.
- Integrate tests into CI targets; provide hardware selection/skip controls.
- Generate a compliance report artifact summarizing pass/fail and coverage.
- Document how to run and interpret the Profile B compliance suite.

Coding Agent Prompt:
1. Understand the task scope and constraints.
2. Follow the plan above.
3. Create or modify required files in the repo.
4. Add or update documentation as specified by the task.
5. Build or lint the project to validate changes.
6. Prepare a pull request description summarizing work and verification.
