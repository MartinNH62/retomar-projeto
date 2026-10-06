---
name: retomar-projeto
description: Resume, execute, or review development work using the available project instructions, sources, and actual state. Use to continue a project, implement an objective, or assess changes, with or without Git or state documentation. Do not use for standalone conceptual questions without project work.
---

# Resume development work with evidence

Reconstruct the minimum context needed, complete the authorized work, and leave a verifiable handoff. Adapt to the project's language, environment, and conventions; do not impose a documentation structure or checkpoint system. Follow the user's explicit instructions over this skill's guidelines. Communicate in the user's preferred language; English instructions do not require English responses. Follow project conventions for code and documentation.

## Establish the current context

- Identify the repository, directory, snapshot, or connected source specified by the user. For monorepos or multiple repositories, identify the affected components and the instructions applicable to each. Do not select a project based on a chat title or temporary directory name.
- Read applicable instructions and relevant documents that exist: README, specification, decisions, tasks, or state records. Locate the current section by version, date, and its relation to actual work; do not assume the first section is the latest. Consult details as needed.
- Confirm the source state: relevant files, existing edits, and, when Git is available, branch/HEAD plus tracked, staged, and untracked changes. Without Git, use the relevant available inventory; do not initialize a repository merely to resume work.
- When state documentation is absent, reconstruct context from the request, code, configuration, tests, and available history. Identify inferences. Do not require a set of documents before starting.
- Reports and chat summaries are leads, not proof of execution. If sources disagree, check versions and implementation; distinguish what exists from what is intended. Resolve what the evidence allows. Ask only when remaining ambiguity materially affects scope or correctness, while advancing independent work.
- When access is limited, use accessible sources and identify their version and scope. Do not present a snapshot as current state or promise operations the environment cannot support.

## Select modes from the request

**Resume:** identify the objective, completed work, outstanding items, and next step. If the user requests continued execution, proceed within the authorized scope; if they request diagnosis or status only, provide that analysis. Do not reduce an action request to a plan because it began with resuming work.

**Execute:** translate the objective into observable completion criteria, reusing existing criteria where available. Implement, validate, and fix related failures until the objective is met. Make routine choices without additional approvals. Authorization for an objective may cover multiple steps; authorization expressly limited to one increment does not cover subsequent increments.

**Review:** identify the target and relevant comparison: local changes, commit, branch, PR, or behavior. Confirm the base rather than assuming main or HEAD; without Git, delimit the files and behaviors assessed. Compare requirements, implementation, and evidence. Examine relevant regressions, error paths, and integrations. Report each actionable finding with location, triggering condition, impact, and evidence; distinguish unconfirmed concerns. Do not edit code in a read-only review. When fixes are also authorized, record the finding, change, and subsequent validation.

Combine modes as requested without requiring separate chats. An implementer's self-review is not independent review. No findings does not establish correctness beyond the inspected scope.

## Carry out the work

- Preserve existing changes and artifacts from other work, including staged changes and untracked files. Do not restore files, apply broad formatting, or clean up merely to obtain an artificially clean state.
- If another session may change the same sources, check their version before writing. Reread and integrate compatible changes; isolate tasks when useful and available. Stop only the conflicting edit when both changes cannot be preserved, and continue independent work.
- Reuse the documented environment and commands. When they are missing, discover the build/test toolchain from configuration. Install or adjust dependencies only when necessary and permitted; do not perform general upgrades incidentally while resuming work.
- Prefer tools with access to original sources and artifacts. Package or copy files when transfer is necessary, identifying the version; do not require ZIPs or hashes for every delivery.
- Preserve the request's and project's authorization boundaries. This skill grants no additional permission to publish, send messages, migrate data, or perform Git operations. When those actions are already authorized, do not request confirmation again merely because this skill is being used.

## Validate in proportion to the change

- Choose checks that demonstrate completion criteria and cover plausible regressions. Distinguish static inspection, unit testing, integration testing, and execution in the actual environment; state which layers were checked.
- Reuse a previous result only with evidence that the code, dependencies, configuration, and environment relevant to the behavior remain equivalent. If equivalence cannot be confirmed, run the relevant check or mark it unverified. Identify reused results without presenting them as newly executed checks.
- A preexisting failure is not automatically caused by the change. Compare against a reference or earlier evidence when possible; record new, preexisting, and unclassified failures separately. Do not alter a test to conceal a regression.
- When fixing a defect, reproduce the triggering condition when feasible and validate the expected behavior afterward. Add a regression test when useful; do not create tests that merely mirror the implementation or trivial changes without meaningful risk.
- If a check is blocked, complete work that does not depend on it and record the limitation. Do not claim validated delivery or checkpoint approval with incomplete evidence. Meeting technical criteria does not replace human approval required by the project.
- Avoid repeating identical attempts. After a failure, change the hypothesis or obtain new evidence before retrying. Do not abandon a solvable objective at the first difficulty.

## Prepare the next handoff

Use existing project records. Update state during execution when it is part of the work; retain relevant decisions and outstanding items with their resolution conditions. Without existing records, provide a delivery summary or a single handoff file when duration or complexity justifies it. Avoid redundant documentation.

Record the objective and scope, outcome, affected files or components, checks actually executed or reused, limitations, and next step to the extent another session needs to continue. Do not record credentials or unnecessary private data.

For read-only reviews, deliver the assessment in chat or another authorized destination without changing technical state. When an external dependency remains, complete useful preparation and identify the minimum missing information or action. In the response, present the outcome, validation, and material limitations, with accessible links when useful.

## Example requests

- `$retomar-projeto Resume this project and complete the already authorized objective.`
- `$retomar-projeto Implement this feature and validate its acceptance criteria.`
- `$retomar-projeto Review this branch against the specified base without editing code.`
