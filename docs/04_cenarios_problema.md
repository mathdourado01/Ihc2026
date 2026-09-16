# Entrega 4 — Cenários de análise/problema

**Data:** 16/09/2026
**Status:** 🟩 concluída
**Responsabilidade:** 1 solução completa por integrante

## Objetivo da atividade

Descrever situações atuais em que o usuário tenta alcançar um objetivo e encontra dificuldades. O cenário de análise/problema deve tornar visível **o contexto, os atores, as ações e as rupturas**, sem antecipar a interface que será projetada.

> **Regra central:** cenário de problema é a “história do problema”. Se o texto já diz “o sistema mostra”, “o aplicativo resolve” ou descreve botões/telas futuras, provavelmente está misturando problema com solução.

Sempre que possível, o cenário deve aprofundar uma **situação concreta já registrada na Entrega 1**.

### Quando o TCC não possuía interface

O cenário continua sendo uma história de **problema/atividade humana**, não uma história do futuro sistema. Descreva como o profissional realiza hoje uma atividade semelhante ou como lida atualmente com dados, resultados, configurações, logs, decisões e limitações que o tema do TCC pretende apoiar.

Exemplo: em vez de “o DBA abre o novo dashboard e executa o algoritmo”, descreva “o DBA precisa investigar uma consulta lenta, reúne informações em ferramentas distintas, compara planos manualmente e tem dificuldade para estimar o impacto de uma mudança”.

A interface da disciplina aparecerá somente depois, nos cenários de interação.

Se o integrante escolher um novo problema/situação, explique por que ele passou a ser relevante e indique a evidência que motivou sua inclusão.

## Cenário C01 — Localização e compreensão de uma informação acadêmica

**Autor(a):** Matheus Dourado Valle — 22.224.023-6  
**Persona(s) relacionada(s):** P01 — Lucas Almeida  
**Necessidade relacionada:** R01, com relação complementar a R02  
**Situação concreta da Entrega 1 relacionada:** A01 — localizar e compreender uma informação acadêmica ou administrativa; H04, H08 e H09  
**Hipóteses ainda presentes:** H04, H07, H08, H09 e H14

### 1. Cenário inicial

Lucas Almeida é estudante da FEI e precisa compreender uma regra acadêmica antes de tomar uma decisão relacionada à sua rotina no semestre. Ele sabe que a informação provavelmente está disponível em algum canal institucional, mas não sabe exatamente em qual página, documento ou sistema deve procurar.

Lucas começa a procurar a informação nos canais que conhece. Durante a busca, pode ser necessário consultar páginas institucionais, documentos ou sistemas acadêmicos diferentes até localizar algo relacionado à sua dúvida. Ao encontrar a informação, ele ainda precisa interpretar o conteúdo e verificar se aquela orientação realmente se aplica à sua situação.

Alguns conteúdos podem utilizar termos institucionais ou estar inseridos em documentos mais extensos, fazendo com que Lucas tenha dificuldade para identificar rapidamente a parte relevante. Quando ainda permanece em dúvida, ele pode repetir a busca utilizando outros termos, consultar outra fonte ou procurar ajuda de colegas, professores ou profissionais da instituição.

Mesmo quando encontra uma informação relacionada ao assunto, Lucas pode continuar inseguro sobre sua interpretação ou sobre qual fonte deve considerar. Isso aumenta o tempo gasto para resolver uma dúvida que inicialmente parecia simples e pode fazer com que ele adie uma decisão ou recorra a outro canal para confirmar o que encontrou.

### 2. Questões de refinamento

Use os tipos de questões/taxonomia definidos na aula. As perguntas devem revelar informações **ainda ausentes** do cenário, não repetir o que já foi respondido.


| # | Questão | Por que precisa ser respondida | Fonte/forma de obter resposta |
|---|---|---|---|
| Q1 | **[Ambiente/planejamento]** Quais canais institucionais o estudante costuma consultar quando não sabe onde determinada informação está disponível? | Permite compreender como a busca realmente começa e quais recursos fazem parte do contexto atual. | Entrevista com estudantes e observação de uma busca real. |
| Q2 | **[Objetivo]** O que o estudante precisa descobrir para considerar uma dúvida acadêmica realmente resolvida? | Encontrar algum texto relacionado ao assunto pode não ser suficiente; é necessário entender o que dá segurança para agir. | Entrevista com estudantes e análise de situações reais de consulta. |
| Q3 | **[Ação]** O que o estudante faz quando encontra uma página ou documento, mas não compreende completamente a informação? | Permite identificar estratégias utilizadas quando a primeira busca não resolve a dúvida. | Entrevista, observação e protocolo think-aloud. |
| Q4 | **[Avaliação]** Como o estudante decide se a informação encontrada é confiável e aplicável à sua situação? | A origem institucional pode influenciar a confiança, mas essa hipótese ainda precisa ser validada. | Entrevista com estudantes. |
| Q5 | **[Atores/eventos]** Em que momento o estudante deixa de tentar resolver a dúvida sozinho e procura outra pessoa ou setor da instituição? | Permite identificar a ruptura que leva da busca autônoma para um canal humano. | Entrevista com estudantes e profissionais de atendimento. |
| Q6 | **[Planejamento]** Como o estudante escolhe novos termos de busca ou uma nova fonte quando a primeira tentativa falha? | Permite compreender a sequência de ações e as estratégias atualmente utilizadas. | Observação de tarefa e entrevista. |
| Q7 | **[Avaliação]** Como o estudante sabe que já compreendeu a informação suficientemente para tomar sua decisão? | Permite identificar o critério de sucesso da atividade pela perspectiva do usuário. | Entrevista e observação de usuários. |

### 3. Cenário refinado

Lucas Almeida é estudante da FEI e precisa compreender uma regra acadêmica antes de tomar uma decisão relacionada à sua rotina no semestre. Ele sabe que a informação provavelmente existe em algum canal institucional, mas não sabe exatamente onde procurá-la.

**[NOVO — H/Q1]** Entre os recursos atualmente disponíveis estão páginas do site institucional, documentos acadêmicos, Portal do Aluno. A ordem em que esses canais são utilizados pelos estudantes ainda precisa ser investigada.

Lucas inicia uma busca utilizando os recursos que já conhece. Quando encontra uma página ou documento relacionado ao assunto, precisa identificar a parte relevante e interpretar seu conteúdo.

**[NOVO — H/Q2]** Para considerar a dúvida resolvida, não basta apenas encontrar uma referência ao assunto: Lucas precisa compreender o significado da regra, entender se ela se aplica à situação que está vivendo e ter confiança suficiente para utilizar aquela informação em sua decisão.

Quando o conteúdo utiliza termos institucionais que ele não conhece ou exige a leitura de informações distribuídas em diferentes partes de uma página ou documento, Lucas pode não conseguir compreender imediatamente a orientação.

**[NOVO — H/Q3 e Q6]** Nessas situações, ele pode reformular os termos utilizados na busca, consultar outra página ou documento e comparar as informações encontradas. Essas estratégias ainda precisam ser confirmadas com estudantes reais.

**[NOVO — H/Q4]** A origem institucional da informação pode ser um dos elementos utilizados por Lucas para avaliar sua confiabilidade, principalmente quando encontra conteúdos semelhantes em diferentes locais.

Se, mesmo após novas tentativas, a dúvida continuar sem resposta clara, **[NOVO — H/Q5]** Lucas pode recorrer a colegas, professores ou profissionais da instituição para confirmar sua interpretação. Ainda não sabemos quais desses canais são utilizados com maior frequência.

**[NOVO — H/Q7]** A atividade termina satisfatoriamente quando Lucas entende a informação em nível suficiente para tomar a decisão que motivou sua busca e consegue reconhecer qual orientação institucional sustenta essa compreensão. Quando isso não acontece, permanece a incerteza e surge a necessidade de continuar procurando ou recorrer a outra pessoa.

### 4. Elementos extraídos

| Elemento | Evidência no cenário |
|---|---|
| Ator(es) | Lucas Almeida, estudante da FEI; eventualmente colegas, professores ou profissionais da instituição. |
| Objetivo(s) | Localizar e compreender uma regra acadêmica necessária para tomar uma decisão. |
| Contexto | Situação cotidiana da vida acadêmica em que o estudante necessita de uma informação institucional e não sabe previamente onde encontrá-la. |
| Recursos/informações | Páginas institucionais, documentos acadêmicos, Portal do Aluno e outras informações acadêmico-administrativas. |
| Ações | Procurar a informação, abrir páginas e documentos, ler, interpretar, reformular a busca, consultar outras fontes e eventualmente pedir ajuda. |
| Problemas/rupturas | Informação distribuída entre diferentes canais; dificuldade para saber onde procurar; linguagem institucional; dificuldade de identificar qual informação se aplica à situação. |
| Consequências | Maior tempo e esforço para solucionar a dúvida, permanência da incerteza, adiamento da decisão ou necessidade de recorrer a outro canal de atendimento. |

### 5. Implicações para as próximas entregas

Quais tarefas merecem análise? Quais informações precisam ser coletadas? **Não desenhe a solução ainda.**

Este cenário indica que as próximas etapas devem analisar com maior profundidade a tarefa de **localizar e compreender uma informação acadêmica ou administrativa**.

Devem ser investigados principalmente o caminho utilizado pelo estudante para iniciar uma busca, os canais consultados, a forma como ele reformula a procura quando não obtém sucesso, os critérios utilizados para avaliar a confiabilidade e aplicabilidade de uma informação e o momento em que decide recorrer a outra pessoa ou setor.

Também será necessário verificar com estudantes reais se a distribuição das informações entre diferentes fontes representa efetivamente um problema frequente e quais características dos conteúdos institucionais dificultam sua compreensão.

Nenhuma solução de interface é definida neste momento.

## Cenário C02 — Compreensão do processo de ingresso em um programa de mestrado

**Autor(a):** João Pedro Sabino Garcia — 22.224.032-7  
**Persona(s) relacionada(s):** P02 — Mariana Costa  
**Necessidade relacionada:** R03, com relação complementar a R01 e R02  
**Situação concreta da Entrega 1 relacionada:** A02 — compreender um procedimento acadêmico ou administrativo; H06, H09 e H10  
**Hipóteses ainda presentes:** H06, H07, H08, H09, H10, H14 e H16

### 1. Cenário inicial

Mariana Costa é estudante da FEI e considera continuar seus estudos em um programa de mestrado da instituição. Antes de decidir se pretende seguir esse caminho, ela precisa compreender como funciona o processo de ingresso, quais requisitos devem ser observados e quais orientações institucionais são relevantes para sua situação.

Para reunir essas informações, Mariana procura conteúdos nos canais institucionais disponíveis. Durante essa atividade, pode ser necessário consultar mais de uma página ou documento, pois informações sobre o programa, requisitos e processo de ingresso podem aparecer em conteúdos diferentes.

Mariana precisa interpretar o material encontrado e relacionar as diferentes informações para formar uma visão do processo como um todo. Dependendo de como o conteúdo está organizado, ela pode encontrar termos que não conhece, informações muito extensas ou orientações cuja aplicação à sua situação não está imediatamente clara.

Quando uma dúvida permanece, Mariana pode continuar procurando em outras páginas ou documentos e comparar as informações encontradas. Caso ainda não consiga compreender alguma etapa ou requisito, pode precisar procurar outro canal ou uma pessoa da instituição para obter esclarecimentos.

Como a decisão de continuar seus estudos depende da compreensão correta dessas informações, uma interpretação equivocada ou incompleta pode fazer com que Mariana permaneça insegura sobre o processo, planeje seus próximos passos a partir de uma compreensão incorreta ou deixe de considerar alguma condição relevante.

### 2. Questões de refinamento

Use os tipos de questões/taxonomia definidos na aula. As perguntas devem revelar informações **ainda ausentes** do cenário, não repetir o que já foi respondido.

| # | Questão | Por que precisa ser respondida | Fonte/forma de obter resposta |
|---|---|---|---|
| Q1 | **[Objetivo]** Quais informações sobre o processo de ingresso são consideradas essenciais pelo estudante para decidir como prosseguir? | Permite identificar quais partes do processo precisam ser compreendidas e quais informações são prioritárias. | Entrevista com estudantes interessados em pós-graduação e análise dos documentos institucionais. |
| Q2 | **[Ambiente]** Em quais canais o estudante procura inicialmente informações sobre um procedimento que ainda não conhece? | Permite entender o ponto de partida e quais recursos fazem parte do contexto atual. | Entrevista com estudantes e observação de uma tarefa de busca. |
| Q3 | **[Planejamento]** Como o estudante organiza informações encontradas em páginas ou documentos diferentes para construir uma compreensão do procedimento completo? | Permite compreender como o estudante lida com informações distribuídas entre diferentes conteúdos. | Observação, protocolo think-aloud e entrevista. |
| Q4 | **[Ação]** Que tipos de conteúdo ou terminologia produzem maior dificuldade de interpretação? | Permite identificar rupturas concretas durante a leitura e compreensão das orientações institucionais. | Teste exploratório com documentos existentes e entrevista. |
| Q5 | **[Avaliação]** Como o estudante verifica se uma regra ou requisito encontrado realmente se aplica à sua situação? | Uma interpretação equivocada pode influenciar decisões e ações posteriores. | Entrevista com estudantes e consulta ao setor responsável pelo procedimento. |
| Q6 | **[Atores/eventos]** Em que momento o estudante deixa de tentar compreender o procedimento sozinho e procura outra pessoa ou setor da instituição? | Permite identificar a ruptura que leva da busca autônoma para um canal humano. | Entrevista com estudantes e profissionais da instituição. |
| Q7 | **[Avaliação]** Como o estudante sabe que compreendeu o procedimento de forma suficiente para decidir seus próximos passos? | Permite identificar o critério de sucesso da atividade pela perspectiva do usuário. | Entrevista e observação de usuários. |
| Q8 | **[Consequência]** Quais são as possíveis consequências de interpretar incorretamente uma etapa, regra ou requisito? | Permite compreender o impacto que uma interpretação incorreta pode ter sobre as decisões do estudante. | Entrevista com estudantes e profissionais responsáveis pelo procedimento. |

### 3. Cenário refinado

Mariana Costa é estudante da FEI e considera continuar seus estudos em um programa de mestrado da instituição. Antes de tomar uma decisão, ela precisa entender como funciona o processo de ingresso e identificar quais informações são relevantes para sua situação.

**[NOVO — H/Q1]** A busca de Mariana envolve informações sobre o programa, o processo de ingresso, seus requisitos e orientações relacionadas. Outros aspectos considerados essenciais pelos estudantes ainda precisam ser investigados.

Mariana procura essas informações nos canais institucionais disponíveis.

**[NOVO — H/Q2]** Páginas institucionais e documentos acadêmicos fazem parte desse conjunto de fontes, mas ainda não sabemos qual canal estudantes com esse objetivo consultam primeiro nem qual sequência de busca utilizam.

Durante a atividade, Mariana encontra informações relacionadas a diferentes partes de seu objetivo e precisa relacioná-las para compreender o processo como um todo.

**[NOVO — H/Q3]** Quando informações relevantes aparecem em páginas ou documentos diferentes, Mariana pode precisar alternar entre esses materiais e comparar o que encontrou para construir uma compreensão do procedimento. A forma como os estudantes realizam essa organização ainda precisa ser confirmada.

**[NOVO — H/Q4]** Termos institucionais desconhecidos, documentos extensos ou orientações que não deixam evidente sua aplicação à situação da estudante podem aumentar o esforço necessário para compreender o conteúdo. Quais elementos efetivamente produzem maior dificuldade ainda precisam ser identificados com estudantes reais.

Mariana também precisa avaliar se as informações encontradas são adequadas para sua situação.

**[NOVO — H/Q5]** A origem institucional da informação pode contribuir para essa avaliação, mas a forma como os estudantes verificam se determinada regra ou requisito realmente se aplica ao seu caso ainda precisa ser investigada.

Quando as informações encontradas não permitem esclarecer completamente uma dúvida, **[NOVO — H/Q6]** Mariana pode continuar procurando em outras fontes ou recorrer a professores, profissionais ou setores da instituição para confirmar sua interpretação. Ainda não sabemos em que momento os estudantes deixam de tentar resolver esse tipo de dúvida sozinhos.

**[NOVO — H/Q7]** A atividade termina satisfatoriamente quando Mariana consegue formar uma compreensão suficientemente clara do processo para decidir seus próximos passos e consegue reconhecer quais informações institucionais sustentam essa compreensão.

Caso isso não aconteça, permanece a incerteza sobre como prosseguir.

**[NOVO — H/Q8]** Uma interpretação incorreta de etapas, requisitos ou condições pode fazer com que Mariana planeje suas próximas ações com base em uma compreensão inadequada, deixe de considerar alguma exigência relevante ou precise procurar esclarecimentos posteriormente. A frequência e o impacto dessas situações ainda precisam ser verificados com usuários reais.

### 4. Elementos extraídos

| Elemento | Evidência no cenário |
|---|---|
| Ator(es) | Mariana Costa, estudante da FEI; eventualmente professores, profissionais ou setores da instituição responsáveis pelas informações. |
| Objetivo(s) | Compreender o processo de ingresso em um programa de mestrado para decidir seus próximos passos. |
| Contexto | Situação em que uma estudante considera continuar seus estudos na instituição e precisa reunir e compreender informações antes de tomar uma decisão. |
| Recursos/informações | Páginas institucionais, documentos acadêmicos, informações sobre o programa, processo de ingresso, requisitos e orientações relacionadas. |
| Ações | Procurar informações, abrir páginas e documentos, ler, interpretar, comparar diferentes fontes e eventualmente pedir esclarecimentos. |
| Problemas/rupturas | Informações distribuídas entre diferentes conteúdos; dificuldade para relacionar regras e requisitos; terminologia institucional; incerteza sobre a aplicação das informações à situação da estudante. |
| Consequências | Maior tempo e esforço para compreender o procedimento, permanência da incerteza, necessidade de recorrer a outro canal ou tomada de decisão baseada em uma compreensão incompleta ou incorreta. |

### 5. Implicações para as próximas entregas

Quais tarefas merecem análise? Quais informações precisam ser coletadas? **Não desenhe a solução ainda.**

Este cenário indica que as próximas etapas devem analisar com maior profundidade a tarefa de **compreender um procedimento acadêmico ou administrativo**, especialmente quando sua compreensão depende de diferentes regras, requisitos e informações institucionais.

Devem ser investigadas principalmente as estratégias utilizadas pelo estudante para localizar as informações necessárias, relacionar conteúdos provenientes de diferentes fontes, compreender termos institucionais, verificar se determinada orientação se aplica à sua situação e identificar quando ainda existem informações faltantes.

Também será necessário verificar com estudantes reais quais informações sobre procedimentos acadêmicos costumam gerar mais dúvidas, quais critérios são utilizados para avaliar a confiabilidade e aplicabilidade das orientações encontradas e em que circunstâncias o estudante decide procurar outra pessoa ou setor da instituição.

Nenhuma solução de interface é definida neste momento.

## Checklist

- [ ] Há um cenário completo por integrante.
- [ ] Cada cenário tem título, ator, objetivo, contexto e problema.
- [ ] O cenário possui origem rastreável na Entrega 1 ou justifica claramente a inclusão de uma nova situação.
- [ ] O texto descreve a situação atual, sem antecipar a solução.
- [ ] Para TCC sem interface original, o cenário descreve uma prática humana plausível relacionada à contribuição técnica, e não “a falta de uma tela”.
- [ ] Questões de refinamento acrescentam informação nova.
- [ ] O refinamento mostra claramente o que foi adicionado/alterado.
- [ ] Cenários são diferentes o suficiente para cobrir objetivos/problemas relevantes.
- [ ] Cada cenário está ligado a persona/necessidade na matriz de rastreabilidade.
