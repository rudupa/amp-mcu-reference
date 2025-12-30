# Task: Phase 4 - Add Domain Manifest

Status: Pending

Description: Add a domain manifest capturing version, hash/signature, memory map, and IPC channels for each domain.

Plan:
- Define manifest fields (version, hash/signature, memory map, IPC channels, optional metadata).
- Implement manifest generation from domain definitions and build artifacts.
- Integrate manifest consumption into boot to verify integrity and compatibility.
- Add tooling/tests to validate manifest integrity and hashes.
- Emit manifest data for existing profiles (RP2350 profile A/B/C).
- Document manifest format and verification flow.

Coding Agent Prompt:
1. Understand the task scope and constraints.
2. Follow the plan above.
3. Create or modify required files in the repo.
4. Add or update documentation as specified by the task.
5. Build or lint the project to validate changes.
6. Prepare a pull request description summarizing work and verification.
