# Task: Phase 3 - Implement Shared Memory IPC

Status: Pending

Description: Build shared memory IPC starting with a ring buffer or FIFO, optionally extending to flag+payload or RPMsg-lite.

Plan:
- Choose an initial IPC primitive (ring buffer or FIFO) for shared memory messaging.
- Define shared memory layout and control structures for the IPC primitive.
- Implement producer/consumer paths with cache/barrier handling.
- Add basic flow control and error handling for buffer full/empty conditions.
- Create a demo that exchanges messages between the two Zephyr domains.
- Document the IPC design and any platform caveats.

Coding Agent Prompt:
1. Understand the task scope and constraints.
2. Follow the plan above.
3. Create or modify required files in the repo.
4. Add or update documentation as specified by the task.
5. Build or lint the project to validate changes.
6. Prepare a pull request description summarizing work and verification.
