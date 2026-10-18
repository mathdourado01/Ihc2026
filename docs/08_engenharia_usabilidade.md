# Entrega 8 — Ciclo de vida e engenharia de usabilidade

**Data:** {{17/10/2026}}  
**Status:** 🟩 concluída 
**Responsabilidade:** 1 solução por equipe

## Objetivo da atividade

Transformar o conhecimento acumulado sobre usuários, tarefas, plataforma e contexto em princípios e **metas de usabilidade verificáveis**, mantendo o caráter iterativo do projeto.

## Delimitação do sistema interativo

Antes das características da plataforma, separe:

| Camada | O que pertence ao projeto | O que será avaliado em IHC |
|---|---|---|
| Contribuição técnica do TCC | Arquitetura de recuperação de informações institucionais, processamento de consultas e geração de respostas fundamentadas por Inteligência Artificial. | O desempenho técnico do modelo, incluindo a qualidade da recuperação e das respostas geradas, será avaliado no TCC e não será substituído pelos testes de IHC. |
| Camada de interação da disciplina | Interface conversacional na qual o estudante formula dúvidas, recebe e compreende respostas, consulta fontes institucionais, continua a conversa durante a sessão e reconhece situações de ausência de evidência. | Compreensão, eficácia, eficiência, satisfação, prevenção de erros e acessibilidade durante a realização das tarefas. |
| Integrações/dados simulados | Perguntas, respostas, fontes institucionais e estados de processamento previamente preparados para representar os cenários de interação quando a implementação técnica não estiver integrada ao protótipo. | Capacidade do estudante de compreender e utilizar a interface. A avaliação não medirá a qualidade técnica das respostas simuladas nem o desempenho real do processamento. |


Em um protótipo de disciplina, é aceitável simular processamento ou resultados quando a implementação técnica não estiver integrada, desde que isso seja declarado e a simulação seja suficiente para avaliar a interação.

## 1. Características da plataforma

| Característica | Descrição | Consequência para IHC |
|---|---|---|
| Software | Aplicação com interface conversacional, prevista para utilização por meio de navegador web. | A interface deverá apresentar navegação simples, permitindo iniciar consultas diretamente pelo campo de entrada de perguntas. |
| Hardware/dispositivos | Computadores, notebooks e dispositivos móveis compatíveis com navegadores atuais. | A organização visual deverá considerar diferentes tamanhos de tela, garantindo legibilidade e acesso aos elementos essenciais. |
| Capacidades | Receber perguntas em linguagem natural, apresentar respostas, disponibilizar fontes institucionais, preservar o contexto da conversa durante a sessão e comunicar quando não houver evidência suficiente. Essas capacidades permitem centralizar a consulta e apoiar a compreensão das informações pelo estudante. | As ações principais deverão ser facilmente identificáveis. Perguntas, respostas e fontes deverão possuir organização clara, permitindo ao estudante compreender e continuar a interação. |
| Restrições | O assistente depende da disponibilidade de informações institucionais e pode não encontrar evidência suficiente para responder a determinadas perguntas. Também não está prevista, no recorte atual, a execução de procedimentos administrativos ou a consulta a dados acadêmicos individuais. | A interface deverá comunicar suas limitações, evitar apresentar informações não confirmadas como definitivas e orientar o estudante sobre como prosseguir quando necessário. |
| Conectividade/latência | A solução pode depender da comunicação entre a interface, os componentes de recuperação documental e serviços externos de processamento. | Deverá existir feedback visual durante o processamento e comunicação compreensível em situações de falha ou indisponibilidade. |
| Segurança/privacidade | O estudante poderá inserir espontaneamente informações pessoais durante a formulação de perguntas, embora esses dados não sejam necessários para o objetivo principal da consulta. | A interface deverá evitar solicitar dados pessoais desnecessários e considerar a transparência sobre o tratamento e eventual armazenamento das informações. |
| Volume de dados/histórico | A sessão poderá conter múltiplas perguntas e respostas, preservando a continuidade da conversa atual. A recuperação de conversas entre sessões permanece como hipótese a investigar. | As mensagens deverão ser apresentadas em sequência organizada, permitindo localizar visualmente interações anteriores dentro da sessão. Busca e filtros entre sessões não serão considerados requisitos obrigatórios neste momento. |
| Tempo de processamento | O intervalo entre o envio da pergunta e a apresentação da resposta poderá variar conforme a recuperação das informações e o processamento realizado. | A interface deverá indicar que a pergunta foi recebida e está sendo processada, evitando que o estudante interprete a espera como ausência de resposta ou falha. |
| Papéis/permissões | O estudante da FEI é o usuário principal do recorte de IHC. Funções de administração técnica ou gerenciamento da base documental não fazem parte das tarefas selecionadas para avaliação. | A interface deverá priorizar as ações do estudante, sem acrescentar funcionalidades administrativas que não correspondam ao escopo definido. |

## 2. Princípios gerais do projeto

Inclua apenas normas, leis, padrões e princípios realmente relevantes, explicando **como** afetam o projeto. Não transforme esta seção em lista de links.

| Princípio/norma | Aplicabilidade ao contexto | Decisão/requisito decorrente | Fonte |
|---|---|---|---|
| Contexto de uso | O público principal é composto por estudantes da FEI que necessitam localizar ou compreender informações acadêmicas e administrativas. A interação poderá ocorrer dentro ou fora da instituição, por meio de computadores, notebooks ou dispositivos móveis. As características comportamentais ainda não investigadas permanecem como hipóteses. | Priorizar uma interface conversacional com campo de consulta evidente, respostas compreensíveis e possibilidade de continuidade durante a sessão, considerando os diferentes dispositivos previstos. | Entregas 1 e 3; cenários da Entrega 4. |
| Engenharia de Usabilidade de Mayhew | O projeto deve considerar conjuntamente perfil do usuário, análise das tarefas, características da plataforma e princípios gerais para estabelecer requisitos de usabilidade. | Definir metas qualitativas e quantitativas verificáveis e revisar a solução por meio de ciclos de prototipação e avaliação. | Barbosa e Silva (2010). Aulas CC8122 — Processos de Projeto de IHC, Partes 1 e 2. |
| ISO 9241-11:2018 | A usabilidade deve ser considerada em relação aos objetivos de usuários específicos, em determinado contexto de utilização. | Estabelecer medidas de eficácia, eficiência e satisfação associadas às tarefas realizadas pelos estudantes. | https://www.iso.org/standard/63500.html |
| LGPD — Lei nº 13.709/2018 | As consultas realizadas pelos estudantes podem conter informações pessoais inseridas espontaneamente durante a interação. | Evitar a solicitação de dados pessoais desnecessários e considerar transparência sobre eventual coleta, utilização e armazenamento das informações. | https://www.planalto.gov.br/ccivil_03/_ato2015-2018/2018/lei/l13709.htm |
| Acessibilidade — WCAG 2.2 | A interface web deverá considerar diferentes condições de acesso e necessidades dos estudantes. | Priorizar legibilidade, contraste adequado, identificação textual dos elementos interativos e possibilidade de navegação por teclado. | https://www.w3.org/TR/WCAG22/ |
| Heurísticas de Nielsen | A interface precisa apresentar seu estado de funcionamento, utilizar linguagem familiar, manter consistência e auxiliar na prevenção e recuperação de erros. | Apresentar feedback durante o processamento, utilizar vocabulário acadêmico-administrativo compreensível, manter padrões consistentes e comunicar claramente situações de falha ou ausência de evidência. | https://www.nngroup.com/articles/ten-usability-heuristics/ |

## 3. Metas de usabilidade

Usabilidade deve ser discutida **no contexto de uso**. Metas quantitativas devem dizer o que será medido, em qual tarefa, com qual população e qual limite será considerado aceitável.

### 3.1 Metas qualitativas

| Meta | Para quem/tarefa | Evidência desejada | Justificativa |
|---|---|---|---|
| Compreensão da interface e facilidade para iniciar uma consulta. | Estudantes da FEI — T01: Formular uma dúvida em linguagem natural. | O participante identifica como iniciar a consulta sem necessitar de explicações adicionais sobre os comandos da interface. | A formulação de perguntas representa a principal ação do sistema e deve ser facilmente compreendida. |
| Clareza e compreensão das respostas apresentadas. | Estudantes da FEI — T02: Ler e compreender a resposta. | O participante consegue explicar, com suas palavras, a informação apresentada pelo assistente. | O objetivo humano do projeto envolve compreender informações acadêmicas e administrativas, não apenas receber uma resposta textual. |
| Identificação da origem institucional das informações. | Estudantes da FEI — T03: Identificar e consultar a fonte institucional associada à resposta. | O participante reconhece onde a fonte está apresentada e consegue identificá-la sem dificuldades significativas. | A apresentação das fontes contribui para a transparência e permite verificar a origem das informações fornecidas. |
| Continuidade da interação durante a sessão. | Estudantes da FEI — T04: Fazer uma nova pergunta ou complementar uma pergunta anterior. | O participante compreende que pode complementar sua consulta sem precisar iniciar uma nova interação. | A manutenção do contexto durante a sessão já faz parte do escopo previsto no TCC. |
| Compreensão das limitações do assistente. | Estudantes da FEI — T05: Reconhecer a ausência de evidência suficiente. | O participante identifica que a informação solicitada não foi confirmada e compreende como prosseguir. | Evita que informações não confirmadas sejam interpretadas como orientações institucionais definitivas. |
| Visibilidade do estado do sistema. | Estudantes da FEI — fluxo entre T01 e T02. | O participante reconhece que sua pergunta foi recebida e está sendo processada. | A espera pelo processamento não deve gerar dúvidas sobre o funcionamento da interface. |


### 3.2 Metas quantitativas

| ID | Dimensão | Métrica | Tarefa/escopo | Meta | Como medir | Justificativa |
|---|---|---|---|---|---|---|
| MU01 | Eficácia | Taxa de conclusão sem ajuda. | T01 — Formular uma dúvida em linguagem natural. | ≥ 90% | Teste observado com estudantes da FEI, registrando quantos participantes conseguem formular e enviar uma pergunta sem orientação do avaliador. | A consulta representa a principal funcionalidade da interface e deve ser facilmente executada. |
| MU02 | Eficácia | Taxa de compreensão correta da resposta. | T02 — Ler e compreender a resposta. | ≥ 80% | Solicitar que cada participante explique a informação recebida e comparar sua interpretação com critérios de sucesso definidos previamente. | A resposta precisa apoiar a compreensão das informações acadêmicas e administrativas. |
| MU03 | Eficiência | Tempo mediano para localizar a fonte institucional. | T03 — Identificar e consultar a fonte. | ≤ 30 segundos | Cronometrar o intervalo entre a apresentação da tarefa e a identificação correta da fonte pelo participante. | A origem da informação deve ser facilmente identificável. |
| MU04 | Eficácia | Taxa de conclusão sem ajuda. | T04 — Complementar uma pergunta durante a sessão. | ≥ 80% | Observar quantos participantes conseguem formular uma pergunta complementar relacionada à interação anterior, sem orientação do avaliador. | A continuidade da conversa representa uma capacidade prevista no projeto. |
| MU05 | Prevenção de erros | Taxa de interpretação correta da ausência de evidência. | T05 — Reconhecer a limitação do assistente. | ≥ 90% | Apresentar uma situação sem evidência suficiente e verificar quantos participantes reconhecem a limitação e identificam como prosseguir. | Interpretações equivocadas podem comprometer a compreensão de regras e procedimentos acadêmicos. |
| MU06 | Eficiência | Tempo mediano para iniciar uma consulta. | T01 — Formular e enviar uma pergunta. | ≤ 60 segundos | Cronometrar o intervalo entre a apresentação da tarefa e o envio da pergunta, utilizando o mesmo cenário para os participantes. | A interface deve permitir iniciar uma consulta sem navegação desnecessária. |
| MU07 | Satisfação | Média da avaliação pós-tarefa em escala de 1 a 5. | T01–T05. | ≥ 4,0 em cada tarefa. | Aplicar uma pergunta padronizada de satisfação após cada tarefa, sendo 1 muito insatisfeito e 5 muito satisfeito. | Permite verificar a percepção dos estudantes sobre a experiência de interação. |

### 3.3 Priorização das metas (se exigida na disciplina)

Se o professor solicitar porcentagens que somem 100%, trate-as como **peso de prioridade**, não como métrica de usabilidade.

| Meta | Peso de prioridade | Justificativa |
|---|---:|---|
| MU01 — Conclusão da consulta | 15% | Representa a ação principal do estudante ao utilizar o assistente. |
| MU02 — Compreensão da resposta | 20% | Está diretamente relacionada ao objetivo humano de compreender informações acadêmicas e administrativas. |
| MU03 — Localização da fonte | 15% | Permite identificar a origem institucional das informações apresentadas. |
| MU04 — Continuidade da conversa | 10% | Apoia a complementação de dúvidas durante a mesma sessão. |
| MU05 — Compreensão da ausência de evidência | 20% | Possui relevância para a prevenção de interpretações equivocadas sobre informações institucionais. |
| MU06 — Tempo para iniciar a consulta | 5% | Contribui para a eficiência da principal ação da interface. |
| MU07 — Satisfação | 10% | Considera a percepção dos estudantes sobre a experiência de utilização. |
| MU08 — Reconhecimento do processamento | 5% | Contribui para a compreensão do estado do sistema durante a espera. |
| **Total** | **100%** | |

## 4. Como o ciclo será iterado

O desenvolvimento do projeto seguirá o modelo de Engenharia de Usabilidade de Mayhew, apresentado nas aulas, que propõe um processo iterativo dividido em três níveis: projeto essencial, padrões de telas e diálogos e projeto detalhado. A ideia é que a interface seja desenvolvida e avaliada gradualmente, permitindo realizar ajustes conforme os problemas identificados e os resultados obtidos.

No nosso projeto, esse processo será aplicado a partir dos artefatos produzidos nas entregas anteriores, como os cenários da Entrega 4, os modelos de tarefas da Entrega 5 e o protótipo em papel da Entrega 6. Esses materiais servirão como base para o desenvolvimento da interface e poderão ser revisitados sempre que forem identificadas dificuldades relacionadas à interação dos estudantes com o assistente virtual.

Nas próximas etapas, a equipe deverá aprimorar a organização das mensagens, a apresentação das fontes institucionais, os elementos visuais e os mecanismos de feedback. Posteriormente, as avaliações previstas nas Entregas 12, 13 e 14 permitirão identificar problemas de usabilidade e verificar se as metas estabelecidas nesta entrega estão sendo atingidas.

Por exemplo, caso os testes indiquem que os estudantes apresentam dificuldades para localizar as fontes institucionais, será necessário revisar a forma como essas informações são apresentadas na interface, considerando a tarefa T03 e a meta MU03. O mesmo processo será aplicado caso sejam identificadas dificuldades na compreensão das respostas, na continuidade da conversa ou no reconhecimento das limitações do assistente.

As melhorias realizadas deverão ser registradas na matriz de rastreabilidade, relacionando os problemas identificados às decisões tomadas pela equipe. Dessa forma, o desenvolvimento não ficará limitado à criação de um único protótipo, mas seguirá um processo contínuo de avaliação e aprimoramento, buscando adequar cada vez mais a interface às necessidades dos estudantes.

## Checklist

- [x] Capacidades e restrições têm impacto de IHC explicitado.
- [x] Está claro o limite entre contribuição técnica do TCC e camada interativa da disciplina.
- [x] Resultados/processamento simulados no protótipo foram explicitados.
- [x] Metas de usabilidade avaliam a interação, não substituem métricas técnicas do TCC.
- [x] Normas/princípios estão contextualizados, não apenas copiados.
- [x] Metas quantitativas são mensuráveis e associadas a tarefas/público.
- [x] Eficácia, eficiência e satisfação são consideradas quando pertinentes.
- [x] Metas poderão ser verificadas nas Entregas 12–14.
