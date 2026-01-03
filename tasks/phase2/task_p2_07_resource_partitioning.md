# Task: Phase 2 - Resource Partitioning

Status: Pending

Description: Partition memory, interrupts, and peripherals across domains with declarative ownership and enforcement.

Plan:
- Extend domain table/schema to capture resource ownership (memory ranges, IRQs, peripherals, shared flags).
- Implement validation to prevent overlaps and to flag shared resources explicitly.
- Add boot-time configuration to route interrupts and peripheral clocks/resets per domain where supported.
- Provide helper APIs for querying ownership and enforcing access checks in runtime components.
- Create examples/tests showing partitioned resources and safe shared resources.
- Document the partitioning model, constraints, and escalation paths for violations.

Coding Agent Prompt:
1. Understand the task scope and constraints.
2. Follow the plan above.
3. Create or modify required files in the repo.
4. Add or update documentation as specified by the task.
5. Build or lint the project to validate changes.
6. Prepare a pull request description summarizing work and verification.
