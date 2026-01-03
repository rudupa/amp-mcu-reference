# Task: Phase 3 - Hybrid SMP/AMP Scheduler Model

Status: Pending

Description: Design and prototype a hybrid SMP/AMP scheduling model for Profile C, allowing mixed RTOS and bare-metal domains.

Plan:
- Define scheduling model and invariants for hybrid SMP/AMP domains (which cores participate, allowed preemption).
- Implement runtime hooks to coordinate scheduling decisions with domain lifecycle and IPC.
- Add configuration toggles to enable/disable hybrid scheduling per platform.
- Create demo showing SMP-capable domain plus isolated AMP domain exchanging messages.
- Validate timing/latency impact and document constraints.
- Provide documentation of the model, configuration, and limitations.

Coding Agent Prompt:
1. Understand the task scope and constraints.
2. Follow the plan above.
3. Create or modify required files in the repo.
4. Add or update documentation as specified by the task.
5. Build or lint the project to validate changes.
6. Prepare a pull request description summarizing work and verification.
