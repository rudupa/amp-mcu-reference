# Task: Phase 1 - Prepare Second Image

Status: Pending

Description: Prepare a second-core image (bare-metal loop or second Zephyr instance) to run independently of Core 0.

Plan:
- Choose the second image model: bare-metal loop (simplest) or second Zephyr instance.
- Scaffold the second image project with startup code and minimal main/loop behavior.
- Define startup vector, stack, and entry symbols for the second image.
- Configure toolchain and board settings for the second image build.
- Build the second image artifact and record size/layout.
- Document the chosen approach and any constraints.

Coding Agent Prompt:
1. Understand the task scope and constraints.
2. Follow the plan above.
3. Create or modify required files in the repo.
4. Add or update documentation as specified by the task.
5. Build or lint the project to validate changes.
6. Prepare a pull request description summarizing work and verification.
