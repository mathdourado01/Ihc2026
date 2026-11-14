
# Entrega 12 — Planejamento da avaliação de usabilidade (DECIDE)

**Data:** 08/11/2026  
**Status:** 🟨 em andamento  
**Responsabilidade:** 1 solução por equipe

## Objetivo da atividade

Planejar a avaliação antes de executá-la, ligando perguntas de avaliação a métodos, participantes, tarefas, métricas, aspectos práticos, ética e forma de análise.

## O que está sendo avaliado

Em projetos cuja interface foi criada ou ampliada para a disciplina, o plano deve declarar explicitamente que a avaliação investiga **a qualidade da interação/protótipo**, não a validade científica ou o desempenho técnico do algoritmo/modelo do TCC.

Exemplos de perguntas:

- o DBA consegue localizar e comparar duas execuções?
- o analista entende o significado de um indicador?
- o administrador consegue alterar uma permissão sem risco de erro não percebido?
- o usuário compreende que o processamento está em andamento e consegue recuperar-se de uma falha?
- os filtros ajudam a localizar o histórico relevante?
- um relatório permite identificar a informação necessária para a decisão?

Se o protótipo utiliza dados ou resultados simulados, documente isso no plano.

No projeto da equipe, a avaliação será realizada sobre o protótipo interativo do **Assistente Virtual Acadêmico da FEI**, desenvolvido na Entrega 11.

O objetivo é verificar se os estudantes conseguem utilizar a interface para:

- formular dúvidas acadêmicas e administrativas em linguagem natural;
- compreender as respostas apresentadas pelo assistente;
- identificar e consultar fontes institucionais;
- realizar perguntas complementares durante uma conversa;
- reconhecer situações em que não existem evidências suficientes para responder;
- compreender quando o sistema está processando uma consulta.

A avaliação não pretende medir a precisão dos modelos de linguagem, a qualidade da recuperação vetorial ou as métricas técnicas do RAG desenvolvido no TCC. O foco está exclusivamente na qualidade da interação e na experiência de utilização do protótipo.

Como o protótipo foi desenvolvido no Figma, algumas perguntas, respostas, fontes institucionais e estados de processamento poderão ser previamente preparados ou simulados. Esses conteúdos serão mantidos iguais para todos os participantes, permitindo avaliar os caminhos de interação sem confundir a experiência de uso com o desempenho técnico do assistente.

A avaliação terá caráter formativo, pois os problemas identificados poderão orientar melhorias na interface.

Essa abordagem considera Barbosa e Silva (2010), que destacam a importância de avaliar a solução de IHC pela perspectiva dos usuários e utilizar protótipos para identificar problemas de interação antes da implementação final.

## A. Método DECIDE

| Etapa | Aplicação no projeto |
|---|---|
| **D — Determine the goals** | Avaliar a eficácia, eficiência, compreensão e satisfação durante o uso do protótipo. As metas MU01–MU07 e a meta qualitativa MU08 da Entrega 8 orientarão a avaliação. Pretende-se verificar se os estudantes conseguem iniciar consultas, compreender respostas, localizar fontes institucionais, complementar perguntas e reconhecer a ausência de evidências suficientes. |
| **E — Explore the questions** | Investigar se os estudantes conseguem enviar consultas sem ajuda, compreender as respostas, localizar fontes institucionais, realizar perguntas complementares e interpretar mensagens de ausência de evidências. Também será observado se o feedback de processamento é percebido e se a interface apresenta consistência, clareza e facilidade de utilização. |
| **C — Choose the evaluation paradigm and techniques** | Serão utilizados três métodos complementares: avaliação heurística, realizada pelos integrantes da equipe utilizando as dez heurísticas de Nielsen; testes de usabilidade com observação de estudantes executando tarefas no protótipo; e questionários pré e pós-teste para identificar familiaridade com sistemas semelhantes e satisfação. A combinação permite identificar problemas potenciais por inspeção e dificuldades durante a interação dos usuários. |
| **I — Identify the practical issues** | Serão realizados testes oficiais com dois estudantes universitários, conforme a quantidade prevista para a equipe na orientação da Entrega 14. Também será realizado um teste piloto adicional, que não será contabilizado entre os participantes oficiais. As sessões ocorrerão preferencialmente em ambiente tranquilo, utilizando computadores ou notebooks com navegador atualizado e acesso ao protótipo do Figma. A duração prevista será de 20 a 30 minutos por sessão. Matheus Dourado Valle será responsável pela condução das sessões e João Pedro Sabino Garcia pelo registro das observações. |
| **D — Decide how to deal with ethical issues** | A participação será voluntária, mediante explicação dos objetivos da atividade e obtenção do consentimento. Será esclarecido que o objetivo é avaliar o sistema, e não as habilidades do participante. Os registros utilizarão identificadores anônimos, como U01 e U02. Não serão solicitadas senhas, notas ou informações acadêmicas individuais. Não haverá gravação de áudio ou vídeo por padrão; qualquer gravação de tela dependerá de autorização específica. O participante poderá interromper a sessão a qualquer momento. |
| **E — Evaluate, interpret and present the data** | Serão registrados a conclusão das tarefas, os tempos, os erros, os pedidos de ajuda, as hesitações e a satisfação dos participantes. Os resultados serão comparados às metas MU01–MU07, enquanto MU08 será analisada qualitativamente. Os problemas identificados na avaliação heurística serão descritos com evidências e níveis de gravidade. Devido ao caráter exploratório e ao número reduzido de participantes, os resultados não serão generalizados estatisticamente. |

A organização do planejamento segue o framework DECIDE apresentado por Barbosa e Silva (2010), considerando a definição dos objetivos, as perguntas de avaliação, a escolha dos métodos, as questões práticas e éticas e a análise dos resultados.

## B. Perguntas de avaliação

| ID | Pergunta | Método | Métrica/evidência | Critério esperado |
|---|---|---|---|---|
| QA01 | O estudante consegue formular e enviar uma pergunta sem ajuda? | Observação | Conclusão sem ajuda, erros e solicitações de orientação. | MU01: pelo menos 90%. |
| QA02 | O estudante compreende corretamente a resposta apresentada? | Observação e pergunta de compreensão | Explicação dos pontos essenciais, comparada aos critérios definidos antes do teste. | MU02: pelo menos 80%. |
| QA03 | O estudante localiza e identifica a fonte institucional? | Observação | Tempo entre a apresentação do cenário e a identificação correta da fonte. | MU03: tempo mediano de até 30 segundos. |
| QA04 | O estudante consegue formular uma pergunta complementar relacionada à conversa? | Observação | Conclusão sem ajuda e necessidade de orientação. | MU04: pelo menos 80%. |
| QA05 | O estudante reconhece quando não há evidência suficiente para responder? | Observação e pergunta de interpretação | Interpretação correta da mensagem e identificação de como prosseguir. | MU05: pelo menos 90%. |
| QA06 | O estudante inicia uma consulta em tempo adequado? | Observação | Tempo entre a apresentação do cenário e o envio da pergunta. | MU06: tempo mediano de até 60 segundos. |
| QA07 | O estudante fica satisfeito com a experiência em cada tarefa? | Questionário pós-teste | Nota de satisfação de 1 a 5, calculada separadamente por tarefa. | MU07: média igual ou superior a 4,0 em cada tarefa. |
| QA08 | O estudante percebe que a consulta foi recebida e está sendo processada? | Observação e avaliação heurística | Comportamento observado e problemas relacionados à visibilidade do estado do sistema (H1). | MU08: estado perceptível e compreensível, sem limite percentual definido na Entrega 8. |
| QA09 | A interface mantém consistência e permite reconhecer, prevenir e recuperar-se de problemas? | Avaliação heurística | Violações das heurísticas H3, H4, H5 e H9, com localização e severidade. | Ausência de problemas críticos que impeçam os fluxos essenciais; demais achados serão registrados e priorizados. |

**Nota de rastreabilidade:** na Entrega 8, MU01–MU07 são metas quantitativas. MU08 corresponde à visibilidade do estado do sistema e está descrita qualitativamente, sem limite quantitativo próprio. Portanto, não será atribuído um percentual fictício a MU08.

## C. Escopo e participantes

| Item | Planejamento |
|---|---|
| Perfis | Estudantes universitários, preferencialmente da FEI, que representam o público-alvo do assistente. As personas P01 — Lucas Almeida e P02 — Mariana Costa serão utilizadas como referências para os cenários de utilização, mas não serão consideradas participantes reais. |
| Critérios de inclusão/exclusão | Inclusão: estudantes maiores de 18 anos, com conhecimentos básicos de navegação na internet e participação voluntária. Exclusão: integrantes da equipe responsável pelo desenvolvimento do protótipo. |
| Nº de participantes | Dois estudantes nos testes oficiais, um para cada integrante da equipe. Um participante adicional poderá realizar o teste piloto e não será contabilizado na avaliação oficial. |
| Ambiente | Preferencialmente presencial, em uma sala tranquila. Caso seja realizado remotamente, serão mantidas as mesmas instruções e condições essenciais de execução. |
| Dispositivo | Computador ou notebook com navegador atualizado, conexão com a internet e acesso ao protótipo interativo do Figma. |
| Protótipo/versão | Protótipo interativo do Assistente Virtual Acadêmico da FEI, desenvolvido na Entrega 11. Link: https://www.figma.com/design/H0YnqyGWkswU88IUZIgDuW. Será utilizada a versão finalizada, após a conferência dos fluxos necessários às tarefas. |
| Teste piloto | Será realizado previamente com um participante que não tenha participado do desenvolvimento. O piloto verificará a clareza das instruções, o funcionamento dos fluxos do Figma, a consistência dos conteúdos simulados, a adequação dos questionários e da planilha de observação e a duração das tarefas. Os ajustes necessários serão registrados antes dos testes oficiais. |

O recrutamento será realizado por convite voluntário a estudantes que atendam aos critérios estabelecidos. As sessões terão duração estimada de 20 a 30 minutos.

Responsabilidades previstas:

- **Matheus Dourado Valle:** moderar as sessões, apresentar os objetivos e as instruções e conduzir as tarefas.
- **João Pedro Sabino Garcia:** observar e registrar tempos, erros, dúvidas, solicitações de ajuda e comentários dos participantes.

Os integrantes poderão alternar as funções entre as sessões, mantendo um moderador e um observador sempre que possível.

O planejamento das sessões considera as orientações de preparação e coleta de dados apresentadas por Barbosa e Silva (2010), incluindo a apresentação da atividade, o consentimento, a aplicação do questionário pré-teste, a execução das tarefas e a coleta das impressões após a utilização.

## D. Lista de tarefas de avaliação

| ID | Cenário neutro entregue ao usuário | Objetivo oculto da avaliação | Critério de sucesso | Tempo-limite (se houver) |
|---|---|---|---|---|
| UT01 | Você é estudante da FEI e precisa esclarecer uma dúvida acadêmica. Utilize o assistente para enviar uma pergunta que ajude a entender essa situação. | T01 — Formular e enviar uma pergunta em linguagem natural e perceber o processamento da consulta. | O participante envia a pergunta sem orientação e percebe que ela foi recebida e está sendo processada. | Até 60 segundos para iniciar e enviar, relacionado à MU06. |
| UT02 | Você recebeu uma orientação sobre um procedimento acadêmico. Leia a resposta e explique, com suas palavras, as principais etapas, requisitos ou informações apresentadas. | T02 — Ler e compreender uma resposta apresentada pelo assistente. | O participante explica corretamente os pontos essenciais definidos previamente pela equipe. | Registrar duração, sem limite quantitativo definido. |
| UT03 | Você deseja confirmar de onde veio a orientação recebida. Identifique a fonte institucional associada à resposta. | T03 — Identificar e consultar a fonte institucional apresentada pelo assistente. | O participante identifica corretamente a fonte institucional apresentada. | Até 30 segundos, relacionado à MU03. |
| UT04 | Depois de receber uma orientação, você percebe que ainda tem uma dúvida relacionada ao mesmo assunto. Continue a conversa para esclarecer esse ponto. | T04 — Formular uma pergunta complementar e manter a continuidade da interação. | O participante envia uma pergunta complementar relacionada ao contexto, sem ajuda. | Registrar duração, sem limite quantitativo definido. |
| UT05 | Em outra consulta, o assistente informa que não encontrou informações suficientes para confirmar uma resposta. Explique o que a mensagem significa e o que faria em seguida. | T05 — Reconhecer a ausência de evidências e compreender como prosseguir. | O participante reconhece que a informação não foi confirmada e indica uma ação adequada para continuar buscando a informação. | Registrar duração, sem limite quantitativo definido. |

As respostas, fontes e estados simulados serão mantidos iguais para todos os participantes. Para UT02, os pontos essenciais esperados na explicação serão definidos antes da coleta.

> Uma boa instrução descreve o objetivo do participante sem dizer **onde clicar** ou usar o rótulo exato do controle que está sendo testado.

## E. Instrumentos

- [Modelo de termo de consentimento](../instrumentos/termo_consentimento_modelo.md)
- [Roteiro de teste](../instrumentos/roteiro_teste_usabilidade.md)
- [Planilha de observação](../instrumentos/planilha_observacao_modelo.md)
- [Formulário de avaliação heurística](../instrumentos/formulario_heuristica_modelo.md)

Os questionários pré e pós-teste estarão integrados ao roteiro de teste, evitando a criação de arquivos separados.

O questionário pré-teste registrará a familiaridade dos participantes com sistemas acadêmicos, assistentes virtuais e ferramentas de consulta de informações.

O questionário pós-teste registrará a satisfação após cada tarefa, além de permitir comentários sobre dificuldades, aspectos positivos e sugestões de melhoria.

O formulário de avaliação heurística utilizará as dez heurísticas de Nielsen, complementadas pelos princípios de design de IHC apresentados por Barbosa e Silva (2010), especialmente consistência, visibilidade, feedback, clareza do conteúdo e prevenção e recuperação de erros.

## F. Plano de análise

Defina antes dos testes:

- **Sucesso total / parcial / falha:**

  - Sucesso total: o participante conclui corretamente a tarefa, sem receber ajuda do moderador.
  - Sucesso parcial: o participante alcança o objetivo, mas necessita de orientação ou apresenta dificuldade que exige uma tentativa adicional.
  - Falha: o participante não consegue alcançar o objetivo, interpreta incorretamente uma informação essencial ou abandona a tarefa sem concluí-la.

- **O que conta como erro, dúvida, ajuda e abandono:**

  - Erro: ação inadequada ou interpretação incorreta que prejudique a execução da tarefa.
  - Dúvida: manifestação verbal de incerteza, hesitação ou dificuldade para compreender a interface.
  - Ajuda: orientação fornecida pelo moderador além da repetição neutra do cenário apresentado.
  - Abandono: situação em que o participante decide interromper uma tarefa antes de alcançar seu objetivo.

  A exploração espontânea da interface não será considerada automaticamente um erro. Será registrada quando houver evidência de dificuldade ou consequência negativa para a realização da tarefa.

- **Como tempo será medido:**

  - A contagem será iniciada após a apresentação do cenário e a autorização para o participante começar.
  - O tempo será encerrado quando o objetivo da tarefa for alcançado, quando ocorrer abandono ou quando for atingido o limite operacional definido.
  - Os tempos serão registrados em segundos.
  - Para MU06, será considerado o intervalo entre a apresentação do cenário e o envio da pergunta.
  - Para MU03, será considerado o intervalo entre a apresentação da resposta e a identificação correta da fonte.
  - Serão calculadas as medianas dos tempos observados, apresentando também os valores individuais.

- **Escala de satisfação pós-tarefa:**

  Será utilizada uma escala de 1 a 5:

  - 1 — Muito insatisfeito.
  - 2 — Insatisfeito.
  - 3 — Neutro.
  - 4 — Satisfeito.
  - 5 — Muito satisfeito.

  Após cada tarefa, o participante responderá à pergunta:

  **"Qual foi seu nível de satisfação ao realizar esta tarefa utilizando o assistente?"**

  A média será calculada separadamente para cada tarefa, considerando a meta MU07 de pelo menos 4,0 pontos.

- **Como observações/falas serão codificadas:**

  | Código | Categoria | Descrição |
  |---|---|---|
  | NAV | Navegação | Dificuldade para localizar elementos ou compreender os caminhos de interação. |
  | COM | Compreensão | Dificuldade para interpretar respostas, instruções ou mensagens. |
  | FON | Fontes | Problemas para identificar ou consultar fontes institucionais. |
  | FDB | Feedback | Falta de clareza sobre o estado do sistema ou processamento da consulta. |
  | ERR | Erros | Ações incorretas ou dificuldades de recuperação. |
  | VIS | Visual | Problemas de legibilidade, organização ou identificação de elementos. |
  | CON | Continuidade | Dificuldades para realizar perguntas complementares ou manter o contexto da conversa. |
  | POS | Positivo | Comentários ou comportamentos que indiquem facilidade e satisfação durante a utilização. |

- **Como problemas serão priorizados:**

  Os problemas identificados serão classificados utilizando uma escala de gravidade de 0 a 4:

  | Gravidade | Classificação | Descrição |
  |---|---|---|
  | 0 | Não é problema | Não representa um problema de usabilidade. |
  | 1 | Cosmético | Problema visual ou de apresentação com baixo impacto na execução das tarefas. |
  | 2 | Menor | Dificulta a utilização, mas não impede a conclusão da tarefa. |
  | 3 | Grave | Compromete significativamente a execução ou compreensão de uma tarefa. |
  | 4 | Crítico | Impede a realização de uma tarefa essencial ou provoca uma interpretação equivocada sem possibilidade clara de recuperação. |

  A priorização considerará a gravidade, a frequência com que o problema aparece e seu impacto sobre os objetivos dos estudantes.

- **Como comparar resultados às metas de usabilidade:**

  | Meta | Critério de comparação |
  |---|---|
  | MU01 | Taxa de conclusão sem ajuda em T01 igual ou superior a 90%. |
  | MU02 | Taxa de compreensão correta em T02 igual ou superior a 80%. |
  | MU03 | Tempo mediano para localizar a fonte em T03 de até 30 segundos. |
  | MU04 | Taxa de conclusão sem ajuda em T04 igual ou superior a 80%. |
  | MU05 | Interpretação correta da ausência de evidências em T05 igual ou superior a 90%. |
  | MU06 | Tempo mediano para iniciar uma consulta em T01 de até 60 segundos. |
  | MU07 | Satisfação média igual ou superior a 4,0 em cada tarefa. |
  | MU08 | Evidência qualitativa de que o estudante percebe e compreende o estado de processamento. |

  Como a amostra planejada é de dois participantes, os resultados serão apresentados também em contagens absolutas, por exemplo, 2/2. Nesse tamanho de amostra, as metas de 80% ou 90% somente serão alcançadas se os dois participantes apresentarem o comportamento esperado. Essa limitação será considerada na interpretação, sem pretensão de generalização estatística.

Os resultados serão organizados por participante e tarefa, utilizando identificadores anônimos.

Serão calculadas as taxas de conclusão, os tempos observados, as médias de satisfação e a quantidade de erros e solicitações de ajuda.

As observações qualitativas serão utilizadas para complementar os resultados quantitativos, permitindo compreender as causas das dificuldades encontradas.

Os resultados da avaliação heurística serão comparados aos problemas observados nos testes com usuários, identificando quais dificuldades poderiam ser previstas pela inspeção e quais foram percebidas durante a interação.

A apresentação final incluirá os objetivos e o escopo da avaliação, os métodos utilizados, o perfil e a quantidade de participantes, os dados coletados, a interpretação dos resultados, os problemas identificados, suas gravidades e as recomendações de melhoria para o protótipo.

## Checklist

- [x] As seis etapas DECIDE foram contextualizadas, não apenas expandidas por sigla.
- [x] Perguntas de avaliação têm método e evidência correspondentes.
- [x] O plano distingue avaliação de IHC de avaliação técnica/científica do TCC.
- [x] Dados ou processamentos simulados no protótipo estão declarados.
- [x] Tarefas vêm de objetivos/cenários relevantes.
- [x] Critérios de sucesso foram definidos antes da coleta.
- [x] Questões práticas e éticas estão resolvidas.
- [x] Instrumentos estão prontos antes da Entrega 13/14.
- [x] Plano diz como dados serão analisados e apresentados.
