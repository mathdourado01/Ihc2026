# Matriz de rastreabilidade de IHC

A matriz deve ser atualizada ao longo do semestre. Ela ajuda a demonstrar que a interface não surgiu arbitrariamente e registra **como o conhecimento da equipe evoluiu**.

Para projetos cujo TCC não previa interface, esta matriz é especialmente importante: deve ficar visível a passagem da **contribuição técnica do TCC** para um **cenário de uso plausível**, e desse cenário para as decisões de interação.

## 1. Derivação do escopo de IHC a partir do TCC

| Elemento | Registro da equipe | Evidência/justificativa | Estado |
|---|---|---|---|
| Tema do TCC | Assistente Virtual com Inteligência Artificial para Suporte a Dúvidas Acadêmicas e Administrativas na FEI | TCC e seção 0.2 da Entrega 1 | definido |
| Resultado técnico esperado | Desenvolvimento de um protótipo funcional de assistente virtual capaz de recuperar informações institucionais e gerar respostas em linguagem natural, acompanhado de avaliação experimental da arquitetura | TCC e seção 0.4 da Entrega 1 | definido |
| O TCC previa interface? | Sim | O TCC prevê formalmente uma interface na qual o usuário envia perguntas em linguagem natural e recebe respostas fundamentadas nas informações institucionais recuperadas pelo sistema | definido |
| Capacidade/contribuição central | Recuperar informações relevantes de uma base documental institucional e utilizá-las como evidência para gerar respostas em linguagem natural a dúvidas acadêmicas e administrativas | TCC e seção 1.3 da Entrega 1 | definido |
| Possíveis beneficiários/stakeholders | Estudantes da FEI; equipe responsável pelo desenvolvimento e avaliação do sistema; profissionais e setores da FEI responsáveis por processos e informações acadêmico-administrativas | Seções 2.1, 2.2 e 2.3 da Entrega 1 | F |
| Usuário escolhido para IHC | Estudante da FEI que necessita localizar ou compreender uma informação acadêmica ou administrativa | O estudante é o usuário direto previsto no TCC e realiza as atividades A01 e A02 definidas na Entrega 1 | F |
| Objetivo principal do usuário | Obter e compreender uma informação acadêmica ou administrativa para resolver uma dúvida, tomar uma decisão ou realizar corretamente um procedimento relacionado à sua vida acadêmica | H04, seção 3.1 e seção 7.3 da Entrega 1 | H |
| Contexto de uso adotado | Situações em que o estudante precisa esclarecer uma dúvida acadêmica ou administrativa, dentro ou fora da FEI, possivelmente por computador, notebook ou dispositivo móvel | H11 e H12, seção 5 da Entrega 1 | H |
| Interface/recorte de IHC | Fluxo conversacional de consulta no qual o estudante formula uma dúvida, recebe e compreende uma resposta, pode consultar a fonte institucional utilizada e é informado quando não existe evidência suficiente para responder | Seções 7.1 e 7.4 da Entrega 1; deriva das capacidades previstas no TCC e das atividades A01 e A02 | proposta |
| Relação com o TCC | parte prevista | A interface conversacional já faz parte do protótipo previsto no TCC. A disciplina de IHC aprofundará seus aspectos de interação e usabilidade | definido |

> Se o escopo de IHC mudar ao longo do semestre, preserve a decisão anterior no histórico e registre **qual evidência motivou a mudança**.

---

## 2. Registro de hipóteses e lacunas da Entrega 1

Use esta tabela para itens importantes marcados como `[H]` ou `[?]`. Preserve o histórico: não apague uma hipótese refutada.

| ID | Afirmação / dúvida inicial | Tipo | Por que importa | Como/onde investigar | Evidência obtida | Estado atual | Impacto no projeto |
|---|---|---|---|---|---|---|---|
| H04 | O estudante busca obter e compreender informações acadêmicas ou administrativas para resolver dúvidas, tomar decisões ou realizar corretamente procedimentos relacionados à vida acadêmica | H | Define o objetivo principal do usuário e orienta quais tarefas deverão ser priorizadas na interface | Entrega 2 — investigação com estudantes da FEI | PENDENTE | aberta | Pode confirmar ou exigir revisão do objetivo principal e das tarefas priorizadas |
| H05 | Localizar e compreender informações acadêmicas ou administrativas é uma das atividades mais frequentes dos estudantes nesse contexto | H | Ajuda a verificar se A01 deve ser considerada a atividade principal do projeto de IHC | Entrega 2 — entrevistas, questionários ou levantamento com estudantes | PENDENTE | aberta | Pode confirmar ou alterar a prioridade das atividades e tarefas da interface |
| H06 | Compreender e realizar procedimentos acadêmicos ou administrativos é uma atividade de maior criticidade quando envolve regras, etapas obrigatórias ou prazos | H | A criticidade pode exigir maior cuidado na apresentação das respostas, fontes, limitações e orientações | Entrega 2 — investigação com estudantes e, quando pertinente, setores responsáveis | PENDENTE | aberta | Pode influenciar o detalhamento das respostas e os mecanismos de prevenção e recuperação de erros |
| H08 | A distribuição das informações entre diferentes páginas, documentos e canais pode aumentar o esforço necessário para o estudante resolver uma dúvida | H | Representa um dos principais problemas que justificam o fluxo de consulta centralizado proposto para o assistente | Entrega 2 — investigação do processo atual com estudantes | PENDENTE | aberta | Se sustentada, reforça o fluxo centralizado de consulta; se refutada, pode exigir revisão da caracterização do problema |
| H14 | A confiabilidade percebida pelo estudante poderá ser influenciada pela clareza sobre a origem institucional das informações apresentadas | H | Pode justificar a apresentação das fontes e determinar como essas informações deverão aparecer na interface | Entrega 2 — investigação com usuários; Entrega 7 — avaliação da interface | PENDENTE | aberta | Pode influenciar a visibilidade, organização e detalhamento das fontes institucionais |
| H15 | Um histórico de conversas anteriores pode ser útil para o estudante retomar informações ou consultas realizadas anteriormente | H | O TCC prevê histórico de interação, mas ainda é necessário verificar se essa funcionalidade representa uma necessidade real do usuário | Entrega 2 — investigação com estudantes; Entrega 7 — teste de usabilidade | PENDENTE | aberta | Pode confirmar, modificar ou remover a funcionalidade de histórico da interface |
| H16 | Uma resposta incorreta ou uma interpretação equivocada sobre regras, prazos ou procedimentos pode produzir consequências relevantes para o estudante | H | Influencia diretamente o tratamento de erros, ausência de evidência, avisos e encaminhamento para canais oficiais | Entrega 2 — investigação com estudantes e setores responsáveis; Entrega 7 — avaliação da interação | PENDENTE | aberta | Pode justificar mensagens de cautela, tratamento explícito da ausência de evidência e encaminhamento para canais oficiais |
| H18 | O padrão de interação utilizado por assistentes como ChatGPT, Gemini e Copilot pode ser familiar aos estudantes da FEI | H | Pode sustentar ou questionar a escolha de uma interface conversacional como principal forma de interação | Entrega 2 — investigação com estudantes e análise de interfaces existentes | PENDENTE | aberta | Pode confirmar o padrão conversacional ou indicar necessidade de adaptação do fluxo de interação |

---

## 3. Rastreabilidade entre contribuição técnica, necessidades e artefatos

| ID | Capacidade do TCC utilizada | Necessidade/problema | Persona | Cenário problema | Objetivo/tarefa | HTA/GOMS/CTT | Cenário de interação / signos | MoLIC | Tela(s) Figma | Heurística / problema | Tarefa no teste | Decisão/melhoria |
|---|---|---|---|---|---|---|---|---|---|---|---|---|
| R01 | Receber uma pergunta em linguagem natural, recuperar informações institucionais relevantes e gerar uma resposta fundamentada | H04, H05 e H08 — necessidade de localizar e compreender informações e possível esforço causado pela distribuição das informações entre diferentes fontes | PENDENTE | PENDENTE | T01 — Formular uma dúvida em linguagem natural; T02 — Ler e compreender a resposta | PENDENTE | PENDENTE | PENDENTE | PENDENTE | PENDENTE | PENDENTE | PENDENTE |
| R02 | Preservar os metadados dos documentos e disponibilizar a origem das informações utilizadas na resposta | H14 — a clareza sobre a origem institucional das informações pode influenciar a confiabilidade percebida | PENDENTE | PENDENTE | T03 — Identificar e consultar a fonte institucional associada à resposta | PENDENTE | PENDENTE | PENDENTE | PENDENTE | PENDENTE | PENDENTE | PENDENTE |
| R03 | Reconhecer quando não existe evidência documental suficiente e evitar gerar respostas sem fundamento institucional | H06 e H16 — erros ou interpretações incorretas podem produzir consequências relevantes em consultas sobre regras, prazos e procedimentos | PENDENTE | PENDENTE | T05 — Compreender quando o assistente não possui evidência suficiente e identificar como prosseguir | PENDENTE | PENDENTE | PENDENTE | PENDENTE | PENDENTE | PENDENTE | PENDENTE |
| R04 | Manter o histórico das interações durante a sessão | H15 — histórico de conversas pode ser útil para retomar informações ou consultas anteriores | PENDENTE | PENDENTE | T06 — Consultar perguntas e respostas anteriores | PENDENTE | PENDENTE | PENDENTE | PENDENTE | PENDENTE | PENDENTE | PENDENTE |
| R05 | Manter uma interação conversacional que permita continuidade da consulta | H04 e H18 — o estudante pode precisar complementar uma dúvida e o padrão conversacional pode ser familiar ao público | PENDENTE | PENDENTE | T04 — Fazer uma nova pergunta ou complementar uma pergunta anterior | PENDENTE | PENDENTE | PENDENTE | PENDENTE | PENDENTE | PENDENTE | PENDENTE |

> Os campos relacionados a persona, cenário, modelos de tarefas, signos, MoLIC, Figma, avaliação heurística e testes permanecerão como `PENDENTE` até que esses artefatos sejam produzidos nas próximas entregas.

---

## 4. Rastreabilidade de padrões de interface

Use esta tabela quando o projeto incorporar padrões como dashboard, relatório, histórico, filtros ou administração. O objetivo é **justificar o padrão**, não apenas listar telas.

| ID da tela/fluxo | Padrão de interface | Objetivo/tarefa que justifica | Informação/ação principal | Evidência de necessidade | Artefatos relacionados |
|---|---|---|---|---|---|
| PENDENTE | Interface conversacional | T01, T02 e T04 | Formular uma pergunta em linguagem natural, visualizar e compreender a resposta e continuar a interação quando necessário | Interface prevista no TCC; H04 e H18 | R01, R05 |
| PENDENTE | Apresentação de fontes/evidências | T03 | Identificar a origem institucional da informação utilizada para fundamentar a resposta | Preservação das fontes prevista no TCC; H14 | R02 |
| PENDENTE | Tratamento de ausência de evidência e mensagens de limitação | T05 | Informar de forma clara quando o assistente não possui informação suficiente para responder e orientar o estudante sobre como prosseguir | Tratamento de ausência de evidência previsto no TCC; H06 e H16 | R03 |
| PENDENTE | Histórico de conversa | T06 | Consultar perguntas e respostas realizadas anteriormente durante a interação | H15 | R04 |

> Os identificadores `F01`, `F02` etc. serão definidos quando as telas ou fluxos correspondentes forem efetivamente modelados e prototipados. Neste momento, permanecem como `PENDENTE`.

> Possibilidades levantadas na Entrega 1, como indicador de processamento e ajuda/documentação, ainda não foram incorporadas como padrões definitivos porque permanecem como possibilidades a serem investigadas.

---

## 5. Registro de mudanças de escopo

| Data | O que mudou | Evidência/feedback que motivou | Artefatos afetados | Responsável |
|---|---|---|---|---|
| {{...}} | {{...}} | {{...}} | {{...}} | {{...}} |

## Como usar

- Use identificadores estáveis (`H01`, `P01`, `C01`, `T01`, `M01`, `F01`, `UT01`).
- Quando uma necessidade/problema tiver origem em hipótese da Entrega 1, cite o ID correspondente.
- Em TCC sem interface original, pelo menos uma linha deve mostrar claramente **como uma capacidade técnica chega até uma tarefa de usuário e uma tela/fluxo**.
- Uma linha pode se desdobrar quando um objetivo possui múltiplos caminhos.
- Não force relação inexistente: se algo ainda não foi modelado, marque `PENDENTE`.
- Ao remover uma funcionalidade, registre a decisão em vez de apagar silenciosamente o histórico.
- Dashboard, CRUD, filtros e relatórios só devem aparecer quando houver objetivo/tarefa que os justifique.
