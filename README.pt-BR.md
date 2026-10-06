# Retomar Projeto (`retomar-projeto`)

[English](README.md) · [Como contribuir (em inglês)](CONTRIBUTING.md)

Skill reutilizável para concluir incrementos de desenvolvimento autorizados pelas instruções do projeto, fontes acessíveis e estado real.

Aplica-se a código, aplicativos, sites, bibliotecas e ferramentas, com ou sem Git e documentação de estado. Adapta o fluxo à linguagem, ao ambiente e às convenções do projeto.

## O que ela faz

- Reconstrói o contexto e distingue estado atual de registros históricos.
- Implementa, valida, corrige e registra cada incremento autorizado, preservando alterações existentes.
- Busca o contexto acessível diretamente e continua o trabalho autorizado sem pedir que você transporte prompts entre chats.
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
$retomar-projeto Conclua os incrementos autorizados deste plano, validando e registrando cada um antes de continuar.
```

```text
$retomar-projeto Revise esta branch contra [base], sem editar código.
```

Pedidos de execução devem produzir um resultado implementado e verificado, sem encerrar apenas com um plano ou um prompt para colar em outro chat. O agente busca contexto pelas ferramentas disponíveis e atualiza os registros do projeto diretamente. Avança ao próximo incremento quando ele já estiver autorizado. Pedidos explícitos de planejamento ou revisão sem alterações mantêm esse escopo.

Se um roteiro estiver inacessível, o agente pode trabalhar a partir do objetivo autorizado e das evidências disponíveis quando forem suficientes; caso contrário, solicita apenas a decisão ou o acesso que falta. Uma verificação bloqueada é registrada como validação incompleta. A conclusão técnica não substitui uma aprovação humana exigida pelo projeto.

Disponibilize as fontes do projeto e as ferramentas necessárias. A skill oferece instruções; não concede acesso a arquivos ou contas, não sincroniza automaticamente ChatGPT/Work/Codex nem agenda execução sem supervisão. A autorização segue a solicitação e o ambiente de execução. Veja [como skills complementam ferramentas](https://developers.openai.com/plugins/concepts/skills).

## Contribuir

Relatos de falhas, melhorias pontuais, exemplos e documentação são bem-vindos. Leia [CONTRIBUTING.md](CONTRIBUTING.md), [abra uma issue](https://github.com/MartinNH62/retomar-projeto/issues) ou envie um pull request. Inglês é preferido nas discussões compartilhadas; relatos em português também são aceitos.

A versão canônica da skill é `skills/retomar-projeto/SKILL.md`, em inglês. Este guia documenta seu uso em português, sem criar uma segunda skill para manter.

## Licença

[MIT](LICENSE). As contribuições são enviadas sob a mesma licença.

## Documentação oficial

- [Criar e instalar skills](https://learn.chatgpt.com/docs/build-skills)
- [Skills e plugins](https://learn.chatgpt.com/docs/skills-and-plugins)
