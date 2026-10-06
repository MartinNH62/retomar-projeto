# Resume Project (`retomar-projeto`)

[Português (Brasil)](README.pt-BR.md) · [Contributing](CONTRIBUTING.md)

A reusable Codex skill for completing authorized development increments from project instructions, accessible sources, and actual state.

Works across codebases, applications, websites, libraries, and tools, with or without Git or state documentation. It adapts to the project's language, environment, and conventions. The stable identifier `retomar-projeto` means “resume project” in Portuguese.

## What it does

- Reconstructs context and distinguishes current state from historical records.
- Implements, validates, repairs, and records each authorized increment while preserving existing changes.
- Retrieves accessible context directly and continues authorized work without asking the user to relay prompts between chats.
- Reviews a defined target against a confirmed base and reports evidence-backed findings.
- Selects appropriate validation and identifies reused results and limitations.
- Leaves enough context for the next session to continue.

The skill instructions and interface metadata are in English so an international community can review and improve them. You can use the skill in Portuguese or another language; responses follow your language preference. Translation alone is not a demonstrated performance improvement.

## Install

In a local Codex chat, send:

```text
$skill-installer Install the skill from https://github.com/MartinNH62/retomar-projeto/tree/main/skills/retomar-projeto
```

After installation, the skill is available on your next turn. Restart Codex if it does not appear.

Alternatively, download and extract the repository ZIP through GitHub's **Code → Download ZIP** menu. Ask Codex to install the extracted `skills/retomar-projeto` directory into your personal skills directory, preserving an existing installation if there is one. For team use, copy it into `.agents/skills/retomar-projeto` in the team's repository, following your environment's conventions.

## Use

Open your project or specify its directory/repository, then describe the objective:

```text
$retomar-projeto Resume this project and complete the already authorized objective.
```

```text
$retomar-projeto Implement [feature]. Acceptance criteria: [observable outcomes].
```

```text
$retomar-projeto Complete the authorized increments in this plan, validating and recording each before continuing.
```

```text
$retomar-projeto Review this branch against [base] without editing code.
```

Execution requests should produce an implemented and checked result, not just a plan or a prompt to paste into another chat. The agent uses available tools to retrieve context and updates project records directly. It continues to the next increment when that increment is already authorized. Explicit requests for planning or read-only review retain their limited scope.

If a referenced brief is inaccessible, the agent can proceed from the authorized objective and accessible evidence when they sufficiently define the work; otherwise, it requests only the missing decision or access. A blocked check is reported as incomplete validation, not successful delivery. Technical completion does not replace required human gate approval.

Make the project sources and necessary tools available. A skill supplies instructions; it does not grant file/account access, automatically synchronize ChatGPT/Work/Codex, or schedule unattended execution. Authorization follows the user's request and execution environment. See [how skills complement tools](https://developers.openai.com/plugins/concepts/skills).

## Contribute

Reports, focused improvements, examples, and documentation contributions are welcome. Read [CONTRIBUTING.md](CONTRIBUTING.md), [open an issue](https://github.com/MartinNH62/retomar-projeto/issues), or submit a pull request. English is preferred for shared discussions; Portuguese reports are welcome too.

## Structure

```text
README.md
README.pt-BR.md
CONTRIBUTING.md
LICENSE
skills/
  retomar-projeto/
    LICENSE
    SKILL.md
    agents/
      openai.yaml
```

The installable skill contains instructions and interface metadata only, with no executable helper scripts or required service credentials. Repository documentation stays outside the installed skill.

## License

[MIT](LICENSE). Contributions are submitted under the same license.

## Official documentation

- [Build skills](https://learn.chatgpt.com/docs/build-skills)
- [Skills and plugins](https://learn.chatgpt.com/docs/skills-and-plugins)
