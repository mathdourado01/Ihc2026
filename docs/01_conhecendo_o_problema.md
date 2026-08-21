# Entrega 1 — Conhecendo o projeto, o usuário e o problema

**Data:** 20/08/2026
**Status:** 🟨 em andamento  
**Responsabilidade:** 1 solução consolidada por equipe

## Objetivo da atividade

Reinterpretar o tema do TCC sob a perspectiva de Interação Humano-Computador e construir um **entendimento comum entre os integrantes da equipe**.

A disciplina utiliza preferencialmente o tema do TCC para os exercícios de IHC. Isso vale tanto para TCCs que já preveem uma interface quanto para trabalhos cujo resultado principal é algoritmo, modelo, API, biblioteca, análise de dados, infraestrutura, estudo experimental ou outro artefato técnico.

> **Importante:** a interface projetada na disciplina é um artefato de aprendizagem de IHC. Ela **não se torna automaticamente uma obrigação do TCC**. Sua incorporação ao trabalho de conclusão depende de decisão da equipe e do orientador.

Antes de preencher, leia [`../GUIA_ESCOPO_IHC.md`](../GUIA_ESCOPO_IHC.md).

Nesta primeira semana a equipe **não deve começar desenhando telas**. Primeiro deverá compreender:

- o que o TCC realmente produz;
- quem poderia obter valor dessa contribuição;
- quais pessoas interagem, administram, configuram, interpretam ou são afetadas;
- o que essas pessoas precisam alcançar;
- como atividades relacionadas acontecem hoje;
- problemas, limitações e contexto;
- alternativas existentes;
- qual recorte de interação fará sentido para a disciplina.

Ao final desta entrega, a equipe deve diferenciar:

- **tema do TCC** × **escopo formal do TCC** × **escopo de IHC da disciplina**;
- **objetivo do projeto** × **objetivo do usuário**;
- **problema do usuário** × **solução tecnológica**;
- **fato conhecido** × **hipótese** × **lacuna de conhecimento**;
- **capacidade técnica** × **forma de uso dessa capacidade**;
- **funcionalidade** × **atividade/resultado que o usuário precisa alcançar**;
- **usuário direto** × **stakeholders**.

---

## Como classificar as respostas

Sempre que a resposta fizer uma afirmação sobre usuários, problemas, atividades, necessidades, contexto ou mercado, use:

- **[F] Fato conhecido** — existe evidência/fonte.
- **[H] Hipótese** — afirmação plausível que ainda precisa ser investigada.
- **[?] Não sabemos ainda** — lacuna relevante.

Quando usar `[F]`, informe a origem. Hipóteses prioritárias devem receber IDs (`H01`, `H02`...) e também ser registradas em [`../RASTREABILIDADE.md`](../RASTREABILIDADE.md).

> **Exemplo:** `[H] H01 — DBAs considerariam útil comparar automaticamente o plano atual de execução com uma recomendação produzida pelo algoritmo.`

Uma hipótese explicitada é melhor do que uma suposição escondida.

---

# 0. Identificação do TCC e da equipe

## 0.1 Membros

| Nome completo | Matrícula | GitHub |
|---|---:|---|
| Matheus Dourado Valle | 22.224.023-6 | mathdourado01 |
| João Pedro Sabino Garcia | 22.224.032-7 | unifjgarcia |

## 0.2 Título atual do TCC

Assistente Virtual com Inteligência Artificial para Suporte a Dúvidas Acadêmicas e Administrativas na FEI

## 0.3 Orientador(a)

Rafael Gomes Alves 

## 0.4 Qual é o resultado principal atualmente previsto no TCC?

Marque e descreva:

- [x] sistema/aplicação interativa;
- [ ] algoritmo;
- [ ] modelo de IA/ML/LLM;
- [ ] biblioteca/API/framework;
- [ ] análise de dataset;
- [x] estudo/benchmark/avaliação experimental;
- [ ] infraestrutura/backend;
- [ ] componente embarcado/IoT;
- [ ] outro: {{...}}.

**Descrição:**  O TCC prevê como resultados principais o desenvolvimento de um protótipo funcional de assistente virtual com Inteligência Artificial para suporte a dúvidas acadêmicas e administrativas na FEI e a avaliação experimental da arquitetura utilizada. O protótipo permitirá que usuários realizem perguntas em linguagem natural e recebam respostas fundamentadas em informações recuperadas de fontes institucionais. Paralelamente, serão avaliadas diferentes configurações de segmentação documental e recuperação, além da qualidade das respostas geradas, permitindo analisar o desempenho e as limitações da solução proposta.

## 0.5 O TCC já previa desenvolvimento de interface com usuário?

- [x] Sim, a interface já faz parte do TCC.
- [ ] Parcialmente; existe alguma interação, mas ainda não está bem definida.
- [ ] Não. O TCC é predominantemente técnico e não previa interface.

**Explique o que está formalmente previsto no TCC:** O TCC prevê formalmente uma interface de interação com o usuário como parte do protótipo do assistente virtual. Por meio dessa interface, o usuário deverá inserir uma dúvida acadêmica ou administrativa, que será encaminhada ao backend e ao mecanismo de recuperação de informações. Após a recuperação das evidências institucionais e a geração da resposta pelo modelo de linguagem, o resultado deverá ser apresentado novamente ao usuário pela interface. Embora a interface faça parte do escopo do TCC, seus aspectos específicos de interação e usabilidade poderão ser aprofundados no projeto desenvolvido na disciplina de IHC.

> Esta resposta serve para separar o compromisso do TCC do projeto da disciplina. Mesmo quando a opção for **não**, a equipe irá definir uma interface para exercitar IHC.

---

# 1. Entendendo a contribuição do projeto

## 1.1 Explique o TCC em uma frase, sem citar linguagem de programação, framework ou banco de dados.

O TCC propõe o desenvolvimento e a avaliação de um assistente virtual com Inteligência Artificial capaz de responder dúvidas acadêmicas e administrativas com base em informações institucionais da FEI.

## 1.2 Qual situação, atividade ou problema do mundo real motivou o TCC?

[H] O TCC foi motivado pela recorrência de dúvidas acadêmicas e administrativas relacionadas a processos institucionais, normas, serviços, prazos e orientações gerais, cuja resolução pode exigir a busca manual por informações distribuídas entre diferentes páginas, documentos e canais institucionais. Fonte: texto atual do TCC, especialmente Resumo, Introdução e Conclusão.

[?] Ainda não sabemos, com base em uma investigação direta com os alunos da FEI, quais dessas dificuldades são mais frequentes, quais canais são mais utilizados e quais situações geram maior esforço ou insatisfação.

## 1.3 Qual é a **capacidade/contribuição central** produzida pelo TCC?
Nosso TCC permite recuperar informações relevantes de uma base documental institucional e utilizá-las como evidência para gerar respostas em linguagem natural a dúvidas acadêmicas e administrativas, além de avaliar experimentalmente como diferentes configurações técnicas influenciam a qualidade da recuperação e das respostas.

## 1.4 O que se espera que esteja diferente **para pessoas, organizações ou processos** se essa contribuição for bem-sucedida?

[H] H01 — Espera-se que os estudantes possam localizar e compreender informações acadêmicas e administrativas de forma mais centralizada, reduzindo a necessidade de consultar manualmente diferentes páginas, documentos ou canais para esclarecer uma dúvida.

[H] H02 — Espera-se que a fundamentação das respostas em fontes institucionais aumente a confiança e a utilidade das informações apresentadas ao estudante quando comparada a uma resposta produzida sem acesso ao contexto documental da instituição.

[H] H03 — Para a instituição, o uso do assistente poderá apoiar o atendimento de dúvidas recorrentes, permitindo que parte das consultas informacionais seja resolvida pelo próprio estudante sem necessidade de recorrer imediatamente a um canal de atendimento humano.

## 1.5 O que é mérito técnico/científico do TCC e o que seria uma possível aplicação prática?

| Mérito/contribuição técnica | Possível aplicação/valor em uso |
|---|---|
| Desenvolvimento e avaliação de uma arquitetura baseada em recuperação de informações e geração de respostas para o domínio acadêmico-administrativo da FEI. | Permitir que estudantes consultem informações acadêmicas e administrativas por meio de uma interface conversacional. |
| Avaliação experimental do impacto de diferentes estratégias de segmentação documental e parâmetros de recuperação na qualidade do sistema. | Buscar configurações que favoreçam respostas mais relevantes e fundamentadas para as dúvidas dos estudantes. |
| Uso e preservação de fontes institucionais como evidência para a geração das respostas e para delimitação do escopo do assistente. | Permitir que o estudante tenha acesso à resposta acompanhada de informações relacionadas às fontes institucionais utilizadas. |
---

# 2. Entendendo as pessoas envolvidas

## 2.1 Quem interage diretamente com o produto, se já existe interface prevista?
[F] O usuário direto previsto para a interface é o estudante da FEI que deseja obter informações relacionadas a dúvidas acadêmicas e administrativas. O TCC prevê que esse usuário envie perguntas em linguagem natural por meio da interface do assistente e receba respostas fundamentadas nas informações institucionais recuperadas pelo sistema

## 2.2 Quem poderia **usar, configurar, administrar, operar, interpretar ou tomar decisões** a partir da contribuição técnica?

Considere perfis profissionais e stakeholders, não apenas consumidores finais.

| Perfil | Relação com a contribuição | O que faria | Status/evidência |
|---|---|---|---|
| Estudante da FEI | Usuário direto do assistente virtual | Formular dúvidas acadêmicas ou administrativas e interpretar as respostas e fontes apresentadas pelo sistema | F |
| Equipe responsável pelo desenvolvimento e avaliação do sistema | Responsável pela configuração técnica, operação dos experimentos e análise dos resultados | Configurar parâmetros do sistema, executar testes, analisar trechos recuperados, respostas geradas e métricas de desempenho | F |
| Profissional ou setor da FEI com conhecimento dos processos acadêmicos e administrativos | Pode contribuir para a validação das fontes e das respostas utilizadas pelo assistente | Validar documentos, procedimentos e, quando possível, verificar se respostas estão de acordo com as práticas e normas institucionais | F |


## 2.3 Existem pessoas afetadas que não usariam a interface diretamente?

| Stakeholder | Como é afetado | Usa interface? | Status/evidência |
|---|---|---|---|
| Setores acadêmicos e administrativos responsáveis pelas informações utilizadas pelo assistente | Suas páginas, documentos, normas e orientações podem ser utilizadas como fonte para fundamentar as respostas fornecidas aos estudantes  | Não Necessariamente | F
| Profissionais responsáveis por atendimento de dúvidas acadêmicas e administrativas | O assistente poderá alterar a forma como algumas dúvidas recorrentes chegam aos canais tradicionais de atendimento | Não Necessariamente | H — efeito ainda não investigado
| Centro Universitário FEI | A instituição é responsável pelas informações e procedimentos que servem de referência para o domínio no qual o assistente pretende atuar | Não | F
## 2.4 Que características desses perfis podem influenciar a interação?

- [H] Os estudantes podem formular uma mesma dúvida utilizando vocabulários e níveis de detalhamento diferentes. Essa possibilidade é relevante para uma interface baseada em linguagem natural e deverá ser considerada durante o projeto e a avaliação da interação.
- [F] Pessoas responsáveis pela validação das respostas e das fontes precisam possuir conhecimento dos processos acadêmicos ou administrativos relacionados ao conteúdo avaliado.
- [?] Ainda não sabemos quais são os níveis de experiência tecnológica dos estudantes, a frequência com que utilizariam o assistente, quais dispositivos seriam predominantes ou quais necessidades específicas de acessibilidade devem ser consideradas.

---

# 3. Entendendo objetivos e atividades

## 3.1 O que o usuário está tentando conseguir no mundo real?

[H] H04 — O estudante busca obter e compreender informações acadêmicas ou administrativas necessárias para resolver uma dúvida, tomar uma decisão ou realizar corretamente um procedimento relacionado à sua vida acadêmica na FEI.

[F] O TCC delimita como domínio de interesse informações relacionadas a normas, prazos, procedimentos, serviços e orientações acadêmico-administrativas.


## 3.2 Quais são as atividades mais importantes?

| ID | Atividade/objetivo | Quem realiza | Frequência/criticidade inicial | Status/evidência |
|---|---|---|---|---|
| A01 |Localizar e compreender uma informação acadêmica ou administrativa, como uma regra, prazo, serviço ou orientação institucional | Estudante da FEI | Frequência alta; criticidade variável conforme a informação consultada| F |
| A02 | Entender como realizar um procedimento acadêmico ou administrativo e quais etapas ou condições devem ser observadas | Estudante da FEI | Frequência alta ; criticidade potencialmente alta quando envolve regras ou prazos | H — o TCC contempla consultas procedimentais, mas o comportamento dos usuários ainda precisa ser investigado |


## 3.3 Qual atividade parece mais frequente? Por quê?

[H] H05 — A atividade A01, de localizar e compreender informações acadêmicas ou administrativas, parece ser a mais frequente, pois o TCC é motivado pela recorrência de consultas informacionais relacionadas a normas, serviços, prazos, procedimentos e orientações gerais.

[?] Entretanto, ainda não há levantamento direto com estudantes da FEI que permita determinar qual atividade ocorre com maior frequência ou quais tipos de dúvida predominam.

## 3.4 Qual parece mais crítica? Que consequência existe se for mal executada?

[H] H06 — A atividade A02, relacionada à compreensão e realização de procedimentos acadêmicos ou administrativos, parece possuir maior criticidade, especialmente quando a informação envolve regras, etapas obrigatórias ou prazos. Uma interpretação incorreta pode levar o estudante a executar um procedimento de maneira inadequada, deixar de cumprir alguma etapa necessária ou tomar uma decisão com base em uma orientação incorreta.

[?] A gravidade e a frequência dessas consequências ainda precisam ser investigadas com estudantes e, quando pertinente, com profissionais responsáveis pelos processos acadêmicos e administrativos.

---

# 4. Entendendo o problema ou processo atual

## 4.1 Como essas atividades são realizadas hoje, antes da interface imaginada na disciplina?

Pode existir software concorrente, linha de comando, planilha, notebook, script, painel técnico, processo manual, consulta a logs, análise visual, troca de mensagens, decisão por especialista etc.

[F] O TCC apresenta como situação atual a possibilidade de o estudante precisar realizar buscas manuais por informações acadêmicas e administrativas em diferentes páginas institucionais e canais de atendimento para esclarecer suas dúvidas. Fonte: TCC — Resumo e Introdução.

[H] H07 — Na prática, estudantes podem recorrer a diferentes meios, como páginas do site institucional, documentos e regulamentos, sistemas acadêmicos ou contato com pessoas e setores da instituição, dependendo do tipo de dúvida.

[?] Ainda não sabemos quais canais são efetivamente mais utilizados pelos estudantes, em qual ordem são consultados e em quais situações eles recorrem a atendimento humano.

## 4.2 O que é difícil, demorado, confuso, repetitivo, arriscado ou pouco transparente?

[H] H08 — A distribuição das informações entre diferentes páginas, documentos e canais pode dificultar a identificação de onde procurar uma determinada informação e aumentar o esforço necessário para resolver uma dúvida.

[H] H09 — Informações relacionadas a regras, procedimentos ou prazos podem exigir interpretação por parte do estudante, principalmente quando estão apresentadas em documentos extensos ou quando ele não conhece previamente o setor ou a fonte responsável pelo assunto.

## 4.3 Que informações o profissional precisa interpretar para tomar decisão?

[H] Dependendo da dúvida, o estudante pode precisar interpretar informações como prazos, regras acadêmicas, requisitos, documentos necessários, etapas de um procedimento, setor responsável, condições ou exceções aplicáveis e orientações institucionais relacionadas à sua situação.

## 4.4 O que acontece quando a atividade falha ou quando o resultado é interpretado incorretamente?

[H] H10 — Quando uma informação acadêmica ou administrativa não é localizada ou é interpretada incorretamente, o estudante pode realizar um procedimento de maneira inadequada, deixar de cumprir alguma etapa ou prazo, tomar uma decisão com base em uma compreensão incorreta ou precisar recorrer posteriormente a um canal de atendimento para esclarecer a situação.

[?] A frequência e a gravidade dessas consequências ainda precisam ser investigadas com estudantes e, quando necessário, com os setores responsáveis pelos processos acadêmicos e administrativos.

## 4.5 Conte uma situação concreta.


[F] Um estudante da FEI que está próximo de concluir a graduação considera continuar seus estudos em um programa de mestrado da instituição. Para entender como funciona esse processo, ele precisa localizar informações sobre o programa, processo de ingresso, requisitos e orientações relacionadas. Durante essa busca, pode ser necessário consultar diferentes páginas ou documentos institucionais e identificar quais informações são relevantes para sua situação. Caso não encontre ou interprete corretamente essas informações, pode permanecer com dúvidas e precisar procurar outro canal ou pessoa da instituição para obter esclarecimentos.


## 4.6 Que evidência existe hoje?

| Evidência/fonte | O que sustenta | Limitação |
|---|---|---|
| Páginas e documentos institucionais disponíveis nos canais oficiais da FEI | Permitem observar que informações acadêmicas e administrativas são disponibilizadas por meio de diferentes páginas, documentos e áreas institucionais | A existência de diferentes fontes não demonstra, por si só, que os estudantes tenham dificuldade para encontrá-las ou interpretá-las |
| Literatura sobre assistentes virtuais e suporte estudantil no ensino superior levantada durante o TCC | Indica que dúvidas recorrentes, acesso a informações institucionais e suporte acadêmico-administrativo são problemas tratados por outras instituições e pesquisas | Os estudos analisados não representam diretamente a experiência dos estudantes da FEI |
| Levantamento direto com estudantes da FEI | Ainda não disponível | Será necessário para verificar quais dificuldades realmente existem, quais canais são utilizados e quais tipos de dúvida são mais frequentes |
| Contato com profissionais/setores responsáveis por processos acadêmicos e administrativos | Ainda precisa ser aprofundado | Poderá ajudar a identificar dúvidas recorrentes e problemas observados nos canais atuais de atendimento |
---

# 5. Entendendo o contexto de uso

## 5.1 Onde e em quais situações a interação poderia ocorrer?

[H] H11 — A interação poderá ocorrer tanto dentro quanto fora do ambiente da FEI, em situações nas quais o estudante precise esclarecer uma dúvida acadêmica ou administrativa, como consultar uma regra, verificar um prazo ou compreender como realizar determinado procedimento.


## 5.2 Em quais dispositivos/equipamentos?

[H] H12 — Por se tratar de uma interface digital de consulta, é plausível que o acesso ocorra por computadores, notebooks ou dispositivos móveis.

## 5.3 Existem condições físicas relevantes?

[F] A arquitetura proposta depende da comunicação com serviços externos para geração das respostas por meio de API.

[?] Ainda não sabemos se limitações de conexão, privacidade durante a consulta, ruído, uso compartilhado de equipamentos ou outras condições físicas representam problemas relevantes para os estudantes.

## 5.4 Existem fatores sociais ou organizacionais?

[F] As informações utilizadas pelo assistente pertencem ao contexto institucional da FEI, e o TCC prevê que documentos e fontes possam ser selecionados ou validados com apoio de setores responsáveis, como secretaria acadêmica, coordenação ou outras áreas administrativas.

[H] H14 — A confiabilidade percebida pelo estudante poderá ser influenciada pela clareza sobre a origem institucional das informações apresentadas.

## 5.5 Existe necessidade de histórico, rastreabilidade ou auditoria?

[F] Existe necessidade de rastreabilidade técnica das informações utilizadas pelo sistema. O TCC prevê preservar os metadados dos documentos e registrar, durante as execuções, informações como os trechos recuperados, suas fontes, a configuração utilizada e a resposta gerada. Esses registros serão utilizados principalmente para avaliar a recuperação documental e a aderência das respostas às fontes institucionais. 

[H] H15 — Para o estudante, um histórico de conversas anteriores pode ser útil para retomar informações ou consultas realizadas anteriormente.

[?] Ainda não sabemos se o histórico de conversas representa uma necessidade real dos estudantes e quais informações deveriam ser armazenadas ou apresentadas.

## 5.6 Um erro pode produzir consequência relevante? Qual?

[H] H16 — Sim. Uma resposta incorreta ou uma interpretação equivocada de informações relacionadas a regras, prazos ou procedimentos pode fazer com que o estudante tome uma decisão inadequada, deixe de cumprir uma etapa necessária ou procure o setor responsável com uma compreensão incorreta da situação.

[F] Por esse motivo, o TCC estabelece que, quando não houver evidência documental suficiente, o sistema deverá reconhecer essa limitação em vez de gerar uma resposta sem fundamento institucional. 

[?] Ainda precisamos investigar quais tipos de erro são considerados mais graves pelos estudantes e pelos setores responsáveis da FEI.

---

# 6. Entendendo mercado e alternativas existentes

> Nesta entrega faça apenas um **levantamento inicial**. A análise aprofundada ocorre na Entrega 2.

## 6.1 Como pessoas resolvem problemas semelhantes hoje?

| Alternativa atual | Quem usa | Para quê | Status/evidência |
|---|---|---|---|
| Páginas institucionais e portal acadêmico | Estudantes | Consultar informações sobre matrícula, calendário, documentos, estágio, sistemas e procedimentos acadêmicos | **[F]** O TCC identifica que informações acadêmico-administrativas podem estar distribuídas em diferentes páginas, documentos e canais institucionais. |
| Atendimento por setores da instituição | Estudantes | Esclarecer dúvidas que não foram resolvidas pelas informações disponíveis nos sistemas e páginas institucionais | **[F]** A literatura analisada aponta que canais humanos recebem demandas recorrentes e que chatbots podem reduzir tarefas repetitivas de atendimento [3], [11], [20], [26]. |
| FAQ e sistemas baseados em regras | Estudantes de instituições de ensino | Obter respostas para perguntas frequentes previamente cadastradas | **[F]** Trabalhos como [8] e [21] apresentam sistemas universitários baseados em regras, fluxos e perguntas frequentes. |
| Chatbots universitários | Estudantes | Obter orientação acadêmica e informações sobre serviços institucionais por meio de conversação | **[F]** Trabalhos como [11] e [17] apresentam chatbots voltados ao suporte estudantil e administrativo. |
| Assistentes de IA generativa | Usuários em geral, incluindo estudantes | Formular perguntas em linguagem natural e obter respostas de maneira rápida | **[F]** O TCC considera sistemas como ChatGPT, Gemini e Copilot como alternativas conversacionais de uso geral, embora não sejam específicos para as regras da FEI. |
| Assistentes baseados em RAG | Estudantes e usuários de sistemas educacionais | Obter respostas geradas a partir de documentos recuperados de uma base de conhecimento | **[F]** Os trabalhos [13], [24] e [25] discutem o uso de documentos e recuperação de informações para apoiar respostas mais contextualizadas. |

## 6.2 Existem produtos que atuam na mesma área, mesmo sem serem equivalentes ao TCC?

**[F]** Existem diferentes soluções que atuam parcialmente no mesmo espaço do assistente proposto. Sistemas de IA generativa de uso geral, como **ChatGPT, Google Gemini e Microsoft Copilot**, oferecem interfaces conversacionais capazes de responder perguntas em linguagem natural, mas não possuem, por padrão, uma base de conhecimento específica e validada sobre os processos acadêmico-administrativos da FEI.

**[F]** No contexto universitário, também existem soluções desenvolvidas especificamente para suporte a estudantes. O **FIT-EBot**, apresentado em [11], oferece suporte administrativo e de aprendizagem em ambiente universitário. O trabalho [21] apresenta um chatbot voltado a perguntas frequentes relacionadas à universidade, enquanto [13] propõe um agente virtual baseado em modelo de linguagem para responder dúvidas relacionadas às políticas presentes no manual do estudante.

## 6.3 Quais interfaces profissionais esse público já conhece?

**[H] H17 —** Considerando o público-alvo formado principalmente por estudantes, as interfaces mais próximas do contexto do projeto são **portais acadêmicos, páginas institucionais, sistemas de consulta de informações e interfaces conversacionais de chat**.

**[H] H18 —** Interfaces semelhantes às utilizadas por assistentes como ChatGPT, Gemini e Copilot podem ser familiares a parte dos estudantes, principalmente o padrão de interação formado por **campo para digitação da pergunta, histórico da conversa e respostas apresentadas em sequência**.

**[?]** O grau de familiaridade dos estudantes da FEI com cada uma dessas interfaces ainda deverá ser confirmado por meio de investigação com os usuários.

## 6.4 O que essas soluções parecem fazer bem?

**[F]** Sistemas baseados em FAQ e regras apresentam como vantagem a **previsibilidade das respostas**, pois trabalham com conteúdos e intenções previamente cadastrados [8], [21].

**[F]** Chatbots voltados ao suporte universitário permitem **automatizar o atendimento de dúvidas recorrentes**, ampliar a disponibilidade de informações e reduzir a necessidade de intervenção humana em consultas repetitivas [3], [11], [20], [26].

**[F]** Sistemas baseados em modelos de linguagem oferecem maior flexibilidade na interação, permitindo que o usuário formule uma mesma dúvida de diferentes maneiras e receba respostas em linguagem natural [1], [13], [14].

**[H] H19 —** Do ponto de vista de interface, o formato conversacional pode reduzir a necessidade de o usuário conhecer previamente onde determinada informação está localizada dentro da estrutura de páginas ou documentos da instituição.

## 6.5 O que parecem fazer mal, dificultar ou não atender?

**[F]** Sistemas baseados em FAQ e regras possuem dificuldade para lidar com perguntas que não foram previamente cadastradas e com diferentes formas de formular uma mesma dúvida [8], [21].

**[F]** Soluções universitárias tradicionais podem depender de bases de conhecimento organizadas manualmente e apresentar limitações para integração com diferentes documentos e processos administrativos [11].

**[F]** Modelos de linguagem generativos podem produzir respostas plausíveis, mas incorretas ou não aderentes às normas da instituição, tornando necessário controlar a factualidade e verificar as evidências utilizadas [4], [13], [29].

**[F]** Mesmo sistemas baseados em RAG continuam dependentes da qualidade da base documental e da recuperação. Um documento inadequado, desatualizado ou um trecho pouco relevante pode prejudicar a resposta final [22], [24], [25].

**[F]** A literatura também aponta desafios relacionados à atualização da base de conhecimento, qualidade da recuperação e avaliação das respostas em sistemas educacionais baseados em RAG [25].

**[H] H20 —** No caso das páginas e documentos institucionais tradicionais, a necessidade de identificar manualmente onde determinada informação está localizada pode aumentar o esforço do estudante quando a dúvida envolve diferentes páginas ou documentos.

## 6.6 Que padrões de interface ou vocabulário parecem familiares a esse público?

**[H] H21 —** O padrão de **interface conversacional**, composto por histórico de mensagens, campo para digitação da pergunta e envio da mensagem, parece adequado ao repertório de interfaces já difundidas entre usuários de sistemas de chat e assistentes de IA.

**[H] H22 —** Outros elementos potencialmente familiares são campos de busca, links para fontes, indicação da origem da informação, organização de conteúdo por categorias e mensagens de erro ou de informação não encontrada.

**[F]** Para o domínio acadêmico-administrativo, termos como **matrícula, notas, documentos, financeiro, estágio, calendário acadêmico, portal do aluno e sistemas institucionais** já fazem parte das categorias previstas no escopo do projeto.

---

# 7. Derivando o escopo de IHC da disciplina

## 7.1 Escolha o caminho do projeto

### Caminho A — TCC já possui interface

Explique qual parte da interface será usada como recorte da disciplina e por que esse fluxo é relevante.

{{...}}

### Caminho B — TCC não possui interface prevista

Faça o exercício de transferência de uso:

> **Imagine que o TCC foi concluído com sucesso e uma empresa, laboratório ou organização quer transformar a contribuição em algo utilizável. Quem precisaria interagir com ela e para quê?**

Responda:

1. quem poderia contratar/adotar a solução? {{...}}
2. quem seria o usuário direto? {{...}}
3. quem administraria/configuraria? {{...}}
4. quem interpretaria resultados? {{...}}
5. quem tomaria decisões? {{...}}
6. quais dados/entradas seriam necessários? {{...}}
7. quais resultados deveriam ser compreendidos? {{...}}
8. que erros/rupturas seriam possíveis? {{...}}

## 7.2 Qual perfil será priorizado no projeto de IHC?

{{...}}

**Por que esse perfil foi escolhido?** {{...}}

## 7.3 Qual objetivo desse usuário será priorizado?

{{...}}

## 7.4 Que interface será explorada na disciplina?

Complete:

> **Para fins da disciplina de IHC, será projetada uma interface que permita a `{{perfil}}` utilizar `{{capacidade/resultado do TCC}}` para `{{objetivo}}`, no contexto de `{{situação}}`.**

{{...}}

## 7.5 Qual é a relação dessa interface com o TCC?

- [ ] Já fazia parte do TCC.
- [ ] É um aprofundamento de algo parcialmente previsto.
- [ ] É uma extensão conceitual criada para a disciplina.
- [ ] É um protótipo demonstrativo de aplicação potencial.
- [ ] Outra: {{...}}.

> **Declaração:** a interface desenvolvida nesta disciplina é um artefato de aprendizagem de IHC baseado no tema do TCC. Sua inclusão ou implementação no TCC somente ocorrerá se isso for posteriormente decidido pela equipe e pelo orientador.

---

# 8. Levantando possibilidades de interação — sem desenhar ainda

A equipe pode registrar possibilidades para investigação. **Não significa que todas serão implementadas.**

Marque apenas as que parecem plausíveis e explique o objetivo correspondente.

| Possibilidade | Pode fazer sentido? | Objetivo/tarefa que justificaria | Evidência atual |
|---|---|---|---|
| Dashboard/visão geral | sim/não/talvez | {{...}} | {{...}} |
| Configuração/parametrização | sim/não/talvez | {{...}} | {{...}} |
| Entrada/upload/seleção de dados | sim/não/talvez | {{...}} | {{...}} |
| Acompanhamento de processamento | sim/não/talvez | {{...}} | {{...}} |
| Relatório/resultados | sim/não/talvez | {{...}} | {{...}} |
| Histórico com busca/filtros | sim/não/talvez | {{...}} | {{...}} |
| Comparação de resultados | sim/não/talvez | {{...}} | {{...}} |
| Explicabilidade/detalhamento | sim/não/talvez | {{...}} | {{...}} |
| Administração/configurações globais | sim/não/talvez | {{...}} | {{...}} |
| Usuários/perfis/permissões | sim/não/talvez | {{...}} | {{...}} |
| CRUD de entidade do domínio | sim/não/talvez | {{...}} | {{...}} |
| Auditoria/logs | sim/não/talvez | {{...}} | {{...}} |
| Alertas/ocorrências | sim/não/talvez | {{...}} | {{...}} |
| Ajuda/documentação | sim/não/talvez | {{...}} | {{...}} |

> **Atenção:** “login + dashboard + CRUD” não é uma solução universal. Cada padrão deve surgir de uma tarefa real.

---

# 9. Benefícios e ações iniciais

## 9.1 Qual benefício concreto o projeto de IHC pretende oferecer?

| Benefício esperado | Problema/necessidade | Usuário | Status/evidência |
|---|---|---|---|
| {{...}} | {{...}} | {{...}} | {{...}} |

## 9.2 Que ações o usuário deverá conseguir realizar?

| ID | O usuário precisa conseguir... | Para alcançar... | Prioridade inicial |
|---|---|---|---|
| F01 | {{ação}} | {{objetivo}} | alta/média/baixa |

## 9.3 Tecnologias/restrições já definidas no TCC

A tecnologia aparece **agora**, depois do entendimento do uso.

| Tecnologia/restrição | Por que existe | Possível impacto na interação |
|---|---|---|
| {{...}} | {{...}} | {{...}} |

---

# 10. Hipóteses e dúvidas prioritárias

| ID | Hipótese/dúvida | Por que importa | Como poderá ser investigada |
|---|---|---|---|
| H01 | {{...}} | {{...}} | Entrega 2/3/7/... |
| H02 | {{...}} | {{...}} | {{...}} |
| H03 | {{...}} | {{...}} | {{...}} |

Registre em [`../RASTREABILIDADE.md`](../RASTREABILIDADE.md).

---

# 11. Síntese da equipe

| Pergunta | Síntese atual |
|---|---|
| Qual é a contribuição central do TCC? | {{...}} |
| O TCC já previa interface? | {{...}} |
| Quem é o usuário prioritário de IHC? | {{...}} |
| O que ele precisa alcançar? | {{...}} |
| Qual problema/atividade será estudado? | {{...}} |
| Como isso acontece hoje? | {{...}} |
| Qual é o contexto de uso? | {{...}} |
| Que interface/recorte será explorado? | {{...}} |
| Como a interface se relaciona ao TCC? | {{...}} |
| Quais pontos ainda são hipóteses? | {{H01...}} |

### Delimitação

**Dentro do escopo de IHC:** {{...}}  
**Fora do escopo de IHC:** {{...}}  
**Dentro do escopo formal do TCC:** {{...}}  
**Interface da disciplina será implementada no TCC?** não definido / sim / não — {{justificativa, se houver}}

---

# 12. Como esta entrega alimenta as próximas

- **Entrega 2:** verifica mercado, concorrentes e interfaces profissionais representativas.
- **Entrega 3:** detalha perfis e contexto.
- **Entrega 4:** aprofunda situações problemáticas.
- **Entrega 5:** modela tarefas centrais.
- **Entrega 6:** experimenta alternativas em baixa fidelidade.
- **Entrega 7:** investiga hipóteses com dados.
- **Entrega 8:** define restrições e metas de usabilidade.
- **Entregas 9–11:** transformam o recorte em modelo de interação e protótipo.
- **Entregas 12–14:** avaliam a interface construída na disciplina.

A Entrega 1 é uma **fotografia inicial do conhecimento**. Ela pode e deve ser revisada quando surgirem evidências.

---

# 13. Relação com INOVA e comunicação do projeto

Prepare uma explicação de até três frases:

1. **Problema/atividade humana:** {{...}}
2. **Contribuição técnica do TCC:** {{...}}
3. **Como uma pessoa poderia utilizar essa contribuição:** {{...}}

Essa síntese ajuda a apresentar o projeto para público não especializado sem reduzir seu mérito técnico.

---

# Checklist de qualidade

- [ ] Está clara a diferença entre tema do TCC, escopo formal do TCC e escopo de IHC.
- [ ] A equipe declarou se o TCC já previa interface.
- [ ] Se não previa, foi derivado um usuário plausível e um objetivo de uso.
- [ ] A interface de IHC não foi apresentada como obrigação automática do TCC.
- [ ] A contribuição do TCC foi descrita sem começar por tecnologias de implementação.
- [ ] Usuários diretos e stakeholders foram diferenciados.
- [ ] Foram considerados profissionais que configuram, administram, interpretam ou decidem, quando pertinente.
- [ ] Objetivo do usuário não foi confundido com objetivo do projeto.
- [ ] Processo/problema atual foi descrito antes da solução.
- [ ] Existe situação concreta de uso/problema.
- [ ] Contexto físico, social/organizacional, dispositivos e consequências de erro foram considerados.
- [ ] Mercado/alternativas existentes foram levantados inicialmente.
- [ ] Possibilidades como dashboard, relatório, histórico, filtros e CRUD foram tratadas como hipóteses de solução, não como requisitos automáticos.
- [ ] Cada possibilidade de interface tem um objetivo/tarefa que poderia justificá-la.
- [ ] Afirmações relevantes estão marcadas `[F]`, `[H]` ou `[?]`.
- [ ] Hipóteses prioritárias receberam IDs e foram para a rastreabilidade.
- [ ] O recorte de IHC é viável para modelar, prototipar e avaliar no semestre.
- [ ] A equipe consegue explicar problema humano → contribuição computacional → forma de uso.
