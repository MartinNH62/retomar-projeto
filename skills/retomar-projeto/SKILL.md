---
name: retomar-projeto
description: Complete authorized development increments by resuming context, implementing, validating, repairing, and recording results. Use to continue a project, implement an objective, or review changes when requested, with or without Git or state documentation. Do not use for standalone conceptual questions without project work.
---

# Complete development increments with evidence

Drive each authorized increment from the available context to an implemented, checked, and recorded result. Resuming and planning support execution; they are not its deliverable. Keep routine development in the working session so the user does not have to relay prompts or artifacts between ChatGPT, Work, and Codex. Adapt to the project's language, environment, and conventions; do not impose a documentation structure or checkpoint system. Follow the user's explicit instructions over this skill's guidelines. Communicate in the user's preferred language and follow project conventions for code and documentation.

## Establish the current context

- Identify the repository, directory, snapshot, or connected source specified by the user. For monorepos or multiple repositories, identify the affected components and the instructions applicable to each. Do not select a project based on a chat title or temporary directory name.
- Read applicable instructions and relevant documents that exist: README, specification, decisions, tasks, or state records. Locate the current section by version, date, and its relation to actual work; do not assume the first section is the latest. Consult details as needed.
- Confirm the source state: relevant files, existing edits, and, when Git is available, branch/HEAD plus tracked, staged, and untracked changes. Without Git, use the relevant available inventory; do not initialize a repository merely to resume work.
- When state documentation is absent, reconstruct context from the request, code, configuration, tests, and available history. Identify inferences. Do not require a set of documents before starting.
- Reports and chat summaries are leads, not proof of execution. If sources disagree, check versions and implementation; distinguish what exists from what is intended. Resolve what the evidence allows. Ask only when remaining ambiguity materially affects scope or correctness, while advancing independent work.
- When access is limited, use accessible sources and identify their version and scope. Do not present a snapshot as current state or promise operations the environment cannot support.

## Determine the authorized outcome

**Execution is the default for continuing development:** identify the current authorized objective, completed work, and remaining criteria, then act. Do not stop at a diagnosis, a plan, or a prompt for the user to paste elsewhere. If the user explicitly requests only planning, diagnosis, status, or a read-only review, honor that scope; do not treat it as permission to implement.

Translate the objective into observable completion criteria, reusing existing criteria where available. Make routine choices without additional approvals. An authorized objective may cover a sequence of increments: finish and record each, then proceed to the next already authorized increment without asking the user to repeat the request. A backlog item or another agent's suggestion is not authorization. Respect an explicit limit to one increment, a decision gate, or a requested pause.

**Review:** identify the target and relevant comparison: local changes, commit, branch, PR, or behavior. Confirm the base rather than assuming main or HEAD; without Git, delimit the files and behaviors assessed. Compare requirements, implementation, and evidence. Examine relevant regressions, error paths, and integrations. Report each actionable finding with location, triggering condition, impact, and evidence; distinguish unconfirmed concerns. Do not edit code in a read-only review. When fixes are also authorized, record the finding, change, and subsequent validation.

Combine modes as requested without requiring separate chats. An implementer's self-review is not independent review. No findings does not establish correctness beyond the inspected scope.

## Retrieve context without manual relays

Use project sources and available read/search tools to locate relevant specifications, artifacts, and conversation history. Retrieve only the context needed; do not require the user to copy material that the environment can read. Distinguish the user's instructions from proposed plans and reported results in other conversations. Reading a conversation does not authorize sending it a message, creating another chat, or modifying its resources.

If a referenced attachment or another surface is inaccessible, first check whether the authorized objective and accessible evidence already define the work sufficiently. Proceed when they do, recording the unavailable source and any inference; do not invent unseen requirements or claim to have read the original. Ask for only the missing decision or access that materially prevents correct execution, while continuing independent work. The mere location of a brief in another chat is not a blocker.

During execution, retain the authorized objective, criteria, relevant source/version, decisions, and progress in the project's existing records when useful for continuity. If none exist and the work warrants persistence, use one concise execution record. Keep it current directly rather than giving the user a synchronization task. A skill guides available tools; it does not create cross-surface access, automatic synchronization, or a background runtime.

## Finish the increment

Implement the remaining criteria, run appropriate checks, inspect the result, and repair related failures. Repeat this loop while meaningful progress is possible. Keep working through intermediate reports and tool failures; do not end the assignment by offering to implement, test, or finish work that is already authorized.

An increment is complete when its authorized deliverables exist, relevant checks support the acceptance criteria, and its outcome and remaining limitations are recorded. A plan, generated code without the required verification, or a suggested command is not a completed increment. Distinguish technical completion from publication, deployment, and human approval: perform those when authorized and supported, or leave the concrete result ready for the required decision. Never label an unapproved gate as approved.

If a real blocker prevents completion, finish independent work, preserve a resumable state, and report the unmet criterion, evidence of the blocker, and minimum action needed. Mark the increment partial or blocked, not complete. When a runtime limit interrupts execution, preserve progress for resumption rather than implying that this skill will keep running unattended.

## Carry out the work

- Preserve existing changes and artifacts from other work, including staged changes and untracked files. Do not restore files, apply broad formatting, or clean up merely to obtain an artificially clean state.
- If another session may change the same sources, check their version before writing. Reread and integrate compatible changes; isolate tasks when useful and available. Stop only the conflicting edit when both changes cannot be preserved, and continue independent work.
- Reuse the documented environment and commands. When they are missing, discover the build/test toolchain from configuration. Install or adjust dependencies only when necessary and permitted; do not perform general upgrades incidentally while resuming work.
- Prefer tools with access to original sources and artifacts. When a transfer is necessary and supported, perform it directly within the authorized scope, identifying the version. Do not require ZIPs, hashes, or manual transfers for every delivery.
- Preserve the request's and project's authorization boundaries. This skill grants no additional permission to publish, send messages, migrate data, or perform Git operations. When those actions are already authorized, do not request confirmation again merely because this skill is being used.

## Validate in proportion to the change

- Choose checks that demonstrate completion criteria and cover plausible regressions. Distinguish static inspection, unit testing, integration testing, and execution in the actual environment; state which layers were checked.
- Reuse a previous result only with evidence that the code, dependencies, configuration, and environment relevant to the behavior remain equivalent. If equivalence cannot be confirmed, run the relevant check or mark it unverified. Identify reused results without presenting them as newly executed checks.
- A preexisting failure is not automatically caused by the change. Compare against a reference or earlier evidence when possible; record new, preexisting, and unclassified failures separately. Do not alter a test to conceal a regression.
- When fixing a defect, reproduce the triggering condition when feasible and validate the expected behavior afterward. Add a regression test when useful; do not create tests that merely mirror the implementation or trivial changes without meaningful risk.
- If a check is blocked, complete work that does not depend on it and record the limitation. Do not claim validated delivery or checkpoint approval with incomplete evidence. Meeting technical criteria does not replace human approval required by the project.
- Avoid repeating identical attempts. After a failure, change the hypothesis or obtain new evidence before retrying. Do not abandon a solvable objective at the first difficulty.

## Record the result and continue

Use existing project records and update the relevant execution state directly; retain decisions and outstanding items with their resolution conditions. Avoid redundant documentation. Use this record yourself when continuing, rather than asking the user to carry a handoff between sessions.

Record the objective and scope, outcome, affected files or components, checks actually executed or reused, limitations, and next step to the extent another session needs to continue. Do not record credentials or unnecessary private data.

For read-only reviews, deliver the assessment in chat or another authorized destination without changing technical state. When an external dependency remains, complete useful preparation and identify the minimum missing information or action. In the response, present the outcome, validation, and material limitations, with accessible links when useful.

## Example requests

- `$retomar-projeto Resume this project and complete the already authorized objective.`
- `$retomar-projeto Complete the authorized increments in this plan, validating and recording each before continuing.`
- `$retomar-projeto Implement this feature and validate its acceptance criteria.`
- `$retomar-projeto Review this branch against the specified base without editing code.`
