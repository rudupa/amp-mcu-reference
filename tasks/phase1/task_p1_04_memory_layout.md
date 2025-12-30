# Task: Phase 1 - Hard-Code Memory Layout

Status: Pending

Description: Select flash/RAM addresses for the second image and stacks, link the second image at that address, and ensure no overlap with Zephyr memory.

Plan:
- Choose flash/RAM addresses for the second image, Core 1 stack, and vector table.
- Update linker scripts or linker flags to place the second image at the chosen addresses.
- Ensure the selected regions do not overlap with Zephyr’s memory map; add checks if possible.
- Emit a memory map artifact (map file) and review alignment and size.
- Build both Core 0 and Core 1 images with the fixed layout and validate placement.
- Document the hard-coded layout and rationale.

Coding Agent Prompt:
1. Understand the task scope and constraints.
2. Follow the plan above.
3. Create or modify required files in the repo.
4. Add or update documentation as specified by the task.
5. Build or lint the project to validate changes.
6. Prepare a pull request description summarizing work and verification.
