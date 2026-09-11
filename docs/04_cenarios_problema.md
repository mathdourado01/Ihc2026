# Entrega 4 — Cenários de análise/problema

**Data:** 11/09/2026
**Status:** 🟨 em andamento 
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
> Repita para C02, C03... com autoria individual.

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
