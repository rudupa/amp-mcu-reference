# Task: Phase 2 - Memory and Peripheral Isolation

Status: Pending

Description: Add Profile B isolation for memory and peripherals using MPU/PMP/TZ-M: region setup, access policies, and validation.

Plan:
- Define isolation policy schema for memory/peripherals (read/write/exec, domain ownership, TZ-M/MPU settings).
- Implement MPU/TZ-M configuration at boot for each domain; apply per-region attributes and fault handlers.
- Add peripheral access guards (whitelist) and shared resource markings; document allowed crossings.
- Integrate isolation checks into boot manager and domain table validation.
- Create tests/demos that prove isolation (positive/negative cases) and log violations.
- Document configuration knobs, defaults, and platform caveats.

Coding Agent Prompt:
1. Understand the task scope and constraints.
2. Follow the plan above.
3. Create or modify required files in the repo.
4. Add or update documentation as specified by the task.
5. Build or lint the project to validate changes.
6. Prepare a pull request description summarizing work and verification.
