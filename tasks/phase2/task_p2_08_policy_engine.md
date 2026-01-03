# Task: Phase 2 - Lightweight Policy Engine

Status: Pending

Description: Add a lightweight policy engine to apply isolation and lifecycle rules from a declarative profile for Profile B.

Plan:
- Define a minimal policy format (YAML/JSON) for isolation, resource ownership, and lifecycle hooks.
- Implement parser/validator and convert policies into runtime tables consumed by the boot manager.
- Enforce policies during domain start/stop/reset; add logging and denial paths for violations.
- Provide configuration switches and defaults for common MCU targets.
- Add tests covering valid/invalid policies and runtime enforcement scenarios.
- Document policy schema, examples, and integration steps.

Coding Agent Prompt:
1. Understand the task scope and constraints.
2. Follow the plan above.
3. Create or modify required files in the repo.
4. Add or update documentation as specified by the task.
5. Build or lint the project to validate changes.
6. Prepare a pull request description summarizing work and verification.
