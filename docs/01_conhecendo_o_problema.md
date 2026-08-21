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

O projeto seguirá o **Caminho A**, pois o TCC já prevê formalmente uma interface de interação com o usuário.

Para a disciplina de IHC, será utilizado como recorte o **fluxo de consulta do estudante**, desde a formulação de uma dúvida acadêmica ou administrativa até a apresentação e compreensão da resposta fornecida pelo assistente.

Esse fluxo poderá envolver a formulação da pergunta em linguagem natural, a apresentação da resposta, a identificação das fontes institucionais utilizadas e o tratamento de situações em que não exista evidência suficiente para responder à consulta.

**[F]** Esse recorte deriva diretamente da interface prevista no TCC, na qual o estudante envia perguntas em linguagem natural e recebe respostas fundamentadas em informações institucionais recuperadas pelo sistema.

**[H] H04 —** O estudante busca obter e compreender informações acadêmicas ou administrativas necessárias para resolver uma dúvida, tomar uma decisão ou realizar corretamente um procedimento relacionado à sua vida acadêmica na FEI.

**[H] H08 —** A distribuição das informações entre diferentes páginas, documentos e canais pode aumentar o esforço necessário para o estudante resolver uma dúvida.

## 7.2 Qual perfil será priorizado no projeto de IHC?

**[F]** O perfil priorizado será o **estudante da FEI que necessita localizar ou compreender uma informação acadêmica ou administrativa**.

**Por que esse perfil foi escolhido?**

O estudante foi escolhido por ser o usuário direto previsto para a interface do assistente no TCC. É esse perfil que formula as dúvidas, interpreta as respostas apresentadas e poderá utilizar as informações recuperadas para compreender regras, prazos, serviços ou procedimentos acadêmico-administrativos.

Além disso, as atividades **A01 — localizar e compreender uma informação acadêmica ou administrativa** e **A02 — entender como realizar um procedimento acadêmico ou administrativo** são realizadas diretamente por esse perfil.

**[?]** Ainda será necessário investigar diretamente com estudantes da FEI suas características, dificuldades, canais utilizados atualmente, familiaridade com interfaces conversacionais e expectativas em relação ao assistente.

## 7.3 Qual objetivo desse usuário será priorizado?

**[H] H04 —** O objetivo priorizado será **obter e compreender uma informação acadêmica ou administrativa necessária para resolver uma dúvida, tomar uma decisão ou realizar corretamente um procedimento relacionado à vida acadêmica na FEI**.

Esse objetivo está relacionado principalmente às atividades:

- **A01:** localizar e compreender uma informação acadêmica ou administrativa, como uma regra, prazo, serviço ou orientação institucional;
- **A02:** entender como realizar um procedimento acadêmico ou administrativo e quais etapas ou condições devem ser observadas.

## 7.4 Que interface será explorada na disciplina?

> **Para fins da disciplina de IHC, será projetada uma interface que permita ao estudante da FEI utilizar a capacidade do assistente de recuperar informações institucionais e gerar respostas fundamentadas para localizar e compreender informações acadêmicas ou administrativas, no contexto de uma dúvida relacionada à sua vida acadêmica na FEI.**

A interface explorada terá como foco o fluxo conversacional de consulta, considerando inicialmente elementos como:

- formulação da dúvida em linguagem natural;
- apresentação da resposta ao estudante;
- apresentação da origem ou fonte institucional utilizada;
- continuidade da interação por meio de novas perguntas;
- comunicação de situações em que o sistema não possua evidência suficiente para responder.

Esses elementos representam um recorte inicial e poderão ser revisados nas próximas entregas conforme novas evidências forem obtidas por meio da investigação com usuários e da análise de interfaces existentes.

## 7.5 Qual é a relação dessa interface com o TCC?

- [x] Já fazia parte do TCC.
- [ ] É um aprofundamento de algo parcialmente previsto.
- [ ] É uma extensão conceitual criada para a disciplina.
- [ ] É um protótipo demonstrativo de aplicação potencial.
- [ ] Outra: {{...}}.

A interface já fazia parte do TCC, pois o protótipo prevê que o estudante envie perguntas em linguagem natural e receba respostas geradas a partir das informações institucionais recuperadas pelo sistema.

> **Declaração:** a interface desenvolvida nesta disciplina é um artefato de aprendizagem de IHC baseado no tema do TCC. Sua inclusão ou implementação no TCC somente ocorrerá se isso for posteriormente decidido pela equipe e pelo orientador.
---

# 8. Levantando possibilidades de interação — sem desenhar ainda

A equipe pode registrar possibilidades para investigação. **Não significa que todas serão implementadas.**

Marque apenas as que parecem plausíveis e explique o objetivo correspondente.

| Possibilidade | Pode fazer sentido? | Objetivo/tarefa que justificaria | Evidência atual |
|---|---|---|---|
| Dashboard/visão geral | não | O fluxo principal do estudante está relacionado à realização de consultas, e não ao acompanhamento de indicadores ou informações agregadas | **[F]** O TCC prevê como interação principal o envio de perguntas e o recebimento de respostas, não havendo necessidade identificada de dashboard para o estudante |
| Configuração/parametrização | não | Os parâmetros técnicos da arquitetura são utilizados pela equipe responsável pelo desenvolvimento e pelos experimentos, e não pelo estudante | **[F]** O TCC prevê parâmetros como tamanho de chunks, sobreposição, valor de `k` e modelo gerador como variáveis experimentais |
| Entrada/upload/seleção de dados | não | O estudante precisa fornecer sua dúvida em linguagem natural, mas não há necessidade atual de enviar documentos ou selecionar conjuntos de dados | **[F]** O fluxo previsto no TCC utiliza uma base documental previamente construída e perguntas em linguagem natural como entrada do usuário |
| Acompanhamento de processamento | talvez | Informar ao estudante que sua pergunta está sendo processada enquanto o sistema recupera informações e gera a resposta | **[H]** Ainda não sabemos se o tempo de espera será suficiente para exigir feedback adicional de processamento. O TCC prevê registrar o tempo de resposta do sistema |
| Relatório/resultados | não | O estudante precisa compreender uma resposta para uma dúvida específica, e não analisar relatórios ou resultados agregados | **[F]** O objetivo principal da interface previsto no TCC é a consulta de informações acadêmicas e administrativas |
| Histórico com busca/filtros | talvez | Permitir ao estudante recuperar perguntas ou respostas realizadas anteriormente | **[H] H15 —** Um histórico de conversas anteriores pode ser útil para retomar informações ou consultas, mas essa necessidade ainda precisa ser investigada |
| Comparação de resultados | não | Não foi identificada uma tarefa do estudante que exija comparar diferentes respostas ou configurações técnicas do sistema | **[F]** A comparação entre configurações e modelos pertence à avaliação experimental do TCC, e não ao fluxo do usuário final |
| Explicabilidade/detalhamento | sim | Permitir que o estudante identifique a origem da informação e compreenda em que evidências institucionais a resposta está fundamentada | **[F]** O TCC prevê a preservação dos metadados e das fontes utilizadas. **[H] H02 e H14 —** A apresentação dessas fontes poderá influenciar a confiança e a utilidade percebida da resposta |
| Administração/configurações globais | não | Não existe, no recorte atual de IHC, uma atividade do estudante que envolva administrar o funcionamento global do assistente | **[F]** O usuário priorizado para IHC é o estudante da FEI |
| Usuários/perfis/permissões | não | O recorte atual não exige que o estudante gerencie usuários, perfis ou permissões | **[F]** O TCC não prevê integração com dados acadêmicos individualizados ou sistemas internos sensíveis |
| CRUD de entidade do domínio | não | O estudante não precisa cadastrar, editar ou excluir documentos, normas ou outras entidades da base institucional | **[F]** A construção e manutenção da base documental fazem parte do funcionamento técnico do sistema, não da tarefa principal do usuário |
| Auditoria/logs | não | Os registros técnicos são necessários para avaliação do sistema, mas não correspondem a uma tarefa identificada para o estudante | **[F]** O TCC prevê logs e registros das execuções para análise experimental, incluindo trechos recuperados, configurações e tempo de resposta |
| Alertas/ocorrências | não | Não foi identificada até o momento uma necessidade de o sistema enviar notificações ou alertas ao estudante | **[?]** Essa necessidade ainda não foi observada no escopo atual e poderá ser reconsiderada caso surjam evidências nas próximas entregas |
| Ajuda/documentação | talvez | Auxiliar o estudante a compreender o escopo do assistente, suas limitações e como formular ou reformular uma consulta | **[H] H16 —** Respostas ou interpretações incorretas podem gerar consequências relevantes, tornando importante investigar como comunicar adequadamente as limitações do sistema |
| Interface conversacional | sim | Permitir que o estudante formule uma dúvida acadêmica ou administrativa em linguagem natural e receba uma resposta contextualizada | **[F]** A interface conversacional já faz parte do protótipo previsto no TCC. **[H] H18 e H21 —** O padrão de interação utilizado por assistentes conversacionais pode ser familiar aos estudantes |
| Tratamento de ausência de evidência | sim | Permitir que o estudante compreenda quando o assistente não possui informações suficientes para responder e evite utilizar uma resposta sem fundamento | **[F]** O TCC determina que o sistema deverá reconhecer situações sem evidência documental suficiente. **[H] H10 e H16 —** Erros de interpretação ou respostas incorretas podem produzir consequências para o estudante |

> As possibilidades classificadas como **talvez** deverão ser investigadas nas próximas etapas antes de serem incorporadas à interface. As possibilidades classificadas como **não** poderão ser reconsideradas caso novas necessidades ou evidências sejam identificadas.

---

# 9. Benefícios e ações iniciais

## 9.1 Qual benefício concreto o projeto de IHC pretende oferecer?

| Benefício esperado | Problema/necessidade | Usuário | Status/evidência |
|---|---|---|---|
| Facilitar o acesso a informações acadêmicas e administrativas por meio de um ponto de consulta mais centralizado | Informações podem estar distribuídas entre diferentes páginas, documentos e canais, aumentando o esforço necessário para localização | Estudante da FEI | **[H] H01, H08 e H20 —** A necessidade e o benefício da centralização ainda deverão ser investigados diretamente com estudantes |
| Facilitar a compreensão de regras, prazos, serviços e procedimentos acadêmico-administrativos | Determinadas informações podem exigir interpretação e conhecimento prévio sobre onde procurar ou como compreender a orientação apresentada | Estudante da FEI | **[H] H04 e H09 —** A dificuldade de interpretação e as necessidades dos estudantes ainda precisam ser validadas |
| Permitir que o estudante identifique a origem institucional das informações utilizadas na resposta | Uma resposta gerada por IA pode gerar dúvidas quanto à sua origem ou confiabilidade | Estudante da FEI | **[F]** O TCC prevê preservação e rastreabilidade das fontes. **[H] H02 e H14 —** O impacto da apresentação das fontes sobre a confiança ainda precisa ser investigado |
| Comunicar de forma clara situações em que o assistente não possui evidência suficiente para responder | Uma resposta incorreta ou sem fundamento pode levar a interpretações ou decisões inadequadas | Estudante da FEI | **[F]** O TCC prevê que o sistema reconheça a ausência de evidência suficiente. **[H] H10 e H16 —** As consequências e a melhor forma de comunicar essa limitação ainda deverão ser investigadas |

## 9.2 Que ações o usuário deverá conseguir realizar?

| ID | O usuário precisa conseguir... | Para alcançar... | Prioridade inicial |
|---|---|---|---|
| T01 | Formular uma dúvida acadêmica ou administrativa em linguagem natural | Localizar uma informação relacionada à sua vida acadêmica sem precisar conhecer previamente onde ela está disponível | alta |
| T02 | Ler e compreender a resposta apresentada pelo assistente | Esclarecer sua dúvida, compreender uma informação ou decidir como realizar determinado procedimento | alta |
| T03 | Identificar e consultar a fonte institucional associada à resposta | Verificar a origem da informação e compreender em que evidência a resposta está fundamentada | alta |
| T04 | Fazer uma nova pergunta ou complementar uma pergunta anterior | Refinar a consulta ou esclarecer pontos que permaneceram incompletos | média |
| T05 | Compreender quando o assistente não possui evidência suficiente para responder | Evitar utilizar uma resposta sem fundamento e identificar a necessidade de procurar outra fonte ou canal institucional | alta |
| T06 | Consultar perguntas e respostas anteriores | Retomar informações apresentadas durante uma interação anterior | média |

> Os identificadores `T01`, `T02` etc. são utilizados por representarem **tarefas do usuário**. Posteriormente, esses IDs poderão ser relacionados aos cenários, modelos de tarefas, MoLIC, telas e testes na matriz de rastreabilidade.

## 9.3 Tecnologias/restrições já definidas no TCC

A tecnologia aparece **agora**, depois do entendimento do uso.

| Tecnologia/restrição | Por que existe | Possível impacto na interação |
|---|---|---|
| Arquitetura baseada em RAG | Permitir que as respostas sejam geradas a partir de informações recuperadas de documentos institucionais | A qualidade da resposta dependerá das evidências recuperadas. Quando não houver evidência suficiente, a interface deverá comunicar essa limitação |
| Base documental composta por fontes públicas ou autorizadas da FEI | Garantir que as respostas sejam fundamentadas em conteúdos institucionais identificáveis e adequados ao escopo do projeto | O assistente somente poderá responder adequadamente sobre assuntos contemplados pela base documental |
| Preservação de metadados e fontes dos documentos | Manter rastreabilidade entre os trechos recuperados e os documentos institucionais de origem | Permite apresentar ao estudante a origem das informações utilizadas na resposta |
| Modelos de linguagem acessados por API externa | Realizar a geração das respostas em linguagem natural | Pode introduzir tempo de espera, indisponibilidade do serviço ou erros de comunicação, exigindo feedback adequado durante a interação |
| Banco vetorial e recuperação semântica | Localizar trechos documentais relacionados semanticamente à pergunta do estudante | Uma recuperação inadequada poderá produzir contexto insuficiente ou pouco relevante, devendo o sistema evitar apresentar respostas sem fundamento |
| Ausência de integração com dados acadêmicos pessoais ou sistemas internos sensíveis | Limitar o protótipo a documentos públicos ou autorizados e evitar o tratamento de dados pessoais dos estudantes | O assistente não poderá responder perguntas que dependam de informações individuais, como situação financeira pessoal, notas específicas ou dados particulares do estudante |
| Escopo restrito a dúvidas acadêmicas e administrativas contempladas pela base documental | Manter o protótipo dentro dos limites definidos para o TCC | A interface deverá tornar compreensível o escopo do assistente e tratar adequadamente perguntas que estejam fora dele |
| Registro do tempo de resposta e das execuções | Permitir a avaliação experimental de desempenho, recuperação e geração das respostas | Tempos maiores de processamento poderão exigir indicadores de carregamento ou outro tipo de feedback ao usuário |
| Histórico de interação durante a sessão | Manter o contexto das perguntas e respostas realizadas pelo estudante | Pode permitir continuidade da conversa e consulta a mensagens anteriores, embora a utilidade desse recurso ainda precise ser validada com usuários |
| Respostas não substituem os canais oficiais da instituição | O protótipo possui caráter acadêmico e pode apresentar limitações ou informações insuficientes | A interface deverá comunicar que informações relevantes podem precisar ser verificadas nos canais oficiais da FEI |

---
# 10. Hipóteses e dúvidas prioritárias

A partir das hipóteses levantadas ao longo da Entrega 1, foram priorizadas aquelas que possuem maior impacto sobre a definição do problema, do usuário, das tarefas e das decisões futuras de interface.

| ID | Hipótese/dúvida | Por que importa | Como poderá ser investigada |
|---|---|---|---|
| H04 | O estudante busca obter e compreender informações acadêmicas ou administrativas para resolver dúvidas, tomar decisões ou realizar corretamente procedimentos relacionados à vida acadêmica | Define o objetivo principal do usuário e orienta quais tarefas deverão ser priorizadas na interface | Entrega 2 — investigação com estudantes da FEI |
| H05 | Localizar e compreender informações acadêmicas ou administrativas é uma das atividades mais frequentes dos estudantes nesse contexto | Ajuda a verificar se A01 deve realmente ser considerada a atividade principal do projeto de IHC | Entrega 2 — entrevistas, questionários ou levantamento com estudantes |
| H06 | Compreender e realizar procedimentos acadêmicos ou administrativos é uma atividade de maior criticidade quando envolve regras, etapas obrigatórias ou prazos | A criticidade da atividade pode exigir maior cuidado na apresentação das respostas, fontes, limitações e orientações | Entrega 2 — investigação com estudantes e, quando pertinente, setores responsáveis |
| H08 | A distribuição das informações entre diferentes páginas, documentos e canais pode aumentar o esforço necessário para o estudante resolver uma dúvida | Representa um dos principais problemas que justificam o fluxo de consulta centralizado proposto para o assistente | Entrega 2 — investigação do processo atual com estudantes |
| H14 | A confiabilidade percebida pelo estudante poderá ser influenciada pela clareza sobre a origem institucional das informações apresentadas | Pode justificar a apresentação das fontes e determinar como essas informações deverão aparecer na interface | Entrega 2 — investigação com usuários; Entrega 7 — avaliação da interface |
| H15 | Um histórico de conversas anteriores pode ser útil para o estudante retomar informações ou consultas realizadas anteriormente | O TCC prevê histórico de interação, mas ainda é necessário verificar se essa funcionalidade representa uma necessidade real do usuário | Entrega 2 — investigação com estudantes; Entrega 7 — teste de usabilidade |
| H16 | Uma resposta incorreta ou uma interpretação equivocada sobre regras, prazos ou procedimentos pode produzir consequências relevantes para o estudante | Influencia diretamente o tratamento de erros, ausência de evidência, avisos e encaminhamento para canais oficiais | Entrega 2 — investigação com estudantes e setores responsáveis; Entrega 7 — avaliação da interação |
| H18 | O padrão de interação utilizado por assistentes como ChatGPT, Gemini e Copilot pode ser familiar aos estudantes da FEI | Pode sustentar ou questionar a escolha de uma interface conversacional como principal forma de interação | Entrega 2 — investigação com estudantes e análise de interfaces existentes |

> Essas hipóteses deverão ser registradas e acompanhadas em [`../RASTREABILIDADE.md`](../RASTREABILIDADE.md). Caso alguma delas seja sustentada, refinada ou refutada nas próximas entregas, o histórico deverá ser preservado.

---

# 11. Síntese da equipe

| Pergunta | Síntese atual |
|---|---|
| Qual é a contribuição central do TCC? | Recuperar informações relevantes de uma base documental institucional e utilizá-las como evidência para gerar respostas em linguagem natural a dúvidas acadêmicas e administrativas, além de avaliar experimentalmente o desempenho da arquitetura utilizada |
| O TCC já previa interface? | Sim. O TCC prevê uma interface na qual o estudante envia perguntas em linguagem natural e recebe respostas fundamentadas nas informações institucionais recuperadas pelo sistema |
| Quem é o usuário prioritário de IHC? | Estudante da FEI que necessita localizar ou compreender uma informação acadêmica ou administrativa |
| O que ele precisa alcançar? | Obter e compreender uma informação acadêmica ou administrativa para resolver uma dúvida, tomar uma decisão ou realizar corretamente um procedimento relacionado à vida acadêmica |
| Qual problema/atividade será estudado? | O processo de localizar e compreender informações acadêmicas ou administrativas, especialmente quando essas informações estão distribuídas entre diferentes páginas, documentos ou canais e quando envolvem regras, prazos ou procedimentos |
| Como isso acontece hoje? | As informações podem ser buscadas em páginas institucionais, documentos e regulamentos, sistemas acadêmicos ou por meio de contato com pessoas e setores responsáveis. A frequência e a ordem de utilização desses canais ainda precisam ser investigadas diretamente com estudantes |
| Qual é o contexto de uso? | Situações em que o estudante precisa esclarecer uma dúvida acadêmica ou administrativa, dentro ou fora da FEI, possivelmente utilizando computador, notebook ou dispositivo móvel |
| Que interface/recorte será explorado? | O fluxo conversacional de consulta, envolvendo a formulação de uma pergunta em linguagem natural, apresentação e compreensão da resposta, identificação das fontes utilizadas e comunicação de situações em que não exista evidência suficiente |
| Como a interface se relaciona ao TCC? | A interface já faz parte do protótipo previsto no TCC. A disciplina de IHC aprofundará aspectos relacionados à interação, compreensão das respostas, apresentação das fontes, tratamento de limitações e usabilidade |
| Quais pontos ainda são hipóteses? | Principalmente H04, H05, H06, H08, H14, H15, H16 e H18, relacionados ao objetivo real do estudante, frequência e criticidade das atividades, esforço no processo atual, confiança nas fontes, utilidade do histórico, consequências de erros e familiaridade com interfaces conversacionais |

### Delimitação

**Dentro do escopo de IHC:**

- interação do estudante com o assistente virtual;
- formulação de dúvidas acadêmicas e administrativas em linguagem natural;
- apresentação e compreensão das respostas;
- apresentação das fontes institucionais utilizadas;
- tratamento de perguntas sem evidência suficiente ou fora do escopo;
- continuidade da conversa e possível utilização de histórico;
- comunicação das limitações do assistente;
- investigação dos padrões de interação e vocabulário mais adequados ao estudante;
- avaliação da usabilidade e da compreensão da interface.

**Fora do escopo de IHC:**

- configuração dos parâmetros experimentais de RAG pelo estudante;
- administração do banco vetorial;
- gerenciamento técnico da base documental;
- configuração de modelos de linguagem, embeddings, tamanho de chunks ou valor de `k`;
- dashboards de métricas experimentais destinados à equipe de desenvolvimento;
- gerenciamento de usuários, perfis e permissões;
- integração da interface com dados acadêmicos pessoais ou sistemas internos sensíveis da FEI;
- desenvolvimento de funcionalidades administrativas sem uma necessidade de usuário identificada.

**Dentro do escopo formal do TCC:**

- desenvolvimento do protótipo funcional do assistente virtual;
- interface para envio de perguntas e apresentação das respostas;
- construção e processamento da base documental institucional;
- recuperação semântica de informações;
- geração de respostas fundamentadas em evidências;
- preservação e registro das fontes utilizadas;
- tratamento de perguntas sem evidência suficiente;
- avaliação experimental das configurações de segmentação e recuperação;
- avaliação da qualidade das respostas;
- análise de tempo de resposta, custo e limitações da solução.

**Interface da disciplina será implementada no TCC?** não definido — o TCC já prevê uma interface funcional para interação com o assistente, porém a incorporação das decisões, fluxos e refinamentos produzidos especificamente na disciplina de IHC dependerá dos resultados das próximas entregas e de decisão posterior da equipe em conjunto com o orientador.

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

1. **Problema/atividade humana:** Estudantes da FEI precisam localizar e compreender informações acadêmicas e administrativas relacionadas a regras, prazos, serviços e procedimentos, atualmente disponíveis em diferentes fontes e canais institucionais.

2. **Contribuição técnica do TCC:** O TCC desenvolve e avalia um assistente virtual capaz de recuperar informações de documentos institucionais e utilizá-las como evidência para gerar respostas em linguagem natural a dúvidas acadêmicas e administrativas.

3. **Como uma pessoa poderia utilizar essa contribuição:** O estudante poderá formular sua dúvida por meio de uma interface conversacional, receber uma resposta fundamentada em informações institucionais e consultar as fontes utilizadas pelo assistente.

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
