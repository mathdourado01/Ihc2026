# Matriz de rastreabilidade de IHC

A matriz deve ser atualizada ao longo do semestre. Ela ajuda a demonstrar que a interface não surgiu arbitrariamente e registra **como o conhecimento da equipe evoluiu**.

Para projetos cujo TCC não previa interface, esta matriz é especialmente importante: deve ficar visível a passagem da **contribuição técnica do TCC** para um **cenário de uso plausível**, e desse cenário para as decisões de interação.

## 1. Derivação do escopo de IHC a partir do TCC

| Elemento | Registro da equipe | Evidência/justificativa | Estado |
|---|---|---|---|
| Tema do TCC | Assistente Virtual com Inteligência Artificial para Suporte a Dúvidas Acadêmicas e Administrativas na FEI | TCC e seção 0.2 da Entrega 1 | definido |
| Resultado técnico esperado | Desenvolvimento de um protótipo funcional de assistente virtual capaz de recuperar informações institucionais e gerar respostas em linguagem natural, acompanhado de avaliação experimental da arquitetura | TCC e seção 0.4 da Entrega 1 | definido |
| O TCC previa interface? | Sim | O TCC prevê formalmente uma interface na qual o usuário envia perguntas em linguagem natural, recebe respostas fundamentadas nas informações institucionais recuperadas e mantém a continuidade da interação durante a sessão | definido |
| Capacidade/contribuição central | Recuperar informações relevantes de uma base documental institucional e utilizá-las como evidência para gerar respostas em linguagem natural a dúvidas acadêmicas e administrativas | TCC e seção 1.3 da Entrega 1 | definido |
| Possíveis beneficiários/stakeholders | Estudantes da FEI; equipe responsável pelo desenvolvimento e avaliação do sistema; profissionais e setores da FEI responsáveis por processos e informações acadêmico-administrativas | Seções 2.1, 2.2 e 2.3 da Entrega 1 | F/H conforme participação |
| Usuário escolhido para IHC | Estudante da FEI que necessita localizar ou compreender uma informação acadêmica ou administrativa | O estudante é o usuário direto previsto no TCC e realiza as atividades A01 e A02 definidas na Entrega 1 | F |
| Personas priorizadas | P01 — Lucas Almeida e P02 — Mariana Costa, ambas classificadas como personas primárias | Entrega 3. P01 representa principalmente A01 e P02 representa principalmente A02. Ambas permanecem proto-personas a validar com estudantes reais | definido para o projeto de IHC |
| Objetivo principal do usuário | Obter e compreender uma informação acadêmica ou administrativa para resolver uma dúvida, tomar uma decisão ou realizar corretamente um procedimento relacionado à sua vida acadêmica | H04, seção 3.1 e seção 7.3 da Entrega 1 | H |
| Contexto de uso adotado | Situações em que o estudante precisa esclarecer uma dúvida acadêmica ou administrativa, dentro ou fora da FEI, possivelmente por computador, notebook ou dispositivo móvel | H11 e H12 da Entrega 1; aprofundado na Entrega 3 por meio de situações hipotéticas de P01 e P02 | H |
| Interface/recorte de IHC | Fluxo conversacional no qual o estudante formula uma dúvida, recebe e compreende uma resposta, pode consultar a fonte institucional utilizada, continuar a conversa durante a sessão e é informado quando não existe evidência suficiente para responder | Seções 7.1 e 7.4 da Entrega 1; deriva das capacidades previstas no TCC e das atividades A01 e A02 | proposta |
| Relação com o TCC | parte prevista | A interface conversacional e a manutenção do histórico durante a sessão já fazem parte do protótipo previsto no TCC. A disciplina de IHC aprofundará os aspectos de interação e usabilidade | definido |

> Se o escopo de IHC mudar ao longo do semestre, preserve a decisão anterior no histórico e registre **qual evidência motivou a mudança**.

---

## 2. Registro de hipóteses e lacunas da Entrega 1

Use esta tabela para itens importantes marcados como `[H]` ou `[?]`. Preserve o histórico: não apague uma hipótese refutada.

| ID | Afirmação / dúvida inicial | Tipo | Por que importa | Como/onde investigar | Evidência obtida | Estado atual | Impacto no projeto |
|---|---|---|---|---|---|---|---|
| H02 | A fundamentação em fontes institucionais pode aumentar a confiança e a utilidade percebida da resposta em comparação com respostas sem contexto documental. | H | Justifica investigar confiança e utilidade das fontes. | Entrega 07 — I01, pergunta 8; avaliação específica de confiança e utilidade em etapa futura. | I01 investiga a importância declarada das fontes. HC01 e AU01 mostram dificuldades de identificação das fontes, mas não demonstram efeito causal sobre a confiança. | aberta | Apresentação e fundamentação das fontes institucionais em R02. |
| H04 | O estudante busca obter e compreender informações acadêmicas ou administrativas para resolver dúvidas, tomar decisões ou realizar corretamente procedimentos relacionados à vida acadêmica. | H | Define o objetivo principal do usuário e orienta quais tarefas deverão ser priorizadas na interface. | **Entrega 07 —** investigação com estudantes da FEI sobre objetivos, necessidades e processo atual. | A Entrega 3 utilizou H04 na construção de P01 e P02, mas as personas são hipotéticas e não confirmam a hipótese. I01, perguntas 2 e 3, e I02 foram preparados, sem coleta. A Entrega 14 demonstra a execução de consultas simuladas, mas não valida a frequência ou necessidade real. | aberta | Pode confirmar ou exigir revisão do objetivo principal e das tarefas priorizadas. |
| H05 | Localizar e compreender informações acadêmicas ou administrativas é uma das atividades mais frequentes dos estudantes nesse contexto. | H | Ajuda a verificar se A01 deve ser considerada a atividade principal do projeto de IHC. | **Entrega 07 —** investigação com estudantes sobre frequência e situações de ocorrência. | I01, perguntas 2 e 3, e I02 foram preparados. A coleta não foi realizada. | aberta | Pode confirmar ou alterar a prioridade das atividades e tarefas da interface. |
| H06 | Compreender e realizar procedimentos acadêmicos ou administrativos é uma atividade de maior criticidade quando envolve regras, etapas obrigatórias ou prazos. | H | A criticidade pode exigir maior cuidado na apresentação das respostas, fontes, limitações e orientações. | **Entrega 07 —** investigação com estudantes e, quando pertinente, profissionais ou setores responsáveis. | P02 — Mariana representa esse tipo de consulta na Entrega 3, mas sua construção como proto-persona não confirma frequência ou criticidade. I01, perguntas 3 e 7, foi preparado, sem coleta. A Entrega 8 prioriza a prevenção de erros. | aberta | Pode influenciar o detalhamento das respostas e os mecanismos de prevenção e recuperação de erros. |
| H07 | Estudantes podem recorrer a diferentes canais institucionais ou pessoas, conforme o tipo de dúvida. | H | Permite compreender o processo atual de busca por informações acadêmicas e administrativas. | **Entrega 07 —** I01, pergunta 4, e I02. | Os instrumentos foram preparados, mas não foram coletadas informações sobre os canais efetivamente utilizados pelos estudantes. | aberta | Pode influenciar o fluxo de consulta e as sugestões de assuntos relacionadas a R01. |
| H08 | A distribuição das informações entre diferentes páginas, documentos e canais pode aumentar o esforço necessário para o estudante resolver uma dúvida. | H | Representa um dos principais problemas que justificam o fluxo de consulta centralizado proposto para o assistente. | **Entrega 07 —** investigação do processo atual e dos canais utilizados pelos estudantes. | Utilizada como hipótese na persona P01, no mapa de empatia e na jornada da Entrega 3. I01, perguntas 4 e 6, e I02 foram preparados, mas não houve coleta sobre o esforço real de busca. | aberta | Se sustentada, reforça o fluxo centralizado de consulta; se refutada, pode exigir revisão da caracterização do problema. |
| H09 | Informações relacionadas a regras, procedimentos, requisitos ou prazos podem exigir interpretação por parte do estudante. | H | Consultas desse tipo podem exigir respostas mais organizadas e cuidadosas do que dúvidas puramente informacionais. | **Entrega 07 —** investigação com estudantes e, quando pertinente, setores responsáveis. | Representada em P01 e P02 na Entrega 3. I01, perguntas 5, 6 e 11, e I02 foram preparados. AU02 demonstra dificuldades em uma situação simulada, sem permitir generalização para o público. | aberta | Pode influenciar a estruturação das respostas procedimentais e a apresentação de regras, etapas, requisitos e prazos. |
| H10 | Uma interpretação equivocada de uma orientação acadêmica ou administrativa pode levar o estudante a executar incorretamente um procedimento, deixar de cumprir uma etapa ou perder um prazo. | H | Ajuda a identificar situações em que erros de compreensão podem afetar a execução de uma tarefa acadêmica ou administrativa. | **Entrega 07 —** investigação de situações de falha, consequências e busca de ajuda. | A jornada de P01 e a caracterização de P02 incorporam esse risco como hipótese. I01, perguntas 7 e 11, foi preparado, mas não existem evidências coletadas sobre consequências acadêmicas reais. | aberta | Pode influenciar mecanismos de prevenção de erro, organização das respostas e destaque de informações críticas. |
| H11 | A interação pode ocorrer dentro ou fora da FEI, conforme a situação acadêmica. | H | Orienta decisões sobre o contexto físico de utilização. | Investigação futura do local e contexto de utilização. | O contexto físico ainda não foi medido. A pergunta 9 do I01 identifica dispositivos, mas não permite determinar diretamente o local de utilização. | aberta | Adequação da interface ao contexto de uso. |
| H12 | O acesso pode ocorrer por computador, notebook ou dispositivo móvel. | H | Orienta decisões sobre responsividade e adaptação da interface. | **Entrega 07 —** I01, pergunta 9. | O questionário foi preparado, mas não houve coleta. A Entrega 8 propõe larguras de referência de 360 e 1280 pixels, que constituem critérios de projeto, não resultados de testes. | aberta | Legibilidade e acesso aos elementos essenciais em diferentes dispositivos. |
| H14 | A confiabilidade percebida pelo estudante poderá ser influenciada pela clareza sobre a origem institucional das informações apresentadas. | H | Pode justificar a apresentação das fontes e determinar como essas informações deverão aparecer na interface. | **Entrega 07 —** investigação com usuários; **Entrega 12 —** planejamento da avaliação; **Entrega 14 —** observação de usuários. | Na Entrega 2, os concorrentes C01 — ChatGPT e C02 — Gemini demonstraram padrões de apresentação de fontes. Na Entrega 3, a consulta à fonte aparece nas personas e na jornada. I01, pergunta 8, foi preparado. HC01 e AU01 evidenciam dificuldades de identificação das fontes, mas não medem diretamente a confiança percebida. | aberta | Pode influenciar a visibilidade, organização e detalhamento das fontes institucionais. |
| H15 | A recuperação de conversas realizadas em sessões anteriores pode ser útil para o estudante retomar informações ou consultas feitas em outro momento. | H | Permite decidir se persistência e recuperação entre sessões representam uma necessidade real, distinta da continuidade já prevista durante a sessão atual. | **Entrega 07 —** investigação da necessidade com estudantes; avaliação exploratória na Entrega 14. | Na Entrega 2, os concorrentes C01 e C02 apresentam histórico de conversas. A Entrega 3 preserva essa possibilidade como hipótese. I01, pergunta 10, foi preparado. F05 representa um histórico simulado, acessado por 2/2 participantes na UT03 da Entrega 14. Esse resultado demonstra a utilização do recurso no teste, mas não confirma sua necessidade real. | aberta | Pode confirmar, modificar ou remover a recuperação de conversas entre sessões, sem afetar a continuidade já prevista dentro da sessão. |
| H16 | Uma resposta incorreta ou uma interpretação equivocada sobre regras, prazos ou procedimentos pode produzir consequências relevantes para o estudante. | H | Influencia diretamente o tratamento de erros, ausência de evidência, avisos e encaminhamento para canais oficiais. | **Entrega 07 —** investigação das consequências percebidas; **Entrega 12 —** planejamento da avaliação; **Entrega 13 —** avaliação heurística; **Entrega 14 —** observação de usuários. | Na Entrega 2, foram observados riscos de imprecisão em sistemas generativos. P01 e P02 possuem situações em que informação insuficiente exige outra forma de confirmação. I01, perguntas 7 e 11, foi preparado. AU02 evidencia dificuldades de recuperação no protótipo, mas não consequências acadêmicas reais. | aberta | Pode justificar mensagens de cautela, tratamento explícito da ausência de evidência e encaminhamento para canais oficiais. |
| H18 | O padrão de interação utilizado por assistentes como ChatGPT, Gemini e Copilot pode ser familiar aos estudantes da FEI. | H | Pode sustentar ou questionar a escolha de uma interface conversacional como principal forma de interação. | **Entrega 02 —** análise de interfaces existentes; **Entrega 07 —** investigação da familiaridade dos estudantes. | Na Entrega 2, os concorrentes C01 e C02 demonstraram padrões conversacionais. Na Entrega 3, esse padrão foi utilizado como referência nas proto-personas. I01, perguntas 12 e 13, foi preparado, sem coleta. AU03 aponta necessidade de esclarecimentos durante a interação, mas não mede a familiaridade prévia com IA. | aberta | Pode confirmar o padrão conversacional ou indicar necessidade de adaptação do fluxo de interação. |

### Instrumentos da Entrega 7

| ID | Responsável | Hipóteses/dados investigados | Situação | Decisão de design relacionada |
|---|---|---|---|---|
| I01 — Questionário | Matheus Dourado Valle | H02, H04, H05, H06, H07, H08, H09, H10, H12, H14, H15, H16 e H18: frequência, canais, dificuldades, fontes, dispositivos, histórico e familiaridade com IA. | [Google Forms publicado](https://docs.google.com/forms/d/e/1FAIpQLSdEVU2WLhhA-rumpGj_FIY1asA0vgKm6zGzQPv-tMY77aN_Rg/viewform?usp=publish-editor). Validação funcional confirmada pela equipe em 25/11/2026. Coleta não realizada. | R01, R02, R03, R04 e R07: prioridades, fontes, recuperação, histórico e linguagem. |
| I02 — Classificação de Cartões (Card Sorting aberto) | João Pedro Sabino Garcia | H04, H05, H07, H08 e H09: agrupamentos, vocabulário e assuntos relacionados. | Planejamento, 16 cartões, tabuleiro textual e ficha de registro definidos na Entrega 7. Coleta não realizada. | R01 e R07: exemplos de perguntas, sugestões de assuntos e linguagem, sem pressupor menus obrigatórios. |

A preparação dos instrumentos não representa validação empírica das hipóteses.

Após o feedback da Entrega 7, o questionário foi implementado no Google Forms, publicado e validado funcionalmente pela equipe. O procedimento do Card Sorting foi complementado com a definição de materiais, modalidade de aplicação, recrutamento, registro e análise dos resultados.

Para uma eventual aplicação futura, foram estabelecidas metas exploratórias de 20 participantes para I01 e cinco participantes para I02.

A equipe optou por não realizar a coleta de dados nesta etapa. Dessa forma, as hipóteses investigadas permanecem abertas e não serão consideradas confirmadas apenas pela preparação dos instrumentos.

H11 permanece aberta por não ser diretamente investigada pelas perguntas do questionário.

---

## 3. Rastreabilidade entre contribuição técnica, necessidades e artefatos

| ID | Capacidade do TCC utilizada | Necessidade/problema | Persona | Cenário problema | Objetivo/tarefa | HTA/GOMS/CTT | Cenário de interação / signos | MoLIC | Tela(s) Figma | Heurística / problema | Tarefa no teste | Decisão/melhoria |
|---|---|---|---|---|---|---|---|---|---|---|---|---|
| R01 | Receber uma pergunta em linguagem natural, recuperar informações institucionais relevantes e gerar uma resposta fundamentada. | H04, H05, H07 e H08 — necessidade de localizar e compreender informações e possível esforço causado pela distribuição das informações entre diferentes fontes. | P01 — Lucas Almeida, persona primária. P02 — Mariana Costa no contexto de consultas procedimentais. | **Cenário C01 — Entrega 04:** localização e compreensão de uma informação acadêmica. C02 no domínio de consultas procedimentais. | TI01 — Formular e enviar dúvida; TI02 — compreender resposta. | HTA T01; GOMS T02; CTT T03; HTA T04, GOMS T05 e CTT T06 no domínio do mestrado. | CI01/CI02; O01–O04, O09 e O11–O14; Dúvida, Assunto acadêmico, Resposta, Orientação acadêmica e Processo de ingresso. | M01/M02 | F01, F03, F07; F06, referente às categorias opcionais. | H7 e H10: boas práticas identificadas. AU03: necessidade de esclarecimentos durante a utilização. | Entrega 12: UT01 e UT02. Entrega 14: UT01 e UT02, consultas sobre rematrícula e declaração. | Manter a formulação da consulta como ação principal, conforme RC01 e RC08. Melhorar instruções e rótulos conforme AU03. Alinhar CI01 e M01, sobre alteração de matrícula, com o conteúdo de F03. |
| R02 | Preservar os metadados dos documentos e disponibilizar a origem das informações utilizadas na resposta. | H02 e H14 — a clareza sobre a origem institucional das informações pode influenciar a confiabilidade percebida. | P01 — Lucas Almeida; P02 — Mariana Costa. | **Cenários C01 e C02 — Entrega 04.** | TI03 — Identificar e consultar a fonte institucional associada à resposta. | HTA T01; CTT T03; HTA T04; GOMS T05; CTT T06. | CI01/CI02; O01/O05; Fonte institucional, Resposta e Orientação acadêmica. | M01/M02 | F03, F07, F15, F16; F10, referente às fontes gerais. | HC01 — H6, severidade 3; AU01 — dificuldade de identificação das fontes. | Entrega 12: UT03. Entrega 14: UT02, consulta e verificação de fonte. | RC03: relacionar claramente as informações apresentadas às respectivas fontes. Apresentar título, órgão responsável, data ou vigência e caminho de consulta quando disponíveis. Melhoria planejada a partir de HC01 e AU01. |
| R03 | Reconhecer quando não existe evidência documental suficiente e evitar gerar respostas sem fundamento institucional. | H06, H09, H10 e H16 — informação insuficiente ou interpretação incorreta pode impedir que o estudante conclua sua tarefa com segurança. | P01 — Lucas Almeida; P02 — Mariana Costa. | **Jornada P01 — Entrega 03:** desfecho com informação insuficiente. **Cenário C02 — Entrega 04:** consulta procedimental. | TI05 — Reconhecer a ausência de evidência suficiente e identificar como prosseguir. | HTA T01, relacionado ao refinamento da consulta; HTA T04 e CTT T06, relacionados à decisão e verificação. Não existe modelo exclusivo para TI05. | CI01/CI02; O07/O08; Ausência de evidência e Orientação de encaminhamento. | M01/M02 | F04; F08, falha operacional distinta; F13, contexto insuficiente distinto. | H5 e H9: boas práticas identificadas. HC02 — H4, severidade 2, em F08. AU02 — dificuldade no tratamento da resposta inconclusiva. | Entrega 12: UT05. Entrega 14: UT04. HC02 não foi confirmado especificamente nos testes com usuários. | RC04: comunicar a ausência de evidência e orientar como prosseguir. Destacar alternativas de recuperação e encaminhamento. Unificar ou esclarecer ações de F08. Diferenciar contexto insuficiente, ausência de evidência e falha operacional. |
| R04 | Possibilidade de armazenar e recuperar conversas realizadas em sessões diferentes. | H15 — recuperação de conversas anteriores pode ser útil para retomar uma consulta realizada em outro momento. | P01 — Lucas Almeida; P02 — Mariana Costa. | Não existe cenário de problema específico. H15 permanece em investigação. | TI06 — Recuperar conversas realizadas em sessões anteriores. | Não modelada como tarefa autônoma na Entrega 5. O identificador T06 não representa recuperação de histórico. | Não existe cenário específico em CI01/CI02 nem signo de persistência entre sessões definido na Entrega 9. | Não existe fluxo específico de recuperação entre sessões em M01/M02. | F05 — histórico simulado, descrito no catálogo da Entrega 11. | Não existe achado heurístico consolidado específico. Na Entrega 14, UT03 foi concluída sem erros ou pedidos de ajuda. | Não prevista nas tarefas UT01–UT05 do DECIDE. Entrega 14: UT03 — histórico. | RC07: manter o histórico entre sessões como possibilidade a investigar. A conclusão da tarefa por 2/2 participantes não confirma a necessidade de persistência real entre sessões. |
| R05 | Manter o histórico e o contexto das interações durante a sessão atual. | Necessidade de permitir continuidade da consulta e perguntas complementares dentro da mesma conversa. | P01 — Lucas Almeida; P02 — Mariana Costa. | **Jornada P01 — Entrega 03; cenários C01 e C02 — Entrega 04.** | TI04 — Formular uma pergunta complementar dentro da mesma sessão. | HTA T01, refinamento; GOMS T02, pergunta complementar; CTT T03, nova consulta; GOMS T05, esclarecimento. | CI01/CI02; O03/O06; Pergunta complementar e Contexto da conversa. | M01/M02 | F03, F07, F09, F12, F13; F01, campo de consulta. | H3: boa prática identificada. AU02 está relacionado à recuperação, não à validação da continuidade contextual. | Entrega 12: UT04. Não existe tarefa específica de pergunta complementar dependente do contexto na Entrega 14. | RC02: estruturar a interface de forma conversacional. PF02 demonstra continuidade visual, mas não comprova compreensão contextual. Verificar essa capacidade em avaliação futura. |
| R06 | Receber a consulta, processar a recuperação e gerar a resposta por meio de serviços externos. | Possível espera entre o envio da pergunta e a apresentação da resposta. | P01 — Lucas Almeida; P02 — Mariana Costa. | **Jornada P01 — Entrega 03; cenários C01 e C02 — Entrega 04.** | Fluxo TI01 → TI02 — reconhecer o estado de processamento. | HTA T01; CTT T03; HTA T04; CTT T06. | CI01/CI02; O10; Estado da consulta. | M01/M02 | F02, F11; F08, situação de falha. | H1: boa prática observada. HC02 — H4, relacionada à recuperação de falhas. | Entrega 12: UT01 e QA08. Não existe registro específico do reconhecimento do processamento na Entrega 14. | RC06: fornecer feedback compreensível durante a espera. Diferenciar processamento de falha e revisar os rótulos de recuperação em F08. |
| R07 | Apresentar a interação ao usuário sem expor desnecessariamente detalhes técnicos internos da arquitetura. | Necessidade de utilizar linguagem compreensível e adequada ao contexto acadêmico-administrativo. | P01 — Lucas Almeida; P02 — Mariana Costa. | **Jornada P01 — Entrega 03; cenários C01 e C02 — Entrega 04.** | TI01 e TI02 — formular consulta e compreender resposta em linguagem familiar. | HTA T01/T04; GOMS T02/T05; CTT T03/T06. | CI01/CI02; O02/O04, O09 e O11–O14; Dúvida, Resposta, Orientação acadêmica e Processo de ingresso. | M01/M02 | F01, F03, F04, F07, F08, F15 e F16. | H2, H8 e H10: boas práticas identificadas. AU03 e HC01 apontam oportunidades de melhoria na clareza e apresentação das informações. | Entrega 12: UT01 e UT02. Entrega 14: UT01, UT02 e UT04, por meio de observações qualitativas. | RC05: utilizar vocabulário acadêmico-administrativo e evitar termos como RAG, embeddings, chunks e banco vetorial no fluxo do estudante. Revisar os detalhes técnicos presentes nas telas da Entrega 6 e a clareza dos rótulos e fontes. |

> As personas **P01 — Lucas Almeida** e **P02 — Mariana Costa** foram definidas na Entrega 3 como **personas primárias e proto-personas a validar**. Elas representam, respectivamente, necessidades relacionadas principalmente às atividades A01 e A02. Sua criação não confirma as hipóteses comportamentais às quais estão relacionadas.

> Os identificadores **concorrente C01 — Entrega 02** e **concorrente C02 — Entrega 02** referem-se, respectivamente, às análises do ChatGPT e do Google Gemini. Os identificadores **cenário C01 — Entrega 04** e **cenário C02 — Entrega 04** referem-se aos cenários de análise/problema definidos posteriormente.

> Os vínculos apresentados registram os artefatos existentes no projeto e as revisões realizadas nas Entregas 7 e 8. A inclusão de um artefato na matriz não significa que todos os problemas identificados pelo professor tenham sido corrigidos ou que sua qualidade tenha sido empiricamente validada.

> As telas F05, F06, F09, F10, F12, F13 e F14 encontram-se descritas no catálogo da Entrega 11, sem captura individual no conjunto de arquivos analisado. As demais nove telas possuem evidência visual correspondente.

### Identificadores e correspondência entre tarefas

A fim de resolver os conflitos de identificadores observados ao longo das entregas, os códigos T01 a T06 serão reservados aos modelos de análise de tarefas da Entrega 5.

Os códigos TI01 a TI06 representarão as tarefas gerais de interação do estudante.

| ID estável de interação | Significado | Modelos da Entrega 5 relacionados | Tarefa planejada — Entrega 12 | Tarefa executada — Entrega 14, código original |
|---|---|---|---|---|
| TI01 | Formular e enviar uma consulta. | T01 — HTA; T02 — GOMS; T04 — HTA; T05 — GOMS. | UT01 | UT01 e UT02 — consultas acadêmicas. |
| TI02 | Ler e compreender a resposta. | T01 — HTA; T03 — CTT; T04 — HTA; T06 — CTT. | UT02 | UT01 e UT02 — compreensão incluída, sem critério isolado padronizado. |
| TI03 | Identificar e consultar a fonte institucional. | T01 — HTA; T03 — CTT; T04 — HTA; T05 — GOMS; T06 — CTT. | UT03 | UT02 — declaração e verificação de fonte. |
| TI04 | Formular uma pergunta complementar durante a mesma sessão. | T01 — HTA; T02 — GOMS; T05 — GOMS. | UT04 | Não testada isoladamente. |
| TI05 | Reconhecer ausência de evidência suficiente e identificar como prosseguir. | T01 — HTA, refinamento; T04 — HTA; T06 — CTT, decisão. Não existe modelo exclusivo para TI05. | UT05 | UT04 — resposta inconclusiva. |
| TI06 | Recuperar uma conversa realizada em sessão anterior, associada à hipótese H15. | Não existe modelo específico na Entrega 5. | Não prevista. | UT03 — histórico simulado. |

Os identificadores T01 a T06 permanecem associados aos seis modelos originais produzidos na Entrega 5.

| ID | Técnica | Responsável | Artefato relacionado |
|---|---|---|---|
| T01 | HTA | Matheus Dourado Valle | Obtenção de resposta para uma dúvida acadêmica. |
| T02 | GOMS | Matheus Dourado Valle | Consulta ao assistente virtual, incluindo alternativas de interação. |
| T03 | CTT | Matheus Dourado Valle | Interação, leitura da resposta e decisão sobre a continuidade da consulta. |
| T04 | HTA | João Pedro Sabino Garcia | Compreensão das etapas, requisitos e prazos para ingresso em programa de mestrado. |
| T05 | GOMS | João Pedro Sabino Garcia | Consulta e confirmação de requisitos relacionados ao ingresso no mestrado. |
| T06 | CTT | João Pedro Sabino Garcia | Interpretação da orientação recebida e definição do próximo passo. |

Os códigos TI01 a TI05 seguem a padronização estabelecida na revisão da Entrega 8. TI06 preserva a atividade de recuperação de histórico que já estava presente na matriz original.

Os identificadores UT das Entregas 12 e 14 possuem significados parcialmente diferentes. Até que os documentos sejam revisados, deverão ser acompanhados da identificação da respectiva entrega.

A correspondência apresentada não representa uma renomeação retroativa das tarefas executadas durante os testes.

As telas P01 a P06 da Entrega 6 também deverão ser qualificadas como telas da Entrega 6, evitando confusão com as personas P01 e P02.

### Metas, princípios e avaliações — Entrega 8

Após o feedback da Entrega 8, os princípios gerais do projeto foram separados em princípios direcionados ao negócio e princípios direcionados à interface.

Os princípios de negócio consideram o contexto acadêmico-administrativo, a proteção de dados pessoais, o uso de fontes institucionais, o tratamento responsável de informações críticas e o encaminhamento aos setores responsáveis.

Os princípios de interface consideram a Engenharia de Usabilidade de Mayhew, a ISO 9241-11, a WCAG 2.2, as heurísticas e metas de Nielsen, os padrões conversacionais, a apresentação de fontes, o feedback e a prevenção de erros.

| Requisito | Metas de usabilidade associadas | Princípios aplicáveis | Planejamento DECIDE | Evidência e situação |
|---|---|---|---|---|
| R01 | MU01, MU02, MU06 e MU07. | Contexto de uso, interação conversacional e ISO 9241-11. | QA01, QA02, QA06 e QA07; UT01 e UT02. | Entrega 14, UT01: 2/2 participantes concluíram a tarefa, com satisfação média de 5/5. MU01 e MU02 permanecem inconclusivas quanto aos critérios específicos. MU06 não possui registro isolado do tempo até o envio da pergunta. |
| R02 | MU03 e MU07. | Fontes institucionais, tratamento de informações críticas, apresentação de fontes e heurísticas de Nielsen. | QA03 e QA07; UT03. | Entrega 14, UT02: 2/2 participantes concluíram a tarefa, com satisfação média de 4,5/5. HC01 e AU01 indicam oportunidades de melhoria. MU03 não foi medida isoladamente. |
| R03 | MU05 e MU07. | Tratamento de informações críticas, encaminhamento institucional, prevenção e recuperação de erros. | QA05, QA07 e QA09; UT05. | Entrega 14, UT04: um participante concluiu integralmente e outro apresentou conclusão parcial, com satisfação média de 4/5. AU02 evidencia dificuldade de recuperação. Os registros não permitem comprovar separadamente todos os critérios previstos em MU05. |
| R04 | Sem meta quantitativa específica nesta etapa. | Contexto de uso, minimização de dados e recuperação de histórico como hipótese. | Não existe tarefa prevista especificamente no DECIDE. I01, pergunta 10. | Entrega 14, UT03: 2/2 participantes concluíram sem erros ou pedidos de ajuda, com satisfação média de 5/5. O resultado não confirma a hipótese H15 sobre a necessidade real de recuperação entre sessões. |
| R05 | MU04 e MU07. | Interação conversacional e continuidade durante a sessão. | QA04 e QA07; UT04. | Não houve teste específico de pergunta complementar dependente do contexto anterior na Entrega 14. MU04 permanece não avaliada diretamente. |
| R06 | MU08, de caráter qualitativo. | Feedback, visibilidade do estado do sistema e recuperação de falhas. | QA08 e QA09; UT01. | H1 foi identificada como boa prática na avaliação heurística. Não existe registro comportamental específico suficiente para verificar MU08 nos testes com usuários. |
| R07 | MU01, MU02 e MU07, de forma transversal. | Linguagem familiar, acessibilidade, minimização de jargão técnico e clareza. | QA01, QA02, QA07 e QA09; UT01 e UT02. | AU03 indica necessidade de esclarecimentos durante a interação, apesar da satisfação elevada. Não houve medição isolada da compreensão dos termos e da linguagem da interface. |

As metas de usabilidade preservam seus significados originais:

| ID | Meta de usabilidade | Limite de referência |
|---|---|---|
| MU01 | Taxa de conclusão da formulação e envio de consulta sem ajuda. | ≥ 90% |
| MU02 | Taxa de compreensão correta da resposta. | ≥ 80% |
| MU03 | Tempo mediano para localizar a fonte institucional. | ≤ 30 segundos |
| MU04 | Taxa de conclusão de pergunta complementar sem ajuda. | ≥ 80% |
| MU05 | Taxa de interpretação correta da ausência de evidência suficiente. | ≥ 90% |
| MU06 | Tempo mediano para iniciar uma consulta. | ≤ 60 segundos |
| MU07 | Média da satisfação pós-tarefa em escala de 1 a 5. | ≥ 4,0 em cada tarefa |
| MU08 | Reconhecimento do estado de processamento da consulta. | Indicador qualitativo e observacional. |

A priorização das metas da Entrega 8 foi reorganizada considerando exclusivamente as cinco metas de usabilidade de Nielsen.

| Meta de Nielsen | Peso de prioridade | Indicadores associados |
|---|---:|---|
| Facilidade de aprendizado | 25% | MU01, MU02, MU04 e MU08. |
| Facilidade de memorização | 10% | MU01, MU04 e MU06, em eventual avaliação repetida após intervalo sem utilização. |
| Eficiência | 20% | MU03 e MU06. |
| Baixa taxa de erro | 30% | MU02, MU05 e MU08, além do registro complementar de erros e pedidos de ajuda. |
| Satisfação positiva do usuário | 15% | MU07. |
| **Total** | **100%** | |

Os pesos representam prioridades de projeto, não resultados de avaliação.

A facilidade de memorização não foi medida diretamente, pois não houve procedimento específico de retorno à interface após um intervalo sem utilização.

As métricas MU01 a MU08 mantêm suas definições originais. Os resultados da Entrega 14 deverão ser interpretados considerando as tarefas efetivamente executadas e os dados registrados, sem assumir equivalência integral às tarefas inicialmente planejadas no DECIDE.

Considerando a participação de apenas dois estudantes, os resultados quantitativos deverão ser apresentados acompanhados de valores absolutos e interpretados como evidências exploratórias.

As metas que não possuírem registros suficientes deverão permanecer classificadas como não avaliadas ou inconclusivas, evitando utilizar o tempo total de uma tarefa como substituto para o tempo de uma ação específica.

### Relação com o ciclo de Engenharia de Usabilidade de Mayhew

| Nível | Artefatos relacionados | Decisões e avaliações |
|---|---|---|
| Nível 1 — Projeto essencial | Personas, cenários, modelos HTA/GOMS/CTT, prototipação inicial, instrumentos de coleta e modelo conceitual. Entregas 3, 4, 5, 6, 7 e 9. | Definição e refinamento dos objetivos, tarefas, necessidades, conceitos e fluxos fundamentais de interação. |
| Nível 2 — Padrões de telas e diálogos | Esquema conceitual de signos, diagramas MoLIC e protótipo Figma. Entregas 9, 10 e 11. | Definição de padrões de linguagem, apresentação de fontes, feedback, continuidade da conversa e recuperação de rupturas. |
| Nível 3 — Projeto detalhado | Protótipo navegável, planejamento DECIDE, avaliação heurística e testes observados. Entregas 11, 12, 13 e 14. | Identificação de problemas de usabilidade, análise das metas MU01 a MU08 e definição de melhorias justificadas pelas evidências obtidas. |

As avaliações realizadas poderão motivar o retorno a qualquer um dos níveis da Engenharia de Usabilidade de Mayhew.

Cada melhoria deverá registrar o problema identificado, a evidência que motivou a alteração, o requisito afetado, o artefato revisado e o procedimento previsto para verificar a correção.

---

## 4. Rastreabilidade de padrões de interface

Use esta tabela quando o projeto incorporar padrões como interface conversacional, fontes, histórico ou mecanismos de feedback. O objetivo é **justificar o padrão**, não apenas reproduzir elementos vistos em outros produtos.

| ID da tela/fluxo | Padrão de interface | Objetivo/tarefa que justifica | Informação/ação principal | Evidência de necessidade / origem | Artefatos relacionados |
|---|---|---|---|---|---|
| Tela P01 — Entrega 6; F01 | Campo de entrada em linguagem natural. | TI01 | Formular uma dúvida acadêmica ou administrativa diretamente por texto. | Interface prevista no TCC; RC01 — Entrega 02; P01 e P02 — Entrega 03; H04 ainda aberta quanto às necessidades reais dos estudantes. | R01; HTA T01; GOMS T02; CI01/CI02; M01/M02; MU01/MU06. |
| Telas P03, P04 e P06 — Entrega 6; F03, F07, F09, F12 e F13 | Interface conversacional e continuidade durante a sessão. | TI02 e TI04 | Visualizar perguntas e respostas em sequência e realizar perguntas complementares mantendo o contexto da sessão atual. | **[F]** Histórico durante a sessão previsto no TCC; RC02 — Entrega 02; jornada P01 — Entrega 03. | R01/R05; PF01/PF02; HTA T01; GOMS T02/T05; M01/M02; MU02/MU04. |
| Tela P03 — Entrega 6; F03, F07, F10, F15 e F16 | Apresentação de fontes e evidências. | TI03 | Identificar a origem institucional da informação utilizada para fundamentar a resposta. | Preservação das fontes prevista no TCC; H14; RC03 — Entrega 02; personas e jornada da Entrega 03. | R02; PF01; CTT T03/T06; O05; M01/M02; MU03; HC01/AU01. |
| Tela P05 — Entrega 6; F04 | Tratamento contextualizado da ausência de evidência. | TI05 | Informar quando o assistente não possui informação suficiente e orientar o estudante sobre como prosseguir. | Tratamento previsto no TCC; H06 e H16; RC04 — Entrega 02; desfecho 7B da jornada P01 — Entrega 03. | R03; PF03; O07/O08; M01/M02; MU05; AU02. |
| F05 | Recuperação de conversas entre sessões. | TI06 | Acessar uma consulta realizada em outro momento. | H15; RC07 — Entrega 02; padrão observado nos concorrentes C01 e C02, mas mantido como hipótese na Entrega 3. | R04; H15; Entrega 14, UT03 — histórico simulado. |
| Tela P02 — Entrega 6; F02 e F11 | Feedback de processamento. | Fluxo TI01 → TI02 | Informar que a pergunta foi recebida e está sendo processada quando houver espera perceptível. | Arquitetura do TCC; RC06 — Entrega 02; etapa 4 da jornada P01 — Entrega 03. Evidência empírica específica ainda não obtida. | R06; PF01–PF03; O10; M01/M02; MU08; H1 da avaliação heurística. |
| Telas P01 a P06 — Entrega 6; F01, F03, F04, F07 e F08 | Vocabulário acadêmico-administrativo e ausência de jargão técnico. | TI01 e TI02 | Apresentar comandos, respostas e orientações utilizando linguagem relacionada às atividades do estudante. | RC05 — Entrega 02; caracterização de P01 e P02 — Entrega 03; familiaridade real ainda a investigar. | R07; MU01/MU02; AU03. A Entrega 6 apresenta informações técnicas que deverão ser revistas. |
| Tela P01 — Entrega 6; F01 | Consulta como ação principal, sem navegação obrigatória prévia. | TI01 | Permitir que o estudante inicie a tarefa diretamente pelo campo de consulta. | RC08 — Entrega 02; jornada P01 — Entrega 03. As capturas do Portal do Aluno e Moodle não comprovam excesso de etapas. | R01; PF01; RC08; MU01/MU06; H7 e H10 da avaliação heurística. |
| F08 | Recuperação de falha de processamento. | Fluxo TI01 → TI02 | Tentar novamente, reformular ou encerrar a consulta. | Entrega 10: representação da ruptura operacional. Entrega 13: HC02, relacionada a H4, com severidade 2. | R03/R06; M01/M02; melhoria planejada. |
| F06 | Sugestões ou categorias opcionais de assuntos. | TI01 | Explorar assuntos acadêmicos sem impedir a formulação direta de uma pergunta. | Catálogo da Entrega 11; instrumento I02 da Entrega 7, preparado sem coleta de dados. | R01/R07; RC08. A necessidade de categorias permanece não confirmada. |

> As referências às telas da Entrega 6 são qualificadas pelo contexto da entrega, evitando colisão com os identificadores das personas P01 e P02.

> O recurso de recuperação de conversas entre sessões foi representado no protótipo e utilizado em uma tarefa da Entrega 14. Entretanto, sua necessidade permanece associada à hipótese H15 e não foi confirmada pela coleta de dados da Entrega 7.

> A presença de um padrão em um concorrente ou em uma proto-persona não é considerada evidência suficiente de necessidade para o público da FEI. Quando a necessidade ainda depende de investigação com estudantes, a hipótese correspondente permanece aberta.

---

## 5. Registro de mudanças de escopo e decisões

| Data | O que mudou | Evidência/feedback que motivou | Artefatos afetados | Responsável |
|---|---|---|---|---|
| 01/10/2026 | Foi explicitada a distinção entre continuidade da conversa durante a sessão atual e recuperação de conversas realizadas em sessões anteriores. | Feedback da Entrega 1 indicou ambiguidade entre os dois conceitos. O TCC prevê formalmente o histórico durante a sessão, enquanto a recuperação entre sessões permanece associada a H15. | Entrega 1; R04; R05; T04 e T06, conforme a nomenclatura utilizada originalmente. | Equipe |
| 01/10/2026 | Foram corrigidos os encaminhamentos das hipóteses para as etapas da disciplina. | Feedback das Entregas 1 e 2 indicou que entrevistas haviam sido associadas incorretamente à Entrega 2 e avaliações à Entrega 7. | Entrega 1; seção 2 desta matriz. | Equipe |
| 01/10/2026 | Foram incorporados à rastreabilidade os aprendizados RC01–RC08 da Entrega 2. | Feedback da Entrega 2 solicitou relacionar as recomendações às tarefas e registros existentes, distinguindo padrão observado de benefício ainda hipotético. | Entrega 2; seções 3 e 4 desta matriz. | Equipe |
| 01/10/2026 | Os identificadores C01 e C02 passaram a ser qualificados pelo contexto da entrega. | Feedback da Entrega 2 apontou ambiguidade entre concorrentes C01/C02 e cenários C01/C02. | Entrega 2; Entrega 4; seção 3 desta matriz. | Equipe |
| 03/10/2026 | P02 — Mariana Costa passou de persona secundária para persona primária. | Feedback da Entrega 3 destacou que a compreensão de procedimentos já integra A02 e o núcleo do escopo do projeto, não sendo apenas uma necessidade periférica. | Entrega 3; seção 1 e relações com P02 nesta matriz. | Equipe |
| 03/10/2026 | P01 — Lucas Almeida passou a ser explicitamente relacionado ao tratamento de ausência de evidência. | A jornada revisada da Entrega 3 possui um desfecho no qual Lucas não obtém evidência suficiente e precisa recorrer a outro canal. | Entrega 3; R03; T05, conforme nomenclatura original; TI05, conforme nomenclatura revisada; RC04; seção 4 desta matriz. | Equipe |
| 03/10/2026 | O contexto físico, social e os resultados humanos das personas foram aprofundados. | Feedback da Entrega 3 solicitou situações mais específicas de uso e uma jornada que apresentasse o que ocorre antes, durante e depois da interação. | Entrega 3; R01, R03, R05, R06 e R07. | Equipe |
| 25/11/2026 | O questionário I01 foi implementado, publicado e validado funcionalmente. O instrumento I02 foi complementado com procedimentos, materiais e critérios de análise. | Feedback da Entrega 7 apontou a ausência de um formulário on-line respondível e a necessidade de detalhamento operacional do Card Sorting. A equipe optou por não realizar a coleta nesta etapa. | Entrega 7; I01; I02; H02, H04–H10, H12, H14–H16 e H18; seção 2 desta matriz. | Equipe |
| 25/11/2026 | Foram complementados os registros das hipóteses H02, H07, H11 e H12 na matriz. | Feedbacks das Entregas 7 e 8 e necessidade de estabelecer correspondência entre os instrumentos, hipóteses e decisões de interface. | Entregas 1, 7 e 8; seção 2 desta matriz. | Equipe |
| 25/11/2026 | Os princípios gerais foram separados em princípios direcionados ao negócio e princípios direcionados à interface. | Feedback da Entrega 8 solicitou a separação explícita entre as duas categorias de princípios. | Entrega 8; R01–R07; seção 3 desta matriz. | Equipe |
| 25/11/2026 | A priorização das metas foi reorganizada utilizando exclusivamente as cinco metas de usabilidade de Nielsen. | Feedback da Entrega 8 apontou que a distribuição de pesos entre MU01 e MU08 não atendia à orientação da disciplina. | Entrega 8; MU01–MU08; seção 3 desta matriz. | Equipe |
| 25/11/2026 | Foram detalhados os critérios operacionais de sucesso, ajuda, erros, compreensão e satisfação, além dos três níveis de Engenharia de Usabilidade de Mayhew. | Feedback da Entrega 8 solicitou metas verificáveis, definição dos participantes, limites observáveis e descrição das iterações. | Entrega 8; R01–R07; MU01–MU08; Entregas 12–14. | Equipe |
| 25/11/2026 | Foi definida a separação entre os identificadores dos modelos T01–T06 e as tarefas gerais de interação TI01–TI06. | Feedback recorrente das Entregas 5, 6 e 8 apontou colisões entre os identificadores utilizados em diferentes documentos. TI01–TI05 foram definidos na revisão da Entrega 8, e TI06 preserva a atividade de histórico da matriz anterior. | Entregas 5–14; matriz de rastreabilidade. A propagação da nomenclatura aos demais documentos permanece em andamento. | Equipe |
| 25/11/2026 | Foram incorporados os vínculos entre os requisitos e os modelos de tarefas, fluxos de prototipação, cenários de interação, signos, MoLIC e telas do Figma. | Feedbacks das Entregas 5 a 12 solicitaram a atualização das colunas de rastreabilidade que permaneciam pendentes, apesar da existência dos respectivos artefatos. | R01–R07; T01–T06; PF01–PF03; CI01/CI02; O01–O14; M01/M02; F01–F16. | Equipe |
| 25/11/2026 | Os achados HC01, HC02 e AU01–AU03 foram incorporados à matriz, relacionando problemas, requisitos e melhorias planejadas. | Evidências registradas nas Entregas 13 e 14, relacionadas à identificação das fontes, recuperação de falhas, clareza e autonomia durante a interação. | R01, R02, R03, R06 e R07; F01, F03, F04, F07, F08, F15 e F16. | Equipe |
| 25/11/2026 | Foram registradas as diferenças entre as tarefas planejadas na Entrega 12 e as tarefas efetivamente executadas na Entrega 14, preservando os significados originais das metas MU. | O DECIDE estabelece cinco tarefas, enquanto a avaliação observada foi realizada com quatro tarefas cujos identificadores e métricas apresentam diferenças em relação ao planejamento inicial. | Entregas 8, 12 e 14; QA; UT; MU01–MU08. Revisão documental complementar permanece prevista. | Equipe |

As revisões realizadas após os feedbacks preservam o histórico das decisões anteriores, distinguindo os artefatos já produzidos, as correções efetivamente realizadas e as melhorias ainda planejadas.

A numeração original dos requisitos R01 a R07 permanece como referência central do projeto.

As correções conceituais dos modelos da Entrega 5, o detalhamento das evidências da Entrega 6, os refinamentos do modelo conceitual e do MoLIC das Entregas 9 e 10, a consistência entre cenários e telas da Entrega 11 e o alinhamento entre planejamento e execução das Entregas 12 e 14 ainda deverão ser incorporados progressivamente aos respectivos documentos.

As melhorias associadas aos achados HC01, HC02 e AU01–AU03 permanecem planejadas até que as alterações correspondentes sejam efetivamente realizadas e verificadas.

## Como usar

- Use identificadores estáveis (`H01`, `P01`, `C01`, `T01`, `TI01`, `M01`, `F01`, `UT01`).
- Quando uma necessidade/problema tiver origem em hipótese da Entrega 1, cite o ID correspondente.
- Quando `C01` ou `C02` puder se referir a artefatos diferentes, qualifique o contexto, por exemplo: **concorrente C01 — Entrega 02** ou **cenário C01 — Entrega 04**.
- Os identificadores T01–T06 devem representar exclusivamente os modelos de análise de tarefas da Entrega 5.
- Os identificadores TI01–TI06 devem representar as tarefas gerais de interação do estudante.
- Os identificadores UT devem ser qualificados pela respectiva entrega enquanto houver diferenças entre as tarefas planejadas e executadas.
- Uma linha pode se desdobrar quando um objetivo possui múltiplos caminhos.
- Não force relação inexistente: se algo ainda não foi modelado, indique a ausência do artefato; use `PENDENTE` quando houver trabalho futuro claramente identificado.
- A presença de um padrão em concorrentes ou em proto-personas não confirma automaticamente sua necessidade para o público do projeto.
- A preparação e a validação funcional de instrumentos de coleta não representam confirmação empírica das hipóteses investigadas.
- A associação entre requisitos e artefatos não representa comprovação automática da qualidade da interação.
- Ao remover ou modificar uma funcionalidade, registre a decisão em vez de apagar silenciosamente o histórico.
- Dashboard, CRUD, filtros, relatórios e histórico entre sessões só devem aparecer quando houver objetivo/tarefa que os justifique.
- As metas de usabilidade devem ser avaliadas conforme suas definições originais, utilizando apenas evidências efetivamente registradas.
- Quando uma métrica não puder ser verificada com os dados disponíveis, registre-a como não avaliada ou inconclusiva.
