# Task: Phase 4 - Add Domain Loader

Status: Pending

Description: Add a domain loader that parses JSON domain definitions at build time or embeds them as C structs with validation.

Plan:
- Implement parsing of domain JSON into in-memory structs (build tool or runtime loader).
- Add validation for addresses, sizes, and alignment per schema rules.
- Generate or embed C structs from validated JSON for runtime use.
- Integrate the loader output with the boot manager domain table.
- Create tests that load valid and invalid JSON definitions.
- Document loader usage and integration steps.

Coding Agent Prompt:
1. Understand the task scope and constraints.
2. Follow the plan above.
3. Create or modify required files in the repo.
4. Add or update documentation as specified by the task.
5. Build or lint the project to validate changes.
6. Prepare a pull request description summarizing work and verification.
