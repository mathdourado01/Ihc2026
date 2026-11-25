# Entrega 8 — Ciclo de vida e engenharia de usabilidade

**Data:** 17/10/2026  
**Status:** 🟩 concluída  
**Responsabilidade:** 1 solução por equipe  
**Revisão após feedback:** 25/11/2026

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
| Hardware/dispositivos | Computadores, notebooks e dispositivos móveis compatíveis com navegadores atuais. Como referência de projeto, serão consideradas larguras de tela de 360 pixels para dispositivos móveis e 1280 pixels para computadores. | A organização visual deverá considerar diferentes tamanhos de tela, garantindo legibilidade e acesso aos elementos essenciais, sem exigir rolagem horizontal para formular perguntas ou consultar respostas. |
| Capacidades | Receber perguntas em linguagem natural, apresentar respostas, disponibilizar fontes institucionais, preservar o contexto da conversa durante a sessão e comunicar quando não houver evidência suficiente. Essas capacidades permitem centralizar a consulta e apoiar a compreensão das informações pelo estudante. | As ações principais deverão ser facilmente identificáveis. Perguntas, respostas e fontes deverão possuir organização clara, permitindo ao estudante compreender e continuar a interação. |
| Restrições | O assistente depende da disponibilidade de informações institucionais e pode não encontrar evidência suficiente para responder a determinadas perguntas. Também não está prevista, no recorte atual, a execução de procedimentos administrativos ou a consulta a dados acadêmicos individuais. | A interface deverá comunicar suas limitações, evitar apresentar informações não confirmadas como definitivas e orientar o estudante sobre como prosseguir quando necessário. |
| Conectividade/latência | A solução pode depender da comunicação entre a interface, os componentes de recuperação documental e serviços externos de processamento. | Em situações de falha ou perda de conexão, a interface deverá apresentar uma mensagem compreensível, preservar a pergunta quando tecnicamente possível e oferecer uma alternativa para tentar novamente. |
| Segurança/privacidade | O estudante poderá inserir espontaneamente informações pessoais durante a formulação de perguntas, embora esses dados não sejam necessários para o objetivo principal da consulta. | A interface deverá evitar solicitar dados pessoais desnecessários e considerar a transparência sobre o tratamento e eventual armazenamento das informações. |
| Volume de dados/histórico | A sessão poderá conter múltiplas perguntas e respostas, preservando a continuidade da conversa atual. A recuperação de conversas entre sessões permanece como hipótese a investigar. | As mensagens deverão ser apresentadas em sequência organizada, permitindo localizar visualmente interações anteriores dentro da sessão. Busca e filtros entre sessões não serão considerados requisitos obrigatórios neste momento. |
| Tempo de processamento | O intervalo entre o envio da pergunta e a apresentação da resposta poderá variar conforme a recuperação das informações e o processamento realizado. | A interface deverá apresentar feedback visual imediatamente após o envio da pergunta, adotando como referência de projeto um intervalo de até 1 segundo para indicar o início do processamento. Esse limite refere-se ao feedback da interface, não ao tempo de geração da resposta. |
| Papéis/permissões | O estudante da FEI é o usuário principal do recorte de IHC. Funções de administração técnica ou gerenciamento da base documental não fazem parte das tarefas selecionadas para avaliação. | A interface deverá priorizar as ações do estudante, sem acrescentar funcionalidades administrativas que não correspondam ao escopo definido. |
| Extensão das respostas | Algumas consultas poderão resultar em respostas extensas, contendo requisitos, etapas, documentos e orientações acadêmicas. | As respostas deverão utilizar parágrafos, listas ou etapas identificáveis quando necessário, mantendo as informações principais e as fontes acessíveis. |
| Disponibilidade das fontes | Documentos e páginas institucionais poderão sofrer alterações, apresentar restrições de acesso ou ficar temporariamente indisponíveis. | As fontes deverão ser identificadas por título, órgão responsável, endereço de consulta e data ou vigência, quando disponíveis. Caso uma fonte não possa ser acessada, a interface deverá comunicar essa limitação e apresentar alternativas de confirmação quando aplicáveis. |

Os limites apresentados constituem referências de projeto e critérios observáveis para orientar a prototipação e a avaliação da interface. Não representam resultados de medições realizadas nem requisitos técnicos já comprovados na implementação do TCC.

A avaliação da responsividade, da conectividade real e do comportamento temporal da aplicação dependerá de um protótipo ou implementação que permita observar essas características. No Figma, tais situações poderão ser representadas por estados simulados.

## 2. Princípios gerais do projeto

Inclua apenas normas, leis, padrões e princípios realmente relevantes, explicando **como** afetam o projeto. Não transforme esta seção em lista de links.

### 2.1 Princípios direcionados ao negócio

Os princípios direcionados ao negócio representam as características do domínio acadêmico-administrativo, as necessidades institucionais e as responsabilidades relacionadas à disponibilização de informações aos estudantes.

| Princípio/norma | Aplicabilidade ao contexto | Decisão/requisito decorrente | Fonte |
|---|---|---|---|
| Contexto de uso | O público principal é composto por estudantes da FEI que necessitam localizar ou compreender informações acadêmicas e administrativas. A interação poderá ocorrer dentro ou fora da instituição, por meio de computadores, notebooks ou dispositivos móveis. As características comportamentais ainda não investigadas permanecem como hipóteses. | Priorizar as necessidades acadêmicas e administrativas dos estudantes, considerando seus objetivos, contexto de utilização e diferentes níveis de experiência com os serviços institucionais. | Entregas 1 e 3; cenários da Entrega 4. |
| LGPD — Lei nº 13.709/2018 | As consultas realizadas pelos estudantes podem conter informações pessoais inseridas espontaneamente durante a interação. | Evitar a solicitação de dados pessoais desnecessários e considerar transparência sobre eventual coleta, utilização e armazenamento das informações. | https://www.planalto.gov.br/ccivil_03/_ato2015-2018/2018/lei/l13709.htm |
| Utilização de fontes institucionais | As orientações acadêmicas e administrativas precisam considerar informações disponibilizadas pelos canais oficiais da instituição. | Priorizar documentos e páginas institucionais, permitindo que o estudante identifique a origem das informações e consulte as evidências utilizadas quando disponíveis. | Escopo do TCC; Entregas 1, 2 e 4. |
| Tratamento responsável de informações críticas | Informações relacionadas a matrícula, prazos, requisitos, documentos e procedimentos acadêmicos podem gerar consequências para o estudante quando interpretadas incorretamente. | Apresentar fontes, data ou vigência quando disponíveis e comunicar explicitamente eventuais limitações da informação. Evitar conclusões definitivas quando não houver evidência suficiente ou quando a aplicação de uma regra depender da situação individual do estudante. | Cenários da Entrega 4; riscos identificados nas entregas anteriores. |
| Encaminhamento institucional | Determinadas dúvidas poderão exigir confirmação por um setor responsável da FEI ou depender de informações acadêmicas individuais não acessíveis ao assistente. | Informar os limites da orientação e indicar um canal institucional pertinente, quando identificado, sem afirmar que o procedimento foi executado ou que a situação individual foi analisada. | Delimitação do TCC; cenários e requisitos do projeto. |

### 2.2 Princípios direcionados à interface

Os princípios direcionados à interface orientam a organização das informações, os elementos de interação, a comunicação do sistema e a avaliação da experiência dos estudantes.

| Princípio/norma | Aplicabilidade ao contexto | Decisão/requisito decorrente | Fonte |
|---|---|---|---|
| Engenharia de Usabilidade de Mayhew | O projeto deve considerar conjuntamente perfil do usuário, análise das tarefas, características da plataforma e princípios gerais para estabelecer requisitos de usabilidade. | Definir metas qualitativas e quantitativas verificáveis e revisar a solução por meio de ciclos de prototipação e avaliação. | Barbosa e Silva (2010). Aulas CC8122 — Processos de Projeto de IHC, Partes 1 e 2. |
| ISO 9241-11:2018 | A usabilidade deve ser considerada em relação aos objetivos de usuários específicos, em determinado contexto de utilização. | Estabelecer medidas de eficácia, eficiência e satisfação associadas às tarefas realizadas pelos estudantes. | https://www.iso.org/standard/63500.html |
| Acessibilidade — WCAG 2.2 | A interface web deverá considerar diferentes condições de acesso e necessidades dos estudantes. | Priorizar legibilidade, contraste adequado, identificação textual dos elementos interativos e possibilidade de navegação por teclado. Como referência, considerar contraste mínimo de 4,5:1 para textos comuns, conforme os critérios aplicáveis de nível AA. | https://www.w3.org/TR/WCAG22/ |
| Heurísticas de Nielsen | A interface precisa apresentar seu estado de funcionamento, utilizar linguagem familiar, manter consistência e auxiliar na prevenção e recuperação de erros. | Apresentar feedback durante o processamento, utilizar vocabulário acadêmico-administrativo compreensível, manter padrões consistentes e comunicar claramente situações de falha ou ausência de evidência. | https://www.nngroup.com/articles/ten-usability-heuristics/ |
| Metas de usabilidade de Nielsen | A interface deverá ser compreensível para novos usuários, eficiente durante a utilização, fácil de recordar, resistente a erros e satisfatória. | Priorizar e avaliar as cinco metas de usabilidade de Nielsen, relacionando-as aos indicadores específicos definidos neste projeto. | Aulas CC8122; https://www.nngroup.com/articles/usability-101-introduction-to-usability/ |
| Padrões de interação conversacional | A formulação de perguntas em linguagem natural representa a principal forma de interação prevista no projeto. | Priorizar um campo de consulta evidente, respostas organizadas, continuidade durante a sessão e ações compreensíveis para reformular ou complementar uma pergunta. | Análise de concorrentes da Entrega 2; cenários da Entrega 4; prototipação da Entrega 6. |
| Apresentação compreensível das fontes | Os estudantes precisam identificar quais informações institucionais sustentam uma orientação recebida. | Apresentar fontes com identificação compreensível, órgão responsável, data ou vigência quando disponíveis e caminho para consulta. Evitar expor parâmetros técnicos do modelo de recuperação e geração no fluxo principal do estudante. | Cenários da Entrega 4; prototipação e refinamentos da Entrega 6. |
| Feedback e prevenção de erros | O estudante precisa distinguir os estados de consulta, processamento, resposta, ausência de evidência e falha. | Utilizar mensagens claras, consistentes e acompanhadas de alternativas de recuperação. Não depender exclusivamente de cores para comunicar estados importantes. | Heurísticas de Nielsen; WCAG 2.2; análise de tarefas da Entrega 5. |

A separação entre os princípios permite distinguir as responsabilidades relacionadas ao domínio institucional das decisões específicas de organização, comunicação e interação da interface.

## 3. Metas de usabilidade

Usabilidade deve ser discutida **no contexto de uso**. Metas quantitativas devem dizer o que será medido, em qual tarefa, com qual população e qual limite será considerado aceitável.

Para evitar ambiguidades entre as tarefas gerais de interação e os identificadores dos modelos HTA, GOMS e CTT da Entrega 5, serão utilizados os identificadores TI01 a TI05 nesta entrega.

| Identificador | Tarefa de interação | Identificador utilizado originalmente nesta entrega |
|---|---|---|
| TI01 | Formular e enviar uma dúvida em linguagem natural. | T01 |
| TI02 | Ler e compreender a resposta apresentada. | T02 |
| TI03 | Identificar e consultar a fonte institucional associada à resposta. | T03 |
| TI04 | Formular uma pergunta complementar durante a mesma sessão. | T04 |
| TI05 | Reconhecer a ausência de evidência suficiente e identificar como prosseguir. | T05 |

Os identificadores TI01 a TI05 representam ações gerais de interação avaliadas pelas metas de usabilidade. Os identificadores T01 a T06 da Entrega 5 permanecem associados aos respectivos modelos HTA, GOMS e CTT.

Essa distinção deverá ser incorporada à matriz de rastreabilidade e aos demais documentos que fazem referência às tarefas de interação, preservando os significados originais das metas MU01 a MU08.

### 3.1 Metas qualitativas

| Meta | Para quem/tarefa | Evidência desejada | Justificativa |
|---|---|---|---|
| Compreensão da interface e facilidade para iniciar uma consulta. | Estudantes da FEI — TI01: Formular uma dúvida em linguagem natural. | O participante identifica o campo de entrada, formula uma pergunta pertinente ao cenário e realiza o envio sem necessitar de orientação sobre os comandos da interface. | A formulação de perguntas representa a principal ação do sistema e deve ser facilmente compreendida. |
| Clareza e compreensão das respostas apresentadas. | Estudantes da FEI — TI02: Ler e compreender a resposta. | O participante consegue explicar, com suas próprias palavras, a orientação principal, os requisitos ou etapas relevantes e as eventuais limitações apresentadas. Os elementos essenciais esperados deverão ser definidos previamente para cada cenário de avaliação. | O objetivo humano do projeto envolve compreender informações acadêmicas e administrativas, não apenas receber uma resposta textual. |
| Identificação da origem institucional das informações. | Estudantes da FEI — TI03: Identificar e consultar a fonte institucional associada à resposta. | O participante localiza a fonte, identifica o documento ou canal institucional apresentado e compreende que ele sustenta a orientação recebida. Quando houver ação de consulta disponível, consegue identificá-la. | A apresentação das fontes contribui para a transparência e permite verificar a origem das informações fornecidas. |
| Continuidade da interação durante a sessão. | Estudantes da FEI — TI04: Fazer uma pergunta complementar. | O participante identifica como complementar a consulta anterior, formula uma pergunta relacionada ao contexto apresentado e reconhece a continuidade da conversa sem precisar iniciar uma nova sessão. | A manutenção do contexto durante a sessão já faz parte do escopo previsto no TCC. |
| Compreensão das limitações do assistente. | Estudantes da FEI — TI05: Reconhecer a ausência de evidência suficiente. | O participante identifica que a informação solicitada não foi confirmada, não interpreta a mensagem como uma orientação institucional definitiva e consegue indicar uma alternativa adequada, como reformular a pergunta ou consultar o canal responsável. | Evita que informações não confirmadas sejam interpretadas como orientações institucionais definitivas. |
| Visibilidade do estado do sistema — MU08. | Estudantes da FEI — fluxo entre TI01 e TI02. | O participante reconhece que sua pergunta foi recebida, identifica que o sistema está buscando informações e não realiza um novo envio motivado pela interpretação equivocada do estado de processamento. | A espera pelo processamento não deve gerar dúvidas sobre o funcionamento da interface. |

Os critérios de compreensão deverão considerar os conteúdos previamente preparados para cada cenário do protótipo. A avaliação verificará a interpretação da informação apresentada, e não a capacidade do modelo de inteligência artificial de produzir respostas tecnicamente corretas.

A meta MU08 possui caráter qualitativo e observacional. Não será atribuído um limite percentual artificial sem evidências suficientes para justificar esse valor.

### 3.2 Metas quantitativas

As metas quantitativas serão avaliadas com estudantes de graduação da FEI, pertencentes ao público-alvo do Assistente Virtual Acadêmico.

Para a avaliação exploratória prevista na disciplina, será considerada uma amostra mínima planejada de dois participantes, preferencialmente com diferentes experiências acadêmicas, que não tenham participado da elaboração do protótipo.

A quantidade de dois participantes corresponde ao recorte acadêmico da avaliação e não constitui uma amostra estatisticamente representativa dos estudantes da instituição.

| ID | Dimensão | Métrica | Tarefa/escopo | Meta | Como medir | Justificativa |
|---|---|---|---|---|---|---|
| MU01 | Eficácia | Taxa de conclusão sem ajuda. | TI01 — Formular uma dúvida em linguagem natural. | ≥ 90% | Teste observado com pelo menos dois estudantes da FEI, registrando quantos participantes conseguem formular e enviar uma pergunta pertinente ao cenário sem orientação do avaliador sobre a execução da tarefa. | A consulta representa a principal funcionalidade da interface e deve ser facilmente executada. |
| MU02 | Eficácia | Taxa de compreensão correta da resposta. | TI02 — Ler e compreender a resposta. | ≥ 80% | Solicitar que cada participante explique a informação recebida e comparar sua interpretação com os elementos essenciais definidos previamente para a resposta simulada. | A resposta precisa apoiar a compreensão das informações acadêmicas e administrativas. |
| MU03 | Eficiência | Tempo mediano para localizar a fonte institucional. | TI03 — Identificar e consultar a fonte. | ≤ 30 segundos | Cronometrar o intervalo entre a apresentação da tarefa de localização e a identificação correta da fonte pelo participante, utilizando o mesmo estado inicial para todos. | A origem da informação deve ser facilmente identificável, sem exigir navegação extensa ou busca em elementos secundários. |
| MU04 | Eficácia | Taxa de conclusão sem ajuda. | TI04 — Complementar uma pergunta durante a sessão. | ≥ 80% | Observar quantos participantes conseguem formular e enviar uma pergunta complementar relacionada à interação anterior, sem orientação do avaliador sobre o caminho a seguir. | A continuidade da conversa representa uma capacidade prevista no projeto. |
| MU05 | Prevenção de erros | Taxa de interpretação correta da ausência de evidência. | TI05 — Reconhecer a limitação do assistente. | ≥ 90% | Apresentar uma situação sem evidência suficiente e verificar quantos participantes reconhecem a limitação, não interpretam a informação como confirmada e identificam uma alternativa adequada para prosseguir. | Interpretações equivocadas podem comprometer a compreensão de regras e procedimentos acadêmicos. |
| MU06 | Eficiência | Tempo mediano para iniciar uma consulta. | TI01 — Formular e enviar uma pergunta. | ≤ 60 segundos | Cronometrar o intervalo entre a apresentação da tarefa e o envio da pergunta, utilizando o mesmo cenário e estado inicial para os participantes. | A interface deve permitir iniciar uma consulta sem navegação desnecessária. |
| MU07 | Satisfação | Média da avaliação pós-tarefa em escala de 1 a 5. | TI01–TI05. | ≥ 4,0 em cada tarefa. | Aplicar a mesma pergunta padronizada de satisfação após cada tarefa avaliada, sendo 1 muito insatisfeito e 5 muito satisfeito. | Permite verificar a percepção dos estudantes sobre a experiência de interação. |

A meta MU08, relacionada ao reconhecimento do processamento, permanece definida na seção 3.1 como indicador qualitativo de visibilidade do estado do sistema.

#### Critérios padronizados de avaliação

Para garantir consistência entre os participantes, serão utilizados os seguintes critérios:

| Indicador | Definição operacional |
|---|---|
| Conclusão sem ajuda | O participante atinge o objetivo da tarefa sem receber instruções sobre qual ação realizar, onde clicar ou qual resposta selecionar. |
| Conclusão com ajuda | O participante atinge o objetivo da tarefa após receber uma orientação necessária para prosseguir. |
| Conclusão parcial | O participante realiza parte das ações esperadas, mas não atinge integralmente o objetivo ou não demonstra compreender um elemento essencial da tarefa. |
| Falha | O participante não consegue atingir o objetivo, abandona a tarefa ou apresenta uma interpretação incompatível com os critérios de sucesso estabelecidos. |
| Erro | Ação ou interpretação que não contribui para o objetivo da tarefa e provoca desvio, recuperação, repetição desnecessária ou compreensão incorreta da informação. |
| Pedido de ajuda | Solicitação de orientação ao avaliador durante a realização da tarefa. Os pedidos deverão ser registrados independentemente de o avaliador fornecer ou não instruções. |
| Ajuda efetivamente fornecida | Intervenção do avaliador que fornece informação sobre a ação ou o caminho necessário para completar a tarefa. |
| Compreensão correta | Interpretação compatível com os elementos essenciais previamente definidos para o cenário e para a resposta apresentada. |
| Tempo de execução | Intervalo entre o início e o término definidos para cada métrica, registrado de forma individual e consistente. |
| Satisfação | Percepção declarada pelo participante após a realização da tarefa, utilizando a mesma escala e o mesmo enunciado. |

Esclarecimentos neutros sobre o enunciado da atividade, que não revelem o caminho de interação, deverão ser registrados separadamente das intervenções que ensinam ou direcionam a execução da tarefa.

A identificação de erros, pedidos de ajuda e ajuda efetivamente fornecida deverá ser realizada separadamente, evitando interpretar automaticamente qualquer dúvida do participante como falha de execução.

Para MU07, será utilizada a seguinte pergunta após cada tarefa:

> Considerando sua experiência ao realizar esta tarefa, qual é o seu nível de satisfação?

| Valor | Interpretação |
|---|---|
| 1 | Muito insatisfeito. |
| 2 | Insatisfeito. |
| 3 | Neutro. |
| 4 | Satisfeito. |
| 5 | Muito satisfeito. |

#### Interpretação das metas e limitações da amostra

Os valores estabelecidos para as metas MU01 a MU07 representam hipóteses de qualidade da interação e referências para orientar o projeto. Não constituem resultados previamente alcançados.

O limite de 30 segundos para localização da fonte foi definido considerando que a identificação da origem institucional deverá ocorrer diretamente na área da resposta ou por meio de uma ação claramente identificável.

O limite de 60 segundos para iniciar uma consulta considera que a interação principal deverá ser realizada diretamente pelo campo de entrada de perguntas, sem exigir navegação por menus ou preenchimento de formulários adicionais.

Esses limites deverão ser examinados a partir do fluxo efetivo da interface e de testes piloto, podendo ser refinados em iterações posteriores mediante justificativa e registro da alteração. As metas originais deverão permanecer identificáveis no histórico do projeto.

Considerando uma avaliação com dois participantes:

- As taxas de sucesso deverão ser apresentadas acompanhadas dos valores absolutos, como 2/2 ou 1/2 participantes.
- As metas de 80% e 90% exigem, nessa amostra, o sucesso dos dois participantes para que o limite seja alcançado numericamente.
- O alcance desses limites não representa confirmação estatística da qualidade da interface para todos os estudantes da FEI.
- Cada dificuldade identificada deverá ser analisada qualitativamente, considerando erros, pedidos de ajuda, intervenções e características da tarefa.
- Os tempos deverão ser apresentados individualmente e resumidos pela mediana, conforme previsto nas métricas.
- Quando uma tarefa não for realizada ou uma informação necessária não for registrada, a respectiva métrica deverá ser classificada como não avaliada ou inconclusiva.
- O tempo total de uma atividade não deverá substituir o tempo de uma ação específica, como localizar uma fonte ou enviar uma pergunta, quando esses intervalos não tiverem sido registrados separadamente.
- A facilidade de memorização não poderá ser considerada validada sem uma avaliação que permita observar o retorno do participante à interface após um intervalo sem utilização.

### 3.3 Priorização das metas (se exigida na disciplina)

Se o professor solicitar porcentagens que somem 100%, trate-as como **peso de prioridade**, não como métrica de usabilidade.

A priorização será realizada considerando exclusivamente as cinco metas de usabilidade de Nielsen: facilidade de aprendizado, facilidade de memorização, eficiência, baixa taxa de erro e satisfação positiva do usuário.

Os indicadores MU01 a MU08 representam metas específicas e instrumentos de verificação relacionados a essas cinco categorias, não constituindo categorias independentes de priorização.

| Meta | Peso de prioridade | Justificativa |
|---|---:|---|
| Facilidade de aprendizado | 25% | O assistente deverá permitir que estudantes, inclusive aqueles que nunca utilizaram a ferramenta, compreendam rapidamente como formular perguntas, interpretar respostas, consultar fontes e continuar a conversa. |
| Facilidade de memorização | 10% | Como as consultas acadêmicas poderão ocorrer de maneira eventual, é importante que o estudante consiga retornar à interface após um período sem utilização e reconhecer novamente suas principais ações. |
| Eficiência | 20% | O assistente deverá permitir localizar informações institucionais e iniciar consultas sem exigir navegação desnecessária por diferentes páginas, sistemas ou documentos. |
| Baixa taxa de erro | 30% | Informações acadêmicas incorretamente interpretadas podem ocasionar consequências relacionadas a prazos, matrícula, requisitos e procedimentos institucionais. A prevenção de erros, a compreensão das respostas e o reconhecimento das limitações do assistente possuem prioridade elevada. |
| Satisfação positiva do usuário | 15% | A experiência de utilização deverá ser percebida como compreensível, útil e satisfatória, contribuindo para a aceitação da solução pelos estudantes. |
| **Total** | **100%** | |

A maior prioridade foi atribuída à baixa taxa de erro devido às possíveis consequências acadêmicas de interpretações incorretas ou da utilização de informações não confirmadas.

A facilidade de aprendizado também recebeu prioridade elevada por se tratar de uma interface que deverá atender estudantes com diferentes níveis de familiaridade com sistemas conversacionais.

A eficiência recebeu peso relevante por estar diretamente relacionada à proposta de facilitar a busca por informações institucionais. A satisfação considera a percepção do estudante durante a utilização.

A facilidade de memorização permanece importante, embora receba menor peso relativo diante dos riscos associados à compreensão incorreta das orientações acadêmicas.

**Relação entre as metas de Nielsen e os indicadores do projeto:**

| Meta de Nielsen | Indicadores associados | Forma de avaliação |
|---|---|---|
| Facilidade de aprendizado | MU01, MU02, MU04 e MU08. | Observar a capacidade de iniciar consultas, compreender respostas, complementar perguntas e reconhecer o estado de processamento sem instruções desnecessárias. |
| Facilidade de memorização | MU01, MU04 e MU06, em eventual avaliação repetida. | Solicitar que o participante retorne à interface após um intervalo sem utilização e verificar se consegue reconhecer e executar as ações previamente realizadas. |
| Eficiência | MU03 e MU06. | Medir o tempo necessário para localizar fontes institucionais e iniciar uma consulta. |
| Baixa taxa de erro | MU02, MU05 e MU08. Registro complementar de erros e pedidos de ajuda. | Verificar a compreensão das informações, o reconhecimento da ausência de evidência, a interpretação do processamento e a ocorrência de ações ou decisões incorretas. |
| Satisfação positiva do usuário | MU07. | Aplicar a pergunta padronizada de satisfação após cada tarefa avaliada. |

Um mesmo indicador poderá contribuir para mais de uma meta de Nielsen, pois determinadas características da interação podem afetar simultaneamente aprendizado, eficiência e prevenção de erros.

Os pesos representam decisões de prioridade do projeto e não serão utilizados para calcular artificialmente uma porcentagem geral de usabilidade do assistente.

A facilidade de memorização exigirá uma avaliação específica de retorno à interface. Na ausência desse procedimento, permanecerá como meta de projeto ainda não verificada diretamente.

## 4. Como o ciclo será iterado

O desenvolvimento do projeto seguirá o modelo de Engenharia de Usabilidade de Mayhew, apresentado nas aulas, que propõe um processo iterativo dividido em três níveis: projeto essencial, padrões de telas e diálogos e projeto detalhado. A ideia é que a interface seja desenvolvida e avaliada gradualmente, permitindo realizar ajustes conforme os problemas identificados e os resultados obtidos.

No nosso projeto, esse processo será aplicado a partir dos artefatos produzidos nas entregas anteriores, como os cenários da Entrega 4, os modelos de tarefas da Entrega 5 e o protótipo em papel da Entrega 6. Esses materiais servirão como base para o desenvolvimento da interface e poderão ser revisitados sempre que forem identificadas dificuldades relacionadas à interação dos estudantes com o assistente virtual.

A aplicação do ciclo será organizada da seguinte maneira:

| Nível da Engenharia de Usabilidade | Aplicação no projeto | Artefatos envolvidos | Avaliação e possíveis revisões |
|---|---|---|---|
| Nível 1 — Projeto essencial | Definir a organização fundamental da interação, considerando os objetivos dos estudantes, as tarefas prioritárias, a formulação de perguntas, a apresentação de fontes e o tratamento de limitações. | Personas, cenários, modelos HTA/GOMS/CTT, protótipos iniciais, instrumentos de coleta e modelo conceitual. | Revisar hipóteses, tarefas e fluxos quando forem identificadas incompatibilidades com os objetivos dos estudantes ou dificuldades na organização geral da interação. |
| Nível 2 — Padrões de telas e diálogos | Definir padrões consistentes para os campos de entrada, respostas, fontes institucionais, linguagem, contraste, feedback de processamento e mensagens de recuperação. | Esquema conceitual de signos, diagramas MoLIC e padrões de interface materializados no Figma. | Realizar inspeções dos fluxos e dos elementos de comunicação, verificando consistência, visibilidade dos estados, compreensibilidade e possibilidades de recuperação. |
| Nível 3 — Projeto detalhado | Materializar os fluxos e padrões em um protótipo navegável, considerando caminhos principais, alternativas, erros e limitações. | Protótipo de alta fidelidade, planejamento DECIDE, avaliação heurística e testes de usabilidade observados. | Avaliar a interface conforme as metas MU01 a MU08, registrar os problemas identificados e propor alterações justificadas pelas evidências obtidas. |

Os três níveis não representam etapas estritamente lineares. Quando uma avaliação indicar problemas relacionados a decisões anteriores, a equipe poderá retornar ao nível correspondente e revisar os artefatos afetados.

Nas próximas etapas, a equipe deverá aprimorar a organização das mensagens, a apresentação das fontes institucionais, os elementos visuais e os mecanismos de feedback. Posteriormente, as avaliações previstas nas Entregas 12, 13 e 14 permitirão identificar problemas de usabilidade e verificar as metas estabelecidas nesta entrega, conforme as evidências efetivamente coletadas.

Por exemplo, caso os testes indiquem que os estudantes apresentam dificuldades para localizar as fontes institucionais, será necessário revisar a forma como essas informações são apresentadas na interface, considerando a tarefa TI03 e a meta MU03. O mesmo processo será aplicado caso sejam identificadas dificuldades na compreensão das respostas, na continuidade da conversa ou no reconhecimento das limitações do assistente.

#### Integração com a coleta de dados da Entrega 7

A Entrega 7 estabeleceu dois instrumentos complementares de coleta:

- I01 — Questionário estruturado.
- I02 — Classificação de Cartões (Card Sorting).

Após o feedback do professor, o questionário foi implementado no Google Forms, publicado e validado funcionalmente. O instrumento de classificação de cartões também teve seu planejamento e procedimento de aplicação complementados.

Entretanto, a equipe optou por não realizar a coleta de dados nesta etapa.

Consequentemente, a publicação dos instrumentos não representa confirmação empírica das hipóteses sobre hábitos, necessidades, familiaridade com inteligência artificial e modelos mentais dos estudantes.

Essas hipóteses continuarão sendo consideradas abertas. Os resultados das avaliações heurísticas e dos testes de usabilidade poderão contribuir para compreender dificuldades específicas de interação, mas não substituirão automaticamente os objetivos exploratórios dos instrumentos da Entrega 7.

#### Relação com as avaliações posteriores

| Entrega | Contribuição para o ciclo de Engenharia de Usabilidade |
|---|---|
| Entrega 9 — Modelo conceitual | Refinar os objetivos, signos e tópicos de conversa necessários à compreensão e utilização da interface. |
| Entrega 10 — MoLIC | Representar as conversas entre estudante e sistema, incluindo caminhos alternativos, processamento, esclarecimentos e recuperação de rupturas. |
| Entrega 11 — Protótipo no Figma | Materializar os modelos de interação em telas e fluxos navegáveis. |
| Entrega 12 — DECIDE | Definir perguntas de avaliação, métodos, participantes, tarefas, métricas, critérios de análise e aspectos éticos. |
| Entrega 13 — Avaliação heurística | Identificar problemas de interface relacionados aos princípios de usabilidade, consistência, comunicação e prevenção de erros. |
| Entrega 14 — Testes de usabilidade | Observar a realização das tarefas por estudantes e registrar evidências sobre eficácia, eficiência, compreensão, dificuldades e satisfação. |

A avaliação heurística contribuirá para identificar problemas de design, enquanto os testes de usabilidade permitirão observar dificuldades durante a realização das tarefas.

O alcance das metas quantitativas deverá ser verificado somente quando os dados necessários tiverem sido efetivamente registrados. A avaliação heurística não será utilizada isoladamente como comprovação de taxas de sucesso, tempos de execução ou satisfação dos estudantes.

#### Registro das decisões e rastreabilidade

As melhorias realizadas deverão ser registradas na matriz de rastreabilidade, relacionando os problemas identificados às decisões tomadas pela equipe.

| Requisito | Aspecto avaliado | Metas associadas | Avaliação prevista |
|---|---|---|---|
| R01 | Formulação e início da consulta acadêmica. | MU01, MU06 e MU07. | Avaliação heurística e teste observado de formulação da pergunta. |
| R02 | Compreensão das informações apresentadas. | MU02 e MU07. | Teste observado de interpretação da resposta e inspeção da clareza das mensagens. |
| R03 | Identificação e consulta das fontes institucionais. | MU03 e MU07. | Teste observado de localização da fonte e inspeção da apresentação das evidências. |
| R04 | Continuidade da conversa durante a sessão. | MU04 e MU07. | Avaliação do fluxo conversacional e teste observado de pergunta complementar. |
| R05 | Reconhecimento da ausência de evidência e orientação para prosseguir. | MU05 e MU07. | Inspeção das mensagens de limitação e teste observado de interpretação e recuperação. |
| R06 | Visibilidade do estado de processamento. | MU08. | Inspeção do feedback apresentado e observação da interpretação do participante durante a espera. |
| R07 | Recuperação de conversas entre sessões, quando contemplada pelo escopo. | Sem meta quantitativa específica nesta etapa. | Investigação exploratória por meio do instrumento I01, sem assumir a funcionalidade como requisito obrigatório confirmado. |

A recuperação de conversas entre sessões, associada à hipótese H15, deverá permanecer distinta da continuidade do contexto durante uma mesma sessão.

Cada iteração deverá registrar, quando aplicável:

- O requisito, a hipótese ou a meta de usabilidade afetada.
- A avaliação ou observação que originou o problema.
- A evidência efetivamente obtida.
- O problema de interação identificado.
- A decisão de manter ou modificar o design.
- O artefato que deverá ser revisado.
- A alteração realizada ou proposta.
- A forma de verificar a alteração em uma avaliação posterior.

As alterações deverão preservar o histórico das decisões, permitindo identificar quais características foram modificadas após a avaliação e quais metas ainda necessitam de verificação.

A matriz `RASTREABILIDADE.md` deverá incorporar os vínculos entre os requisitos R01 a R07, as metas MU01 a MU08, os princípios aplicáveis e as avaliações correspondentes.

A padronização dos identificadores deverá ser propagada aos demais documentos do projeto, mantendo a distinção entre os modelos de análise de tarefas da Entrega 5 e as tarefas gerais de interação representadas por TI01 a TI05.

Dessa forma, o desenvolvimento não ficará limitado à criação de um único protótipo, mas seguirá um processo contínuo de avaliação e aprimoramento, buscando adequar cada vez mais a interface às necessidades dos estudantes.

## Checklist

- [x] Capacidades e restrições têm impacto de IHC explicitado.
- [x] Está claro o limite entre contribuição técnica do TCC e camada interativa da disciplina.
- [x] Resultados/processamento simulados no protótipo foram explicitados.
- [x] Metas de usabilidade avaliam a interação, não substituem métricas técnicas do TCC.
- [x] Normas/princípios estão contextualizados, não apenas copiados.
- [x] Metas quantitativas são mensuráveis e associadas a tarefas/público.
- [x] Eficácia, eficiência e satisfação são consideradas quando pertinentes.
- [x] Metas poderão ser verificadas nas Entregas 12–14.
