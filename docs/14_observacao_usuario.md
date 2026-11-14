# Entrega 14 — Avaliação de usabilidade por observação de usuários

**Data:** 14/11/2026  
**Status:** 🟨 em andamento  
**Responsabilidade:** solução consolidada por equipe. O número de participantes finais observados deve ser igual ao número de integrantes, conforme o modelo da disciplina; recomenda-se que cada integrante seja responsável por conduzir/analisar ao menos um participante.

## Objetivo da atividade

Observar usuários representativos realizando tarefas reais ou realisticamente simuladas para identificar problemas de eficácia, eficiência, compreensão e satisfação que não podem ser inferidos apenas por inspeção.

> **Participantes finais não devem ser membros da equipe.** Um integrante pode participar do teste piloto apenas para validar roteiro/equipamentos, sem contar na amostra final.

### Quando o usuário é um perfil profissional especializado

Em TCCs técnicos, o público pode ser DBA, analista, pesquisador, administrador, técnico ou outro especialista. Priorize participantes que possuam relação real com as tarefas. Se não for possível recrutar o perfil ideal, qualquer participante aproximado/proxy deve ser **justificado previamente e tratado como limitação**; não apresente o resultado como equivalente ao de especialistas reais.

O teste avalia a **interação com o protótipo**. Não é necessário que o participante valide o desempenho científico do algoritmo. Resultados simulados podem ser usados quando declarados e coerentes com a tarefa.

Tarefas podem envolver, por exemplo, interpretar um dashboard, configurar uma análise, encontrar uma execução no histórico usando filtros, comparar resultados, gerar relatório, revisar alerta ou administrar permissões.

## A. Fluxograma do processo — equipe

![Fluxograma](../assets/14_testes/fluxograma_avaliacao.png)

O fluxograma deve representar, no mínimo: planejamento → recrutamento → consentimento → preparação → execução das tarefas/observação → pós-teste → consolidação/análise → recomendações.

## B. Procedimento de preparação e execução — equipe

### Passo 1 — Objetivos e versão avaliada

**Versão/commit/Figma:** [Assistente Virtual Acadêmico da FEI](https://www.figma.com/design/H0YnqyGWkswU88IUZIgDuW)

**Metas de usabilidade relacionadas:**

- MU01 — Compreensão: verificar se os estudantes compreenderam as funcionalidades da interface, as respostas apresentadas e as fontes institucionais.
- MU02 — Eficácia: avaliar se os participantes conseguiram concluir as tarefas propostas.
- MU03 — Eficiência: analisar o tempo necessário para realizar as tarefas e a quantidade de erros e pedidos de ajuda.
- MU04 — Satisfação: verificar a percepção dos participantes em relação à facilidade de utilização do protótipo.
- MU05 — Erros e recuperação: avaliar se os participantes conseguiram compreender mensagens de erro e identificar alternativas para continuar suas consultas.

### Passo 2 — Participantes

| ID | Perfil | Critérios que justificam participação | Integrante responsável |
|---|---|---|---|
| U01 | Estudante universitário, familiarizado com plataformas acadêmicas e ferramentas de inteligência artificial. | O participante foi selecionado por apresentar características compatíveis com o público-alvo do Assistente Virtual Acadêmico da FEI. Sua familiaridade com sistemas acadêmicos e ferramentas digitais permitiu avaliar a facilidade de utilização, a compreensão das respostas e a navegação pelo protótipo. | Matheus Dourado Valle — 22.224.023-6 |
| U02 | Estudante universitário. | Participante previsto para avaliação da interação com o protótipo. Perfil e critérios específicos a serem confirmados. | João Pedro Sabino Garcia — 22.224.032-7 |

### Passo 3 — Consentimento e privacidade

- Termo/registro de consentimento: os participantes U01 e U02 autorizaram sua participação e a utilização dos resultados para fins acadêmicos. O consentimento foi registrado por meio de mensagens privadas e os comprovantes foram mantidos pela equipe, sem publicação no repositório.
- Gravação de tela/áudio/vídeo: não foi realizada gravação. Os resultados foram documentados por meio de registros das tarefas, dificuldades, tempos, erros, ajudas e respostas pós-teste.
- Forma de anonimização: os participantes foram identificados pelos códigos `U01` e `U02`, preservando suas identidades nas tabelas de avaliação.
- Local e período de armazenamento: os registros foram mantidos em ambiente privado da equipe, com acesso restrito aos integrantes, durante o período necessário à conclusão da avaliação acadêmica.

### Passo 4 — Teste piloto

**Data:** 14/11/2026

**Participante piloto:** Matheus Dourado Valle — 22.224.023-6.

**Moderador:** João Pedro Sabino Garcia — 22.224.032-7.

**Objetivo:** Verificar a clareza das instruções, o funcionamento do protótipo no Figma, a adequação das tarefas propostas e o procedimento de registro das observações antes da avaliação com os participantes finais.

**O que foi validado:** O teste piloto permitiu verificar os seguintes aspectos:

- Clareza das instruções das tarefas UT01, UT02, UT03 e UT04.
- Disponibilidade das telas necessárias no protótipo.
- Funcionamento dos elementos de navegação.
- Adequação da sequência das tarefas.
- Tempo necessário para realizar as atividades.
- Possibilidade de registrar tempos, erros e pedidos de ajuda.
- Clareza das perguntas utilizadas no pós-teste.

**Resultados do teste piloto:**

| Tarefa | Resultado | Tempo | Dificuldades identificadas | Ajustes realizados |
|---|---|---|---|---|
| UT01 — Rematrícula | Concluída | 00:55 | Não foram identificadas dificuldades relevantes. | A instrução original foi mantida. |
| UT02 — Documentos acadêmicos | Concluída | 01:20 | Foi identificada a necessidade de deixar mais claro que o participante deveria verificar a origem da informação. | A instrução foi ajustada para solicitar a identificação da fonte institucional, sem indicar onde encontrá-la. |
| UT03 — Histórico | Concluída | 00:40 | Não foram identificadas dificuldades relevantes. | A instrução original foi mantida. |
| UT04 — Resposta inconclusiva | Concluída | 01:30 | Foi identificada a necessidade de esclarecer que o participante deveria tentar continuar a consulta. | O cenário foi ajustado para solicitar uma alternativa de continuidade, sem ensinar o caminho. |

**Mudanças após piloto:**

1. Na UT02, a instrução foi ajustada para deixar explícita a necessidade de verificar a origem da informação apresentada.
2. Na UT04, o enunciado foi ajustado para esclarecer que o participante deveria identificar uma alternativa para continuar a consulta.
3. A ordem das quatro tarefas foi mantida, pois não foram identificados problemas relacionados à sequência.
4. Foi mantida a escala de satisfação de 1 a 5 para todas as tarefas.
5. O registro de erros e pedidos de ajuda foi organizado separadamente, facilitando a análise posterior.

O teste piloto permitiu verificar o funcionamento do procedimento de avaliação e identificar pequenos ajustes necessários nas instruções.

As alterações realizadas tiveram como objetivo melhorar a clareza dos cenários apresentados, sem fornecer orientações sobre os caminhos que deveriam ser utilizados pelos participantes.

Após os ajustes, o roteiro foi considerado adequado para a aplicação com os participantes finais U01 e U02.

O participante utilizado no teste piloto não foi contabilizado na amostra final da avaliação.

### Passo 5 — Tarefas

| ID | Cenário/instrução apresentada | Critério de sucesso | Métricas | Ligação com modelo |
|---|---|---|---|---|
| UT01 | "Você precisa descobrir como funciona o processo de rematrícula na FEI. Utilize o assistente virtual para encontrar essa informação." | Realizar a consulta e compreender as informações apresentadas pelo assistente. | Sucesso, tempo, erros, ajudas e satisfação. | T01 / M01 — Consulta de informações acadêmicas. |
| UT02 | "Você precisa descobrir como solicitar uma declaração de matrícula. Utilize o assistente para encontrar essa informação e verificar sua origem." | Consultar a informação e identificar a fonte institucional apresentada na resposta. | Sucesso, tempo, erros, ajudas e satisfação. | T01 / M01 — Consulta e compreensão de informações acadêmicas. |
| UT03 | "Imagine que você realizou uma consulta anteriormente e deseja acessar novamente aquela conversa. Encontre uma conversa anterior." | Localizar e acessar uma conversa disponível no histórico. | Sucesso, tempo, erros, ajudas e satisfação. | M01 — Recuperação de informações e histórico de conversas. |
| UT04 | "Você realizou uma pergunta, mas o assistente informou que não encontrou informações suficientes. Identifique o que aconteceu e tente descobrir como continuar sua consulta." | Compreender a ausência de informações e identificar uma alternativa para continuar a consulta. | Sucesso, tempo, erros, ajudas e satisfação. | M01 — Tratamento de respostas inconclusivas e recuperação de erros. |

### Passo 6 — Protocolo do moderador

1. Receber participante e explicar que **o produto está sendo avaliado, não a pessoa**.
2. Obter consentimento.
3. Aplicar perfil pré-teste mínimo necessário.
4. Ler instruções padronizadas.
5. Observar sem ensinar o caminho; registrar pedidos de ajuda separadamente.
6. Se usar *think aloud*, explicar e aplicar de forma consistente.
7. Após cada tarefa, registrar satisfação/SEQ ou escala definida.
8. Fazer pós-teste/entrevista breve.
9. Encerrar e explicar uso dos dados.

## C. Resultados — por participante

### U01 — Estudante universitário

**Integrante responsável:** Matheus Dourado Valle — 22.224.023-6  
**Protótipo avaliado:** Assistente Virtual Acadêmico da FEI — Figma.  
**Data:** 14/11/2026  
**Escala de satisfação:** 1 (muito insatisfeito) a 5 (muito satisfeito).

| Tarefa | Grau de sucesso | Erros | Tipos de erro/dificuldade | Ajudas | Tempo | Satisfação | Evidência/observação |
|---|---|---:|---|---:|---|---|---|
| UT01 | Total | 0 | Não apresentou dificuldades relevantes. | 0 | 01:12 | 5/5 | O participante identificou rapidamente o campo de mensagens, realizou uma consulta sobre rematrícula e compreendeu a resposta apresentada. |
| UT02 | Total | 1 | Apresentou dificuldade inicial para identificar as fontes institucionais utilizadas na resposta. | 0 | 01:45 | 4/5 | O participante consultou informações sobre documentos acadêmicos, mas demorou para localizar a referência institucional apresentada. Após examinar a resposta, conseguiu identificar a fonte. |
| UT03 | Total | 0 | Não apresentou dificuldades relevantes. | 0 | 00:48 | 5/5 | O participante identificou o histórico na barra lateral e localizou uma conversa anterior sem solicitar auxílio. |
| UT04 | Parcial | 1 | Apresentou dificuldade para identificar como continuar a consulta após uma resposta sem informações suficientes. | 1 | 02:10 | 3/5 | O participante compreendeu que o assistente não possuía informações suficientes, mas necessitou de uma orientação para identificar como continuar a consulta. |

**Link da gravação (se autorizado):** Não disponível.

**Resposta pós-teste:**

O participante considerou a interface simples, organizada e fácil de utilizar. Destacou que a semelhança com outras ferramentas de inteligência artificial facilitou a compreensão das funcionalidades e permitiu que ele utilizasse o sistema sem dificuldades iniciais.

Em relação às consultas acadêmicas, relatou que conseguiu formular perguntas e compreender as informações apresentadas pelo assistente. Também considerou o histórico de conversas fácil de localizar e utilizar.

Entretanto, apontou que as fontes institucionais poderiam apresentar maior destaque visual, pois demorou um pouco para identificar de onde as informações haviam sido obtidas.

Outra dificuldade mencionada esteve relacionada às situações em que o assistente não conseguiu apresentar uma resposta conclusiva. O participante compreendeu que não havia informações suficientes, mas considerou que a interface poderia oferecer orientações mais claras sobre como continuar.

Como sugestões de melhoria, destacou a necessidade de tornar as fontes mais visíveis e apresentar alternativas de perguntas ou orientações quando o assistente não conseguir responder.

De maneira geral, avaliou positivamente o protótipo e considerou que a ferramenta poderia facilitar a consulta de informações acadêmicas e administrativas da FEI.

### U02 — Estudante universitário

**Integrante responsável:** João Pedro Sabino Garcia — 22.224.032-7

| Tarefa | Grau de sucesso | Erros | Tipos de erro/dificuldade | Ajudas | Tempo | Satisfação | Evidência/observação |
|---|---|---:|---|---:|---|---|---|
| UT01 | {{...}} | {{...}} | {{...}} | {{...}} | {{mm:ss}} | {{1–5}} | {{...}} |
| UT02 | {{...}} | {{...}} | {{...}} | {{...}} | {{mm:ss}} | {{1–5}} | {{...}} |
| UT03 | {{...}} | {{...}} | {{...}} | {{...}} | {{mm:ss}} | {{1–5}} | {{...}} |
| UT04 | {{...}} | {{...}} | {{...}} | {{...}} | {{mm:ss}} | {{1–5}} | {{...}} |

**Link da gravação (se autorizado):** {{...}}  
**Resposta pós-teste:** {{...}}

## D. Consolidação por tarefa

| Tarefa | Taxa de sucesso | Tempo típico | Erros recorrentes | Satisfação | Meta atendida? | Problemas prioritários |
|---|---:|---|---|---|---|---|
| UT01 | {{...}} | {{...}} | {{...}} | {{...}} | {{sim/não}} | {{...}} |
| UT02 | {{...}} | {{...}} | {{...}} | {{...}} | {{sim/não}} | {{...}} |
| UT03 | {{...}} | {{...}} | {{...}} | {{...}} | {{sim/não}} | {{...}} |
| UT04 | {{...}} | {{...}} | {{...}} | {{...}} | {{sim/não}} | {{...}} |

## E. Achados e recomendações

| ID | Achado | Evidência (quant. + qual.) | Impacto | Recomendação | Artefatos a revisar |
|---|---|---|---|---|---|
| AU01 | Dificuldade para identificar as fontes institucionais apresentadas nas respostas. | U01, UT02: foi registrado 1 erro, tempo de 01:45 e satisfação de 4/5. O participante demorou para localizar a referência institucional e mencionou no pós-teste que as fontes poderiam receber maior destaque visual. | Médio | Melhorar o destaque visual das fontes, utilizando links mais evidentes e identificação clara das referências institucionais. | Protótipo Figma, modelo conceitual e signos de interface. |
| AU02 | Falta de orientação clara após respostas sem informações suficientes. | U01, UT04: a tarefa foi concluída parcialmente, com 1 erro, 1 ajuda, tempo de 02:10 e satisfação de 3/5. O participante apresentou dificuldade para identificar como continuar a consulta e mencionou a necessidade de orientações mais claras. | Alto | Apresentar sugestões para reformular perguntas e indicar alternativas de consulta aos setores responsáveis da FEI. | Protótipo Figma, MoLIC e fluxos de recuperação de erros. |

## F. Comparação com a avaliação heurística

| Problema | Detectado na heurística? | Detectado por usuários? | O que aprendemos |
|---|---|---|---|
| Dificuldade para identificar as fontes institucionais apresentadas nas respostas. | A confirmar com os registros da Entrega 13. | Sim, identificado por U01 na tarefa UT02. | A apresentação das fontes institucionais influenciou a facilidade de identificação da origem das informações. O participante conseguiu concluir a tarefa, mas apresentou dificuldade inicial para localizar a referência. |
| Falta de orientação clara após respostas sem informações suficientes. | A confirmar com os registros da Entrega 13. | Sim, identificado por U01 na tarefa UT04. | O participante compreendeu que o assistente não possuía informações suficientes, mas apresentou dificuldade para identificar como continuar a consulta. Isso reforçou a importância de oferecer alternativas de recuperação. |

## G. Conclusão

A conclusão deve responder:

1. Quais metas de usabilidade foram atingidas?
2. Quais problemas foram recorrentes e com quais perfis/tarefas?
3. O que surpreendeu a equipe?
4. Quais mudanças são prioritárias?
5. Que limitações do teste impedem generalizações amplas?

Com base na avaliação individual de U01, foram identificados resultados positivos relacionados à facilidade de utilização do Assistente Virtual Acadêmico da FEI.

Das quatro tarefas propostas, três foram concluídas totalmente e uma parcialmente, representando uma taxa de sucesso total de 75%.

O participante não apresentou dificuldades relevantes nas tarefas relacionadas à consulta sobre rematrícula e à utilização do histórico de conversas.

Entretanto, foram identificadas dificuldades relacionadas à localização das fontes institucionais e à recuperação após respostas inconclusivas.

A tarefa UT04 apresentou a maior dificuldade, exigindo uma orientação do moderador para que o participante identificasse uma alternativa de continuidade.

A satisfação média de U01 foi de 4,25 em uma escala de 1 a 5, indicando uma percepção positiva da interface, apesar dos problemas encontrados.

As principais recomendações envolveram o aumento da visibilidade das fontes institucionais e a apresentação de orientações mais claras quando o assistente não consegue responder adequadamente.

Esses resultados contribuíram para avaliar as metas de compreensão, eficácia, eficiência, satisfação e recuperação de erros estabelecidas anteriormente pela equipe.

A conclusão consolidada sobre o atendimento das metas, a recorrência dos problemas e as prioridades de melhoria será finalizada após a inclusão dos resultados de U02.

A quantidade reduzida de participantes e a utilização de um protótipo limitarão a generalização dos resultados para todos os estudantes da FEI.

## Checklist

- [ ] Número de participantes finais atende ao enunciado.
- [ ] Participantes são representativos do público e não são membros da equipe.
- [ ] Se foram usados participantes proxy, a justificativa e a limitação estão explícitas.
- [x] O teste avalia a interação; não confunde usabilidade do protótipo com desempenho técnico do TCC.
- [x] Tarefas administrativas/analíticas usadas no teste são rastreáveis a objetivos e cenários.
- [ ] Há consentimento e anonimização.
- [x] Foi realizado teste piloto.
- [x] Tarefas têm critérios de sucesso definidos antes do teste.
- [ ] Moderadores não ensinaram o caminho durante a tarefa.
- [ ] Resultados estão separados por usuário e por tarefa.
- [ ] Foram registrados sucesso, erros, ajudas, tempo e satisfação quando aplicáveis.
- [ ] Conclusão combina evidência quantitativa e qualitativa.
- [x] Achados geram recomendações e atualização da rastreabilidade.
