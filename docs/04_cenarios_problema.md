# Entrega 4 — Cenários de análise/problema

**Data inicial:** 16/09/2026  
**Última atualização:** 03/10/2026  
**Status:** 🟦 revisada após feedback  
**Responsabilidade:** 1 solução completa por integrante

## Objetivo da atividade

Descrever situações atuais em que o usuário tenta alcançar um objetivo e encontra dificuldades. O cenário de análise/problema deve tornar visível **o contexto, os atores, as ações, os acontecimentos e as rupturas**, sem antecipar a interface que será projetada.

> **Regra central:** cenário de problema é a “história do problema”. Se o texto já diz “o sistema mostra”, “o aplicativo resolve” ou descreve botões/telas futuras, provavelmente está misturando problema com solução.

Sempre que possível, o cenário deve aprofundar uma **situação concreta já registrada na Entrega 1**.

### Quando o TCC não possuía interface

O cenário continua sendo uma história de **problema/atividade humana**, não uma história do futuro sistema. Descreva como a pessoa realiza hoje uma atividade semelhante ou como lida atualmente com dados, resultados, configurações, logs, decisões e limitações que o tema do TCC pretende apoiar.

Exemplo: em vez de “o DBA abre o novo dashboard e executa o algoritmo”, descreva “o DBA precisa investigar uma consulta lenta, reúne informações em ferramentas distintas, compara planos manualmente e tem dificuldade para estimar o impacto de uma mudança”.

A interface da disciplina aparecerá somente depois, nos cenários de interação.

Se o integrante escolher um novo problema/situação, explique por que ele passou a ser relevante e indique a evidência que motivou sua inclusão.

---

## Cenário C01 — Localização e compreensão de uma informação acadêmica

**Autor(a):** Matheus Dourado Valle — 22.224.023-6  
**Persona(s) relacionada(s):** P01 — Lucas Almeida  
**Necessidade relacionada:** R01, com relação complementar a R02  
**Situação concreta da Entrega 1 relacionada:** A01 — localizar e compreender uma informação acadêmica ou administrativa; H04, H08 e H09  
**Hipóteses ainda presentes:** H04, H08, H09 e H14

### 1. Cenário inicial

Lucas Almeida é estudante da FEI e está organizando sua rotina do semestre. Em determinado momento, ele percebe que precisa confirmar uma orientação acadêmica antes de decidir se fará uma alteração em sua matrícula naquele período.

Ele sabe que a informação deve estar em algum canal institucional, mas não lembra exatamente onde. Como está no campus, durante um intervalo entre atividades, tenta resolver a dúvida naquele momento para decidir como vai se organizar.

Lucas inicia a busca pelos recursos que já conhece, como Portal do Aluno, páginas institucionais e documentos acadêmicos. Quando encontra um conteúdo relacionado ao assunto, ainda precisa interpretar a orientação e entender se ela realmente se aplica à sua situação.

A atividade se torna mais difícil quando a informação aparece distribuída entre lugares diferentes, quando um documento usa uma expressão diferente da outra página ou quando o texto não deixa claro se a orientação vale para o caso que ele está tentando resolver. Se permanece em dúvida, Lucas tende a procurar outra fonte ou recorrer a outra pessoa para confirmar a interpretação.

### 2. Questões de refinamento

Use os tipos de questões/taxonomia definidos na aula. As perguntas devem revelar informações **ainda ausentes** do cenário, não repetir o que já foi respondido.

| # | Questão | Por que precisa ser respondida | Fonte/forma de obter resposta |
|---|---|---|---|
| Q1 | **[Contexto/ambiente]** Em que situação concreta Lucas percebe a necessidade de buscar essa informação naquele momento? | Permite entender a circunstância prática que dá início à atividade. | Entrevista com estudantes e reconstrução de episódios reais. |
| Q2 | **[Objetivo]** O que exatamente Lucas precisa descobrir para poder tomar sua decisão? | Permite delimitar melhor a dúvida e o critério de resolução do problema. | Entrevista com estudantes e análise de situações reais de consulta. |
| Q3 | **[Planejamento]** Qual canal Lucas escolhe consultar primeiro e por quê? | Permite compreender como ele inicia a busca e qual raciocínio utiliza. | Entrevista e observação de tarefa. |
| Q4 | **[Ação]** O que Lucas faz quando encontra informação parcial ou distribuída em mais de uma fonte? | Permite identificar o comportamento observável durante a busca. | Observação de tarefa e protocolo think-aloud. |
| Q5 | **[Evento]** Que acontecimento faz Lucas perceber que a primeira tentativa não foi suficiente? | Permite identificar a ruptura que altera o curso da atividade. | Entrevista e observação. |
| Q6 | **[Atores]** Quem Lucas procura quando decide que não conseguirá resolver a dúvida sozinho? | Permite identificar o papel de outras pessoas no processo atual. | Entrevista com estudantes e profissionais de atendimento. |
| Q7 | **[Avaliação]** Como Lucas reconhece que já compreendeu a orientação de forma suficiente para agir? | Permite identificar o critério de sucesso da atividade pela perspectiva do usuário. | Entrevista e observação de usuários. |

### 3. Cenário refinado

Lucas Almeida é estudante da FEI e está tentando decidir se fará uma alteração em sua matrícula naquele período do semestre. Para tomar essa decisão, ele precisa confirmar se a orientação institucional que encontrou sobre o tema realmente se aplica à sua situação.

**[NOVO — H/Q1]** A necessidade surge durante um intervalo entre atividades no campus, quando Lucas percebe que precisa resolver aquela dúvida naquele mesmo dia para decidir se mantém sua organização atual do semestre ou se busca outra alternativa.

**[NOVO — H/Q2]** O que ele precisa descobrir não é apenas “alguma informação sobre matrícula”, mas especificamente se a orientação encontrada permite entender qual ação acadêmica é possível no período atual e se aquela regra vale para o caso que ele está vivendo.

**[NOVO — H/Q3]** Como associa procedimentos acadêmicos ao ambiente onde costuma acompanhar sua vida acadêmica, Lucas decide começar pelo Portal do Aluno. Ele escolhe esse caminho primeiro porque espera encontrar ali um atalho ou referência mais direta para o tipo de decisão que precisa tomar.

Ao procurar, Lucas encontra uma referência relacionada ao tema, mas percebe que a informação não está toda no mesmo lugar. Uma página indica o nome do procedimento, enquanto outra apresenta datas ou orientações mais gerais.

**[NOVO — H/Q4]** Para tentar compreender o assunto, ele alterna entre páginas, abre um documento institucional relacionado e compara os termos usados em cada fonte para verificar se estão tratando exatamente da mesma orientação.

**[NOVO — H/Q5]** A mudança de estratégia acontece quando Lucas encontra um conteúdo que parece relevante, mas não deixa claro se a regra vale para a situação dele. Além disso, uma das fontes utiliza uma expressão institucional diferente daquela que ele tinha usado inicialmente na busca, o que aumenta sua dúvida sobre estar consultando o conteúdo certo.

Nesse momento, Lucas já não considera suficiente continuar apenas relendo os mesmos materiais.

**[NOVO — H/Q6]** Como próximo passo, ele procura primeiro um colega que possa já ter passado por situação semelhante. Se ainda assim a interpretação continuar insegura, considera recorrer a um canal institucional de atendimento para confirmar o entendimento.

**[NOVO — H/Q7]** Lucas entende que a atividade foi concluída com sucesso quando consegue explicar para si mesmo qual orientação se aplica ao seu caso, qual fonte institucional sustenta essa interpretação e o que ele deve fazer a seguir com base nisso. Se esse nível de compreensão não é alcançado, a dúvida continua aberta e a decisão fica adiada.

### 4. Elementos extraídos

| Elemento | Evidência no cenário |
|---|---|
| Ator(es) | Lucas Almeida; colega consultado posteriormente; possível canal institucional de atendimento. |
| Objetivo(s) | Confirmar uma orientação acadêmica para decidir se realiza ou não uma alteração relacionada à matrícula no semestre. |
| Contexto | Intervalo entre atividades, no campus, com necessidade de resolver uma dúvida naquele mesmo dia para seguir com sua organização acadêmica. |
| Recursos/informações | Portal do Aluno, páginas institucionais, documentos acadêmicos e orientações relacionadas ao procedimento. |
| Planejamento | Começar pelo Portal do Aluno por associá-lo aos procedimentos acadêmicos e, em seguida, ampliar a busca para outras fontes institucionais. |
| Ações | Procurar informações, abrir páginas, ler, alternar entre fontes, comparar termos e eventualmente procurar outra pessoa. |
| Evento(s) | A primeira fonte encontrada não deixa claro se a orientação se aplica ao caso de Lucas; uma segunda fonte usa terminologia diferente, provocando nova dúvida. |
| Avaliação | Lucas considera a atividade resolvida quando entende o que a orientação significa, sabe se ela vale para seu caso e reconhece a fonte institucional que sustenta essa interpretação. |
| Problemas/rupturas | Informação distribuída; termos diferentes entre fontes; dificuldade para saber se a orientação vale para o caso concreto. |
| Consequências | Maior tempo e esforço, manutenção da dúvida, necessidade de recorrer a outra pessoa ou adiamento da decisão. |

### 5. Implicações para as próximas entregas

Quais tarefas merecem análise? Quais informações precisam ser coletadas? **Não desenhe a solução ainda.**

Este cenário indica que as próximas etapas devem analisar com maior profundidade a tarefa de **localizar e compreender uma informação acadêmica ou administrativa**, especialmente quando o estudante não sabe em qual canal a informação está disponível e precisa relacionar conteúdos provenientes de mais de uma fonte.

Devem ser investigados principalmente:

- o ponto de partida mais comum da busca;
- os critérios usados para escolher uma nova fonte quando a primeira tentativa falha;
- o papel da terminologia institucional na dificuldade de compreensão;
- os critérios pelos quais o estudante decide que a informação já é suficiente para agir;
- o momento em que a busca autônoma é interrompida e substituída por procura de ajuda.

Nenhuma solução de interface é definida neste momento.

---

## Cenário C02 — Compreensão do processo de ingresso em um programa de mestrado

**Autor(a):** João Pedro Sabino Garcia — 22.224.032-7  
**Persona(s) relacionada(s):** P02 — Mariana Costa  
**Necessidade relacionada:** R03, com relação complementar a R01 e R02  
**Situação concreta da Entrega 1 relacionada:** A02 — compreender um procedimento acadêmico ou administrativo; H06, H09 e H10  
**Hipóteses ainda presentes:** H06, H09, H10, H14 e H16

### 1. Cenário inicial

Mariana Costa é estudante da FEI e está considerando ingressar em um programa de mestrado da instituição. Antes de decidir se seguirá por esse caminho, ela precisa entender como funciona o processo de ingresso e quais informações são relevantes para sua situação.

Sua dificuldade não é apenas “encontrar o site do programa”, mas compreender o procedimento de forma suficiente para decidir se consegue ou não se planejar para participar do processo. Isso envolve relacionar informações como requisitos, etapas, documentos e orientações institucionais.

Como essas informações podem estar distribuídas em páginas e documentos diferentes, Mariana precisa reunir o material, interpretar os conteúdos e verificar o que realmente se aplica ao seu caso. Quando isso não acontece, permanece a insegurança sobre como prosseguir.

### 2. Questões de refinamento

Use os tipos de questões/taxonomia definidos na aula. As perguntas devem revelar informações **ainda ausentes** do cenário, não repetir o que já foi respondido.

| # | Questão | Por que precisa ser respondida | Fonte/forma de obter resposta |
|---|---|---|---|
| Q1 | **[Contexto/ambiente]** O que leva Mariana a procurar essas informações neste momento, e não em outro? | Permite entender a situação concreta que inicia a atividade. | Entrevista com estudantes interessados em pós-graduação. |
| Q2 | **[Objetivo]** Qual dúvida específica impede Mariana de decidir como prosseguir? | Permite delimitar o problema de compreensão dentro do procedimento. | Entrevista e reconstrução de episódios. |
| Q3 | **[Planejamento]** Qual canal Mariana escolhe consultar primeiro e por quê? | Permite entender o ponto de partida da atividade e o raciocínio inicial. | Entrevista e observação de tarefa. |
| Q4 | **[Ação]** Como Mariana organiza a consulta quando percebe que precisa relacionar diferentes páginas ou documentos? | Permite identificar o comportamento observável durante a atividade. | Observação, think-aloud e entrevista. |
| Q5 | **[Evento]** O que acontece durante a consulta que faz Mariana perceber que ainda não compreendeu o procedimento? | Permite identificar a ruptura que altera a atividade. | Entrevista e observação. |
| Q6 | **[Atores]** Quem Mariana procura quando conclui que não conseguirá esclarecer a dúvida sozinha? | Permite entender o papel de outras pessoas ou setores no processo atual. | Entrevista com estudantes e profissionais da instituição. |
| Q7 | **[Avaliação]** Como Mariana reconhece que já compreendeu o procedimento de forma suficiente para decidir seus próximos passos? | Permite identificar o critério de sucesso da atividade pela perspectiva do usuário. | Entrevista e observação. |
| Q8 | **[Consequência]** O que pode acontecer se Mariana interpretar incorretamente uma etapa, requisito ou condição do processo? | Permite compreender o impacto de uma interpretação incompleta ou incorreta. | Entrevista com estudantes e profissionais responsáveis. |

### 3. Cenário refinado

Mariana Costa é estudante da FEI e está avaliando a possibilidade de ingressar em um programa de mestrado da instituição. Ela decide procurar informações agora porque percebe que, se quiser considerar seriamente essa possibilidade, precisa entender o processo com antecedência suficiente para se planejar.

**[NOVO — H/Q1]** A busca acontece em um momento em que Mariana já considera essa opção de continuidade acadêmica como algo real, e não apenas uma curiosidade distante. Por isso, a atividade tem peso direto sobre uma decisão pessoal e acadêmica.

**[NOVO — H/Q2]** A dúvida que impede Mariana de decidir como prosseguir não é genérica: ela precisa entender quais etapas compõem o processo de ingresso, quais requisitos precisam ser observados e se as condições apresentadas nas fontes institucionais se encaixam na situação em que ela se encontra.

Para começar, Mariana utiliza um canal institucional que associa diretamente ao tema da pós-graduação.

**[NOVO — H/Q3]** Seu ponto de partida é a página institucional relacionada ao programa ou à pós-graduação, porque ela espera encontrar ali a referência oficial mais direta para entender o processo. A partir daí, acessa outras páginas e documentos indicados nesse percurso.

Ao avançar na consulta, Mariana percebe que a compreensão do procedimento não depende de uma única leitura.

**[NOVO — H/Q4]** Ela alterna entre a página do programa, documentos com orientações do processo e outras referências institucionais, tentando relacionar etapas, requisitos e documentos. Para não perder o fio da atividade, passa a anotar o que cada fonte parece esclarecer e o que ainda permanece incerto.

**[NOVO — H/Q5]** A ruptura ocorre quando Mariana encontra informações que parecem se referir ao mesmo processo, mas não respondem de forma suficientemente clara à sua situação. Um documento pode detalhar etapas, enquanto outra página usa terminologia diferente ou não deixa evidente como determinada condição deve ser interpretada. Nesse momento, ela percebe que encontrou material relevante, mas ainda não compreensão suficiente.

Depois de comparar os conteúdos e continuar insegura, Mariana entende que a busca autônoma chegou a um limite.

**[NOVO — H/Q6]** O próximo passo passa a ser procurar alguém que possa ajudá-la a interpretar corretamente o procedimento, como um professor, um profissional do setor responsável ou outro canal institucional de esclarecimento.

**[NOVO — H/Q7]** Mariana considera a atividade satisfatoriamente concluída quando consegue descrever, com segurança razoável, quais são as etapas do processo, quais informações importam para sua situação, quais documentos ou requisitos precisa considerar e qual fonte institucional sustenta essa compreensão.

Se isso não acontece, a incerteza permanece.

**[NOVO — H/Q8]** Uma interpretação incorreta pode levar Mariana a planejar seus próximos passos com base em uma compreensão inadequada, deixar de considerar alguma condição importante ou adiar uma decisão por insegurança. Dependendo do tipo de erro, ela também pode perder tempo seguindo um caminho que não corresponde ao que realmente precisava entender.

### 4. Elementos extraídos

| Elemento | Evidência no cenário |
|---|---|
| Ator(es) | Mariana Costa; professor, profissional ou setor institucional procurado posteriormente. |
| Objetivo(s) | Compreender o processo de ingresso em um programa de mestrado para decidir se e como pretende prosseguir. |
| Contexto | Momento em que a possibilidade de continuar os estudos passa a exigir planejamento real. |
| Recursos/informações | Página institucional da pós-graduação ou do programa, documentos e orientações sobre processo, requisitos e etapas. |
| Planejamento | Começar por uma referência institucional diretamente associada à pós-graduação e, a partir dela, abrir os materiais relacionados. |
| Ações | Procurar informações, abrir páginas, ler, alternar entre documentos, anotar, comparar conteúdos e buscar esclarecimentos. |
| Evento(s) | Mariana encontra materiais relevantes, mas ainda insuficientes para esclarecer sua situação; surgem diferenças de terminologia ou lacunas de aplicabilidade. |
| Avaliação | Ela considera o problema resolvido quando consegue explicar as etapas, requisitos e implicações relevantes para o seu caso, com base em fontes institucionais reconhecíveis. |
| Problemas/rupturas | Informações distribuídas; necessidade de relacionar diferentes documentos; terminologia institucional; dificuldade para saber se a orientação se aplica à sua situação. |
| Consequências | Insegurança, maior esforço, possível adiamento da decisão ou planejamento baseado em compreensão incompleta. |

### 5. Implicações para as próximas entregas

Quais tarefas merecem análise? Quais informações precisam ser coletadas? **Não desenhe a solução ainda.**

Este cenário indica que as próximas etapas devem analisar com maior profundidade a tarefa de **compreender um procedimento acadêmico ou administrativo**, especialmente quando sua compreensão depende de mais de uma fonte e exige relacionar requisitos, etapas e orientações.

Devem ser investigados principalmente:

- o ponto de partida mais comum da busca por esse tipo de procedimento;
- como o estudante organiza informações provenientes de fontes diferentes;
- quais tipos de conteúdo ou terminologia mais dificultam a compreensão;
- em que momento a pessoa decide que a busca autônoma não é suficiente;
- quais critérios utiliza para avaliar se entendeu o procedimento;
- quais consequências percebe em uma interpretação incorreta.

Nenhuma solução de interface é definida neste momento.

---

## Checklist

- [x] Há um cenário completo por integrante.
- [x] Cada cenário tem título, ator, objetivo, contexto e problema.
- [x] O cenário possui origem rastreável na Entrega 1 ou justifica claramente a inclusão de uma nova situação.
- [x] O texto descreve a situação atual, sem antecipar a solução.
- [x] Para TCC sem interface original, o cenário descreve uma prática humana plausível relacionada à contribuição técnica, e não “a falta de uma tela”.
- [x] Questões de refinamento acrescentam informação nova.
- [x] O refinamento mostra claramente o que foi adicionado/alterado.
- [x] Cenários são diferentes o suficiente para cobrir objetivos/problemas relevantes.
- [x] Cada cenário está ligado a persona/necessidade na matriz de rastreabilidade.

---

## Histórico de revisões

### 03/10/2026 — Revisão após feedback da Entrega 4

- transformação dos cenários em episódios mais concretos e encadeados;
- delimitação mais clara da situação específica enfrentada por Lucas e por Mariana;
- revisão das perguntas de refinamento para garantir cobertura mais efetiva de contexto, atores, objetivos, planejamento, ações, eventos e avaliação;
- substituição de trechos que apenas registravam lacunas por respostas hipotéticas incorporadas à narrativa;
- diferenciação mais clara entre o que a pessoa faz, o que acontece durante a atividade e como interpreta o resultado;
- reforço da distinção entre cenário de problema e solução de interface;
- atualização do checklist e do estado da entrega.
