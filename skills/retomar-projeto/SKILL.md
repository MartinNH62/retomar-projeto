---
name: retomar-projeto
description: Retomar, executar ou revisar um projeto de desenvolvimento a partir das instruções, fontes e estado real disponíveis. Use para continuar trabalho, implementar um objetivo ou avaliar mudanças em código, aplicativos, sites, bibliotecas e ferramentas, com ou sem Git e documentação de estado. Não usar para perguntas conceituais avulsas sem trabalho no projeto.
---

# Retomar projeto com evidências

Reconstrua o contexto mínimo necessário, conclua o trabalho autorizado e deixe uma continuidade verificável. Adapte o processo à linguagem, ao ambiente e às convenções do projeto; não imponha uma estrutura de documentação ou um sistema de checkpoints.

## Encontrar o contexto atual

- Identifique o repositório, pasta, snapshot ou fonte conectada indicado pelo usuário. Em monorepos ou múltiplos repositórios, delimite os componentes afetados e as instruções que se aplicam a cada um. Não escolha um projeto pelo nome de um chat ou de um diretório temporário.
- Leia as instruções aplicáveis e os documentos relevantes que existirem: README, especificação, decisões, tarefas ou registro de estado. Localize o trecho corrente pela versão, data e relação com o trabalho real; não presuma que a primeira seção é a mais recente. Consulte detalhes conforme forem necessários.
- Confirme o estado das fontes: arquivos pertinentes, alterações existentes e, quando houver Git, branch/HEAD e mudanças rastreadas, staged e não rastreadas. Sem Git, use o inventário relevante disponível; não inicialize um repositório só para retomar.
- Se não houver documentação de estado, reconstrua o contexto pela solicitação, código, configuração, testes e histórico disponível. Diga o que foi inferido. Não crie um conjunto de documentos como condição para começar.
- Relatórios e resumos de chats são pistas, não prova de execução. Se fontes divergem, confira versões e implementação; não confunda o que está implementado com o que deveria estar. Resolva o que as evidências permitem. Pergunte somente se a ambiguidade restante muda materialmente o escopo ou a correção, enquanto avança no trabalho independente.
- Quando houver limitação de acesso, use as fontes acessíveis e identifique sua versão e alcance. Não apresente snapshot como estado atual nem prometa operações que o ambiente não suporta.

## Escolher o modo pela solicitação

**Retomar:** identifique o objetivo, o que já foi feito, pendências e próximo passo. Se o usuário pediu continuidade de execução, prossiga dentro do escopo autorizado; se pediu apenas diagnóstico ou status, entregue essa análise. Não reduza um pedido de ação a um plano por ter iniciado pela retomada.

**Executar:** traduza o objetivo em critérios observáveis de conclusão, usando os critérios existentes quando disponíveis. Implemente, valide e corrija falhas relacionadas até cumprir o objetivo. Decida escolhas rotineiras sem novas aprovações. Uma autorização para o objetivo pode abranger vários passos; uma autorização expressamente limitada a um incremento não abrange os seguintes.

**Revisar:** identifique o alvo e a comparação relevante: mudanças locais, commit, branch, PR ou comportamento. Confirme a base em vez de assumir main ou HEAD; sem Git, delimite os arquivos/comportamentos avaliados. Confronte requisitos, implementação e evidências. Examine regressões, caminhos de erro e integrações pertinentes. Relate cada achado acionável com localização, condição de ocorrência, impacto e evidência; diferencie suspeitas não confirmadas. Não corrija código em revisão somente leitura. Se a correção também estiver autorizada, registre achado, mudança e validação posterior.

Combine modos conforme o pedido, sem exigir chats separados. Uma revisão do próprio implementador não é revisão independente. Ausência de achados não prova correção fora do alcance inspecionado.

## Conduzir o trabalho

- Preserve alterações existentes e artefatos de outros trabalhos, inclusive mudanças staged e arquivos não rastreados. Não restaure, formate em massa ou faça limpeza para obter um estado artificialmente limpo.
- Se outra sessão puder alterar as mesmas fontes, confira sua versão antes de gravar. Releia e integre alterações compatíveis; isole tarefas quando útil e disponível. Interrompa apenas a edição conflitante se não puder preservar ambos os trabalhos, continuando as partes independentes.
- Reutilize o ambiente e os comandos documentados. Quando faltarem, descubra a cadeia de build/teste pela configuração. Instale ou ajuste dependências apenas quando necessário à tarefa e permitido; não faça upgrades gerais como parte incidental de uma retomada.
- Prefira ferramentas que tenham acesso às fontes e aos artefatos originais. Empacote ou copie arquivos quando a transferência for necessária, com identidade da versão; não transforme ZIPs e hashes em obrigação para toda entrega.
- Preserve os limites de autorização da solicitação e do projeto. A skill não concede permissão adicional para publicar, enviar mensagens, migrar dados ou fazer operações Git. Quando essas ações já estiverem autorizadas, não solicite confirmação novamente apenas por usar a skill.

## Validar na medida da mudança

- Escolha verificações que demonstrem os critérios de conclusão e cubram regressões plausíveis. Diferencie inspeção estática, teste unitário, integração e execução no ambiente real; declare quais camadas foram verificadas.
- Reutilize um resultado anterior somente se houver evidência de que o código, dependências, configuração e ambiente relevantes ao comportamento continuam equivalentes. Se isso não puder ser confirmado, rode a verificação pertinente ou marque-a como não verificada. Identifique resultados reutilizados sem tratá-los como execução nova.
- Falha preexistente não é automaticamente causada pela mudança. Compare com uma referência ou evidência anterior quando possível; registre falhas novas, antigas e não classificadas separadamente. Não ajuste um teste para ocultar uma regressão.
- Em correção de defeito, reproduza a condição quando viável e valide o comportamento esperado após a mudança. Acrescente teste de regressão quando útil; não crie testes que apenas espelhem a implementação ou mudanças triviais sem risco relevante.
- Se uma verificação estiver bloqueada, conclua o trabalho que não depende dela e registre a limitação. Não anuncie entrega validada ou aprovação de checkpoint com evidência incompleta. Cumprir critérios técnicos não substitui uma aprovação humana exigida pelo projeto.
- Evite ciclos de tentativas idênticas. Depois de uma falha, altere a hipótese ou obtenha nova evidência antes de repetir. Não encerre um objetivo solucionável só por encontrar a primeira dificuldade.

## Deixar a próxima retomada pronta

Use os registros existentes do projeto. Atualize o estado durante execução quando isso fizer parte do trabalho; mantenha decisões relevantes e pendências com sua condição de resolução. Sem registro existente, deixe um resumo na entrega ou um único arquivo de continuidade quando a duração/complexidade justificar. Não crie documentação redundante.

Registre objetivo e escopo, resultado, arquivos ou componentes afetados, verificações realmente executadas/reutilizadas, limitações e próximo passo, na medida necessária para outra sessão continuar. Não registre credenciais nem dados privados desnecessários.

Em revisão somente leitura, entregue o parecer no chat ou destino autorizado sem alterar o estado técnico. Se houver dependência externa, deixe a preparação útil concluída e identifique a informação ou ação mínima que falta. Na resposta, apresente resultado, validação e limitações materiais, com links acessíveis quando úteis.

## Exemplos de pedidos

- `$retomar-projeto Retome este projeto e conclua o objetivo já autorizado.`
- `$retomar-projeto Implemente esta funcionalidade e valide os critérios de aceitação.`
- `$retomar-projeto Revise as mudanças desta branch contra a base indicada, sem editar código.`
