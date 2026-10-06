# Retomar Projeto

Skill para retomar, executar e revisar projetos de desenvolvimento com base nas instruções, fontes e estado real disponíveis.

Aplica-se a código, aplicativos, sites, bibliotecas e ferramentas, com ou sem Git e documentação de estado. Adapta o fluxo à linguagem, ao ambiente e às convenções do projeto.

## O que ela faz

- Reconstrói o contexto pelas fontes acessíveis e distingue estado atual de registros históricos.
- Conduz o objetivo autorizado até uma entrega verificável, preservando alterações existentes.
- Revisa mudanças com alvo e base definidos, relatando achados com evidências.
- Escolhe validações proporcionais à mudança e identifica resultados reutilizados e limitações.
- Deixa informações suficientes para uma próxima sessão continuar.

## Instalar pelo GitHub

Abra um chat no Codex e envie:

```text
$skill-installer Instale a skill de https://github.com/MartinNH62/retomar-projeto/tree/main/skills/retomar-projeto
```

O instalador integrado aceita skills em repositórios públicos do GitHub. Depois da instalação, a skill fica disponível no próximo turno. Se não aparecer, reinicie o Codex.

## Instalar a partir do pacote ZIP

Extraia o ZIP. A pasta que precisa ser instalada é `skills/retomar-projeto`, contendo `SKILL.md` e `agents/openai.yaml`.

Abra um chat local no Codex, indique o caminho da pasta extraída e solicite:

```text
Instale a skill retomar-projeto desta pasta na minha pasta pessoal de skills do Codex, preservando os arquivos e avisando se já existir uma versão instalada.
```

Para compartilhar com uma equipe dentro de um projeto, copie essa pasta para `.agents/skills/retomar-projeto` no repositório da equipe, seguindo as convenções do ambiente.

## Usar

Abra o projeto ou informe sua pasta/repositório e descreva o objetivo:

```text
$retomar-projeto Retome este projeto e conclua o objetivo já autorizado.
```

```text
$retomar-projeto Implemente esta funcionalidade: [descrição]. Critérios de aceitação: [resultados esperados].
```

```text
$retomar-projeto Revise as mudanças desta branch contra [base], sem editar código.
```

Informe os caminhos ou fontes necessários e mantenha disponíveis as ferramentas do projeto. A skill fornece instruções reutilizáveis; não fornece acesso a arquivos, contas ou ambientes de outra pessoa. Permissões e aprovações continuam seguindo a solicitação e o ambiente de quem a usa.

## Conteúdo

```text
README.md
skills/
  retomar-projeto/
    SKILL.md
    agents/
      openai.yaml
```

A skill contém apenas instruções e metadados de interface. Não executa um script próprio de instalação e não depende de credenciais ou serviços específicos.

## Documentação

- [Skills e instalação no Codex](https://learn.chatgpt.com/docs/build-skills)
- [Skills e plugins](https://learn.chatgpt.com/docs/skills-and-plugins)
