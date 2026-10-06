# Retomar Projeto (`retomar-projeto`)

[English](README.md) · [Como contribuir (em inglês)](CONTRIBUTING.md)

Skill reutilizável para retomar, executar e revisar projetos de desenvolvimento pelas instruções do projeto, fontes acessíveis e estado real.

Aplica-se a código, aplicativos, sites, bibliotecas e ferramentas, com ou sem Git e documentação de estado. Adapta o fluxo à linguagem, ao ambiente e às convenções do projeto.

## O que ela faz

- Reconstrói o contexto e distingue estado atual de registros históricos.
- Conclui o trabalho autorizado, preservando alterações existentes.
- Revisa um alvo definido contra uma base confirmada e relata achados com evidências.
- Escolhe validações pertinentes e identifica resultados reutilizados e limitações.
- Deixa contexto suficiente para a próxima sessão continuar.

As instruções da skill e os metadados de interface estão em inglês para facilitar contribuições internacionais. Você pode continuar usando a skill em português: as respostas seguem sua preferência de idioma. A tradução, por si só, não demonstra ganho de desempenho.

## Instalar

Em um chat local do Codex, envie:

```text
$skill-installer Instale a skill de https://github.com/MartinNH62/retomar-projeto/tree/main/skills/retomar-projeto
```

Depois da instalação, a skill fica disponível no próximo turno. Se não aparecer, reinicie o Codex.

Como alternativa, baixe e extraia o ZIP do repositório pelo menu **Code → Download ZIP** do GitHub. Peça ao Codex para instalar a pasta extraída `skills/retomar-projeto` na sua pasta pessoal de skills, preservando uma instalação existente. Para equipes, copie-a para `.agents/skills/retomar-projeto` no repositório da equipe, seguindo as convenções do ambiente.

## Usar

Abra o projeto ou informe sua pasta/repositório e descreva o objetivo:

```text
$retomar-projeto Retome este projeto e conclua o objetivo já autorizado.
```

```text
$retomar-projeto Implemente [funcionalidade]. Critérios de aceitação: [resultados observáveis].
```

```text
$retomar-projeto Revise esta branch contra [base], sem editar código.
```

Forneça as fontes e ferramentas pertinentes. A skill oferece instruções reutilizáveis; não concede acesso a arquivos, contas ou ambientes de outra pessoa. A autorização segue a solicitação e o ambiente de execução.

## Contribuir

Relatos de falhas, melhorias pontuais, exemplos e documentação são bem-vindos. Leia [CONTRIBUTING.md](CONTRIBUTING.md), [abra uma issue](https://github.com/MartinNH62/retomar-projeto/issues) ou envie um pull request. Inglês é preferido nas discussões compartilhadas; relatos em português também são aceitos.

A versão canônica da skill é `skills/retomar-projeto/SKILL.md`, em inglês. Este guia documenta seu uso em português, sem criar uma segunda skill para manter.

## Licença

[MIT](LICENSE). As contribuições são enviadas sob a mesma licença.

## Documentação oficial

- [Criar e instalar skills](https://learn.chatgpt.com/docs/build-skills)
- [Skills e plugins](https://learn.chatgpt.com/docs/skills-and-plugins)
