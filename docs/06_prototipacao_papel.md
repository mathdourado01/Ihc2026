
# Entrega 6 — Prototipação em papel

**Data:** 27/10/2026  
**Status:** 🟨 em andamento  
**Responsabilidade:** 1 solução integrada por equipe

## Objetivo da atividade

Externalizar rapidamente ideias de interação em baixa fidelidade para explorar alternativas antes de investir em detalhes visuais. O valor da atividade está no **ciclo construir → simular → observar → revisar**, não na beleza do desenho.

## 1. Escopo do protótipo

**Personas:** P01 — Lucas Almeida e P02 — Mariana Costa, definidas na Entrega 3.  

**Cenários/tarefas cobertos:** C01 — localização e compreensão de uma informação acadêmica (Lucas); C02 — compreensão do processo de ingresso em um programa de mestrado (Mariana), definidos na Entrega 4. As tarefas abrangem T01 — obter resposta para uma dúvida acadêmica, T02 — formular e enviar uma consulta, T03 — consultar a resposta e verificar as fontes, T04 — realizar uma pergunta complementar e T05 — compreender a ausência de evidências suficientes.

**Objetivos principais:** Permitir que o estudante formule dúvidas acadêmicas ou administrativas em linguagem natural, compreenda as respostas apresentadas pelo assistente virtual, consulte as fontes institucionais utilizadas e continue a conversa quando precisar de esclarecimentos adicionais.

O protótipo representa a interface conversacional do Assistente Virtual da FEI, desenvolvido como parte do TCC da equipe.

O cenário de Lucas prioriza a realização de uma consulta acadêmica e a verificação da fonte utilizada. O cenário de Mariana prioriza a compreensão de informações relacionadas ao ingresso em um programa de mestrado, incluindo etapas, requisitos e orientações disponíveis nas fontes institucionais.

A proposta busca representar as funcionalidades essenciais da interação entre o estudante e o assistente virtual, sem incluir elementos que não estejam diretamente relacionados às tarefas analisadas.

## 1.1 Possíveis famílias de interface

Escolha apenas o que for coerente com tarefas e cenários. Para TCCs técnicos, o protótipo pode explorar:

- **dashboard** para monitoramento e tomada de decisão;
- **configuração/parametrização** para preparar algoritmo/modelo/processo;
- **entrada/seleção de dados** com validação;
- **acompanhamento de execução** com progresso, fila, cancelamento e recuperação;
- **relatório/resultados** com explicação, gráficos e exportação;
- **histórico** com busca, filtros, ordenação e detalhes;
- **comparação** entre execuções, versões, algoritmos ou períodos;
- **administração** de usuários, papéis, permissões ou entidades do domínio;
- **auditoria/logs** traduzidos para o perfil;
- **alertas/ocorrências** com ação de resposta.

> Não desenhe todas essas telas por obrigação. O objetivo da baixa fidelidade é experimentar a **estrutura da interação** necessária para as tarefas priorizadas.

Para o projeto da equipe, foi escolhida uma interface conversacional, com foco nas seguintes funcionalidades:

- Campo para inserção de perguntas em linguagem natural.
- Botão para envio das consultas.
- Indicação de processamento da pergunta.
- Apresentação das respostas produzidas pelo assistente.
- Identificação das fontes institucionais utilizadas.
- Continuidade da conversa por meio de perguntas complementares.
- Mensagens de orientação quando não houver informações suficientes para responder.

Não foram incluídas telas de administração, dashboard ou configuração dos modelos de inteligência artificial, pois essas funcionalidades não fazem parte das tarefas priorizadas para os estudantes.

## 2. Fluxos escolhidos

| Fluxo | Tarefa/objetivo | Por que foi priorizado |
|---|---|---|
| PF01 | Formular e enviar uma dúvida acadêmica, receber a resposta e verificar as fontes institucionais apresentadas. Relacionado às tarefas T01, T02 e T03 e ao cenário C01 de Lucas. | Representa a principal interação do estudante com o assistente virtual, permitindo analisar a facilidade de realizar consultas e compreender as informações retornadas. |
| PF02 | Consultar informações sobre o ingresso em um programa de mestrado, compreender as orientações e realizar perguntas complementares. Relacionado ao cenário C02 de Mariana e à continuidade da interação prevista na T04. | Permite analisar a organização das respostas, a apresentação das fontes e a possibilidade de esclarecer informações sem reiniciar a conversa. |
| PF03 | Identificar quando não existem evidências suficientes para responder e reformular a pergunta. Relacionado à T05. | Permite avaliar como o assistente comunica suas limitações e orienta o estudante a continuar sua busca por informações confiáveis. |

Os fluxos foram escolhidos por representarem interações diretamente relacionadas aos objetivos definidos nas entregas anteriores.

O PF01 representa a interação principal do sistema. O PF02 explora a continuidade da conversa em uma consulta com múltiplas informações. O PF03 representa um caminho alternativo, importante para evitar que o usuário interprete uma resposta sem fundamentação como informação institucional confirmada.

## 3. Telas e estados

- Numere as telas/estados (`P01`, `P02`...).
- Indique controles que mudam o estado.
- Mostre pelo menos caminhos principais e estados de erro/retorno relevantes.

O protótipo foi organizado em seis telas ou estados de interação, compartilhados pelos fluxos selecionados.

| Tela/estado | Descrição | Interação e transição |
|---|---|---|
| P01 — Tela inicial | Apresenta a interface principal do assistente, com campo para digitar perguntas e botão de envio. | O estudante escreve sua dúvida e seleciona o botão de envio, avançando para P02. |
| P02 — Processamento da consulta | Apresenta a pergunta enviada e uma indicação de que o assistente está buscando informações. | Após o processamento, o sistema apresenta P03, P04 ou P05, conforme o resultado da consulta. |
| P03 — Resposta acadêmica | Apresenta a resposta para uma dúvida acadêmica, acompanhada das fontes institucionais utilizadas. | O estudante lê a resposta, consulta as fontes e pode realizar uma nova pergunta por meio de P06. |
| P04 — Resposta sobre mestrado | Apresenta orientações sobre o ingresso em um programa de mestrado, organizadas de maneira compreensível e acompanhadas das fontes disponíveis. | O estudante consulta as orientações e pode realizar perguntas complementares por meio de P06. |
| P05 — Ausência de evidências | Apresenta uma mensagem informando que não foram encontradas evidências suficientes para confirmar a informação solicitada. | O estudante pode reformular a pergunta ou procurar orientação nos canais institucionais indicados. |
| P06 — Continuidade da conversa | Permite realizar uma pergunta complementar ou reformular a consulta, mantendo as mensagens anteriores disponíveis. | O estudante escreve uma nova pergunta e retorna ao estado P02. |

**Fluxo principal — Lucas (PF01):**

1. O estudante acessa o assistente virtual na tela P01.
2. Digita uma dúvida acadêmica no campo de entrada.
3. Envia a pergunta, passando para P02.
4. Aguarda o processamento da consulta.
5. Recebe a resposta com as fontes institucionais na tela P03.
6. Analisa as informações e verifica a origem da resposta.
7. Caso precise de mais informações, utiliza P06 para continuar a conversa.

**Fluxo principal — Mariana (PF02):**

1. A estudante acessa o assistente virtual na tela P01.
2. Formula uma pergunta sobre o ingresso em um programa de mestrado.
3. Envia a consulta, passando para P02.
4. Aguarda o processamento.
5. Recebe as orientações organizadas na tela P04.
6. Consulta as fontes institucionais relacionadas às informações apresentadas.
7. Caso precise esclarecer alguma etapa ou requisito, utiliza P06 para fazer uma pergunta complementar.

**Fluxo alternativo — Ausência de evidências (PF03):**

1. O estudante realiza uma consulta pela tela P01 ou P06.
2. O assistente inicia o processamento na tela P02.
3. Quando não existem evidências documentais suficientes, apresenta a tela P05.
4. O estudante recebe uma orientação informando a limitação da resposta.
5. O estudante pode reformular a pergunta por meio de P06.
6. Após o novo envio, a interação retorna para P02.

**Estados de erro e retorno:**

- Quando o campo estiver vazio, a interface deverá impedir o envio e orientar o estudante a preencher uma pergunta.
- Durante o processamento, deverá ser apresentada uma indicação visual de que a solicitação está sendo realizada.
- Quando não houver informações suficientes, o assistente deverá informar essa limitação sem apresentar respostas sem fundamento.
- O estudante deverá conseguir realizar novas perguntas sem perder o contexto da conversa atual.

**Protótipo — Visão geral dos fluxos:**

![Protótipo](../assets/06_prototipos/prototipo_fluxo_01.svg)

**P01 — Tela inicial do assistente**

Representa o primeiro contato do estudante com o assistente virtual, destacando o campo para digitar perguntas e a ação de envio.

![P01 — Tela inicial](../assets/06_prototipos/p01_consulta_inicial.png)

**P02 — Processamento da consulta**

Representa o estado da interface após o envio de uma pergunta, informando ao estudante que a solicitação está sendo processada.

![P02 — Processamento](../assets/06_prototipos/p02_processamento.png)

**P03 — Resposta acadêmica com fontes**

Representa uma resposta apresentada ao estudante, com o conteúdo da orientação e a identificação das fontes institucionais utilizadas.

![P03 — Resposta com fontes](../assets/06_prototipos/p03_resposta_fontes.png)

**P04 — Resposta sobre ingresso no mestrado**

Representa a apresentação de informações sobre o ingresso em um programa de mestrado, com organização das orientações e identificação das respectivas fontes.

![P04 — Resposta sobre mestrado](../assets/06_prototipos/p04_mestrado.png)

**P05 — Ausência de evidências suficientes**

Representa a situação em que o assistente não consegue confirmar uma informação com base nos documentos disponíveis, apresentando uma mensagem de orientação.

![P05 — Ausência de evidências](../assets/06_prototipos/p05_sem_evidencias.png)

**P06 — Continuidade ou reformulação da consulta**

Representa a possibilidade de realizar perguntas complementares ou reformular dúvidas anteriores dentro da mesma conversa.

![P06 — Continuidade da conversa](../assets/06_prototipos/p06_pergunta_complementar.png)

## 4. Simulação / walkthrough

Realize uma simulação com uma pessoa que não participou da elaboração dessas telas. Um colega pode ser usado **para essa iteração formativa**, mas isso não substitui os participantes finais da Entrega 14.

A simulação será realizada com uma pessoa que não participou da elaboração do protótipo, utilizando os fluxos definidos na seção 2.

O objetivo é observar se a pessoa consegue compreender a interface e realizar as tarefas propostas sem receber instruções detalhadas sobre cada ação.

Para a simulação, foram definidos três cenários de utilização.

**Cenário 1 — Consulta acadêmica (PF01):**

O participante deverá utilizar o protótipo para realizar uma pergunta relacionada a uma informação acadêmica, como a solicitação de uma declaração de matrícula, localizar a resposta apresentada e identificar a fonte utilizada.

**Cenário 2 — Consulta sobre mestrado (PF02):**

O participante deverá utilizar o protótipo para consultar informações relacionadas ao ingresso em um programa de mestrado, compreender as orientações apresentadas e realizar uma pergunta complementar.

**Cenário 3 — Ausência de informações suficientes (PF03):**

O participante deverá interagir com um estado em que o assistente não apresenta evidências suficientes para responder à pergunta. Será observado se ele compreende a mensagem e consegue identificar uma maneira de continuar a consulta.

Durante o walkthrough, um integrante da equipe ficará responsável por apresentar os estados da interface conforme as ações indicadas pelo participante, enquanto o outro registrará dificuldades, dúvidas e comentários observados.

A simulação deverá considerar principalmente a localização dos controles, a compreensão das respostas, a identificação das fontes e a possibilidade de recuperação após uma consulta sem resultado conclusivo.

**Registro da simulação:**

- **Participante:** {{preencher após a realização}}
- **Data:** {{dd/mm/aaaa}}
- **Modalidade:** {{presencial/remota}}
- **Responsáveis:** Matheus Dourado Valle e João Pedro Sabino Garcia.

| Observação | Tela/ação | Evidência | Consequência para o design |
|---|---|---|---|
| {{Registrar a observação real sobre o envio da primeira consulta.}} | P01 / P02 | {{Registrar ação, dúvida ou comentário observado.}} | {{Indicar a decisão tomada com base na observação.}} |
| {{Registrar a observação real sobre a compreensão das respostas e fontes.}} | P03 / P04 | {{Registrar ação, dúvida ou comentário observado.}} | {{Indicar a decisão tomada com base na observação.}} |
| {{Registrar a observação real sobre a reformulação de perguntas.}} | P05 / P06 | {{Registrar ação, dúvida ou comentário observado.}} | {{Indicar a decisão tomada com base na observação.}} |

Os campos de observação, evidência e consequência serão preenchidos após a realização da simulação, utilizando os comportamentos efetivamente observados. As situações descritas anteriormente constituem o roteiro planejado, não resultados já obtidos.

## 5. Alterações após a simulação

As alterações no protótipo serão definidas após a realização do walkthrough, considerando as dificuldades identificadas durante a interação do participante com os estados apresentados.

As revisões deverão priorizar aspectos relacionados à clareza das informações, à identificação dos controles de interação, à apresentação das fontes institucionais e à possibilidade de continuar ou reformular consultas.

| Antes | Problema | Depois | Justificativa |
|---|---|---|---|
| {{Descrever como o elemento estava apresentado na versão inicial.}} | {{Registrar o problema identificado durante a simulação.}} | {{Descrever a alteração aplicada ao protótipo.}} | {{Explicar como a alteração atende ao problema observado.}} |

**Protótipo revisado após a simulação:**

![Protótipo revisado](../assets/06_prototipos/prototipo_revisado.png)

As alterações realizadas deverão ser representadas na versão revisada do protótipo e relacionadas às observações registradas na seção anterior.

Dessa maneira, a equipe poderá demonstrar a aplicação do ciclo construir, simular, observar e revisar, previsto no objetivo da atividade.

## Checklist

- [ ] O protótipo cobre tarefas relevantes da Entrega 5.
- [x] Cada tela/estado pode ser justificado por uma tarefa, decisão ou informação necessária.
- [x] O projeto não criou dashboard/CRUD/login apenas para parecer “completo”.
- [ ] Telas/estados estão numerados e navegáveis na documentação.
- [ ] Há pelo menos uma simulação/walkthrough documentado.
- [ ] Críticas não foram apenas listadas: geraram decisão de revisão.
- [ ] O protótipo continua em baixa fidelidade; detalhes visuais não mascaram problemas de fluxo.
