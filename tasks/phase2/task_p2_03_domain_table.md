# Task: Phase 2 - Move Hard-Coded Addresses into a Domain Table

Status: Pending

Description: Consolidate hard-coded addresses (release, entry, stack, shared memory) into a domain table that mirrors the AMP profile A.

Plan:
- Create a domain table data structure holding release/entry/stack/shmem info for each domain.
- Migrate existing hard-coded constants from Phase 1 into the table.
- Update boot flow to consume the table instead of scattered constants.
- Add validation to ensure no overlapping memory regions between domains.
- Emit logs or diagnostics showing the domain table contents at boot.
- Document how to extend the table for new domains.

Coding Agent Prompt:
1. Understand the task scope and constraints.
2. Follow the plan above.
3. Create or modify required files in the repo.
4. Add or update documentation as specified by the task.
5. Build or lint the project to validate changes.
6. Prepare a pull request description summarizing work and verification.
