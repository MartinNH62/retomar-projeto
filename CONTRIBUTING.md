# Contributing

Contributions are welcome: report a failure, improve an instruction, clarify an example, or improve the documentation. English is the preferred shared language for issues and pull requests; Portuguese reports are also welcome.

## Scope

This skill supports resuming, executing, and reviewing development work across projects, languages, and environments. Keep it independent of a particular repository, vendor, framework, or documentation system.

The canonical skill instructions are in English at `skills/retomar-projeto/SKILL.md`. `README.pt-BR.md` documents usage in Portuguese; it is not a separate executable skill. Keep the identifier `retomar-projeto` and its installation path stable unless a compatibility change is explicitly agreed.

## Report a problem

[Open an issue](https://github.com/MartinNH62/retomar-projeto/issues) with:

- The task, environment, and model/version if known.
- Expected and observed behavior.
- The smallest reproducible example and relevant evidence.
- Whether the problem comes from the skill, unavailable tools, project instructions, or an unknown cause.

Remove credentials and private project data. A synthetic example is preferable when the original cannot be shared. Do not post sensitive vulnerability details publicly; report the general issue without disclosure and agree on a suitable private channel first.

## Propose a change

1. Fork the repository and create a branch.
2. Make a focused change addressing a demonstrated problem or clear use case.
3. Keep the English README and Portuguese usage guide consistent when installation or usage changes. Update `agents/openai.yaml` if the interface changes; preserve its invocation policy.
4. Open a pull request explaining the problem, resulting behavior, validation, and remaining limitations. Link a related issue when there is one.

Preserve authorization boundaries, existing edits, read-only review behavior, and the distinction between observed and inferred state. Do not introduce required accounts, tools, checkpoints, or documents without a concrete need. Prefer narrow improvements over accumulating rules for hypothetical failures.

## Validate the change

Check valid YAML frontmatter, matching directory/name (`retomar-projeto`), readable Markdown, working relative links, and consistent interface metadata. The Codex skill-creator validator can check structure when available; passing it does not prove behavior.

For changes that affect decisions, try relevant scenarios in an isolated disposable project, for example:

- Resume without Git or state documentation.
- Implement a small objective while preserving existing staged/untracked edits.
- Review against an explicitly specified base without editing files.
- Encounter a blocked check, stale test result, or conflicting edit and accurately report the limitation.

Record the setup, checks, observed outcome, and limitations. Do not require live accounts, paid API calls, or access to someone else's project to contribute. If claiming that a translation improves performance, compare equivalent tasks with the same model/settings and multiple runs; distinguish readability improvements from measured execution improvements.

## License

By submitting a contribution, you agree to license it under the repository's [MIT license](LICENSE). Do not submit material you lack permission to share.
