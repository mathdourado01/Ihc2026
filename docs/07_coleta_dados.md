# Entrega 7 — Coleta de dados, necessidades e aspectos éticos

**Data:** 10/10/2026  
**Status:** 🟩 concluída  
**Revisão após feedback:** 25/11/2026

## Objetivo da atividade

Planejar a coleta de dados necessária para compreender as necessidades dos estudantes da FEI em relação à busca por informações acadêmicas e administrativas, identificando dificuldades, hábitos de consulta e requisitos de interação relevantes para o desenvolvimento do Assistente Virtual FEI.

## Para escopos de IHC derivados de TCC técnico

O projeto de IHC é derivado do TCC que propõe um assistente virtual baseado em Recuperação Aumentada por Geração (RAG), destinado a responder dúvidas acadêmicas e administrativas de estudantes da FEI.

A coleta proposta busca investigar se o cenário de uso definido nas entregas anteriores corresponde às necessidades reais dos estudantes, considerando:

- Como os estudantes procuram informações acadêmicas atualmente.
- Quais ferramentas e canais utilizam para realizar consultas.
- Quais assuntos são procurados com maior frequência.
- Quais dificuldades encontram ao localizar ou compreender informações.
- Como verificam a confiabilidade das informações obtidas.
- Quais consequências podem ocorrer quando uma informação não é encontrada ou compreendida corretamente.
- Quais recursos de interação seriam relevantes em uma possível solução digital.
- Se funcionalidades como histórico de conversas e apresentação de fontes representam necessidades reais dos estudantes.
- Qual é a familiaridade dos estudantes com assistentes conversacionais e ferramentas de inteligência artificial.

As personas e os cenários definidos anteriormente serão tratados como hipóteses de projeto, e não como evidências suficientes para confirmar as necessidades do público-alvo.

Nesta etapa, os instrumentos de coleta foram preparados para eventual aplicação. O questionário foi implementado, publicado e validado funcionalmente, mas a equipe optou por não realizar a coleta de respostas neste momento.

## Hipóteses e lacunas prioritárias herdadas da Entrega 1

As hipóteses estabelecidas anteriormente orientam a definição dos dados necessários e das perguntas presentes no instrumento de coleta.

| ID | Hipótese/lacuna | Evidência atual | Decisão que depende da resposta | Prioridade |
|---|---|---|---|---|
| H04/H05 | Necessidades relacionadas à frequência e aos tipos de consultas acadêmicas. | Hipóteses e cenários definidos nas entregas anteriores, ainda sem validação direta com usuários. | Priorização das tarefas e dos conteúdos contemplados pela interface. | Alta |
| H07/H08 | Dificuldades relacionadas aos canais utilizados e à localização de informações institucionais. | Análise inicial do contexto de utilização e dos canais institucionais existentes. | Organização do fluxo de consulta e apresentação das informações. | Alta |
| H09 | Possíveis dificuldades de compreensão das informações acadêmicas. | Hipótese de projeto ainda não verificada diretamente com estudantes. | Definição da linguagem e da estrutura das respostas. | Alta |
| H02/H14 | Necessidade de apresentar fontes institucionais para apoiar a confiabilidade das respostas. | Requisito considerado na proposta inicial do assistente virtual. | Forma de exibição das fontes consultadas e referências institucionais. | Alta |
| H12 | Necessidades relacionadas aos dispositivos utilizados pelos estudantes. | Contexto de uso previsto nas entregas anteriores. | Adaptação da interface para diferentes dispositivos. | Média |
| H15 | Necessidade de recuperar informações consultadas anteriormente. | Funcionalidade considerada no projeto, ainda sem confirmação de sua relevância para os usuários. | Priorização do histórico de conversas entre sessões. | Média |
| H06/H10/H16 | Possíveis consequências de erros ou dificuldades durante a obtenção de informações acadêmicas. | Riscos considerados nos cenários e hipóteses anteriores. | Definição de mecanismos de prevenção de erros e apresentação de orientações. | Alta |
| H18 | Familiaridade dos estudantes com interfaces conversacionais e assistentes de inteligência artificial. | Hipótese estabelecida anteriormente, ainda sem confirmação direta com estudantes. | Adequação da linguagem, das instruções iniciais e do padrão conversacional da interface. | Alta |

## Parte A — necessidades e requisitos de IHC

> **Responsabilidade:** solução individual por integrante.

### A01 — Matheus Dourado Valle

**Autor(a):** Matheus Dourado Valle — 22.224.023-6

#### Que dados coletar?

A coleta busca compreender como os estudantes da FEI procuram informações acadêmicas e administrativas, quais dificuldades enfrentam e quais características seriam relevantes para uma possível interface de assistência virtual.

| Dado/informação | Hipótese/lacuna relacionada | Por que é necessário | Qual decisão de design pode afetar |
|---|---|---|---|
| Frequência com que estudantes procuram informações acadêmicas ou administrativas. | H04/H05 | Investigar se a atividade considerada central no projeto realmente faz parte da rotina dos estudantes. | Definição das tarefas prioritárias da interface. |
| Tipos de informações mais procuradas. | H04/H05/H06 | Identificar quais assuntos representam necessidades recorrentes ou relevantes. | Priorização dos conteúdos contemplados pelo assistente. |
| Canais utilizados atualmente para encontrar informações. | H07/H08 | Compreender como os estudantes realizam suas consultas e quais ferramentas utilizam. | Organização do fluxo de consulta e apresentação das fontes de informação. |
| Dificuldades encontradas durante a busca. | H08/H09 | Investigar possíveis obstáculos relacionados à localização e compreensão das informações. | Organização e apresentação das respostas. |
| Consequências de informações não encontradas ou compreendidas incorretamente. | H06/H10/H16 | Identificar situações nas quais erros podem prejudicar decisões ou procedimentos acadêmicos. | Tratamento de erros, orientações e apresentação de limitações. |
| Importância da identificação das fontes institucionais. | H02/H14 | Investigar quais elementos influenciam a confiança nas informações consultadas. | Forma de apresentação das fontes e referências utilizadas nas respostas. |
| Dispositivos utilizados para realizar consultas. | H12 | Compreender o contexto tecnológico de utilização. | Adaptação da interface para diferentes dispositivos. |
| Necessidade de recuperar informações consultadas anteriormente. | H15 | Investigar se o histórico de consultas representa uma necessidade real dos estudantes. | Priorização do recurso de histórico e recuperação de conversas entre sessões. |
| Frequência e finalidade de utilização de assistentes conversacionais e inteligência artificial. | H18 | Investigar a familiaridade dos estudantes com esse padrão de interação. | Adequação da linguagem, das instruções e do fluxo conversacional. |

#### De quem coletar?

O público principal será composto por estudantes de graduação da FEI, considerando que o assistente virtual foi proposto para apoiar a resolução de dúvidas acadêmicas e administrativas desse público.

| Perfil/stakeholder | Critério de inclusão | Relação com persona/público |
|---|---|---|
| Estudantes de graduação da FEI. | Estar regularmente matriculado em um curso de graduação da instituição e concordar voluntariamente em participar da pesquisa. | Público principal representado pelas personas P01 — Lucas Almeida e P02 — Mariana Costa. |
| Estudantes de diferentes períodos da graduação. | Estar em qualquer etapa do curso, preferencialmente contemplando experiências distintas com os serviços institucionais. | Permite investigar se as necessidades variam conforme a experiência acadêmica. |

A participação de estudantes de diferentes períodos poderá contribuir para identificar necessidades relacionadas tanto à adaptação à instituição quanto a procedimentos acadêmicos específicos de etapas mais avançadas da graduação.

As personas utilizadas anteriormente representam hipóteses de perfis de usuários, não sendo consideradas evidências suficientes para confirmar suas necessidades reais.

Para uma eventual aplicação do questionário, foi estabelecido o seguinte planejamento:

- **Meta de participantes:** 20 estudantes de graduação da FEI.
- **Estratégia de recrutamento:** divulgação voluntária em grupos de estudantes e convites diretos, buscando participantes de diferentes períodos da graduação.
- **Modalidade:** on-line, por meio do Google Forms.
- **Duração estimada:** 5 a 8 minutos por participante.
- **Critério de encerramento:** atingir a meta de participantes ou o prazo previamente definido para a coleta.
- **Responsável:** Matheus Dourado Valle.

A quantidade estabelecida representa uma meta exploratória de planejamento, não uma amostra estatisticamente representativa da população de estudantes da FEI.

A equipe optou por não iniciar o recrutamento ou a coleta nesta etapa.

#### Aspectos éticos

A coleta de dados deverá respeitar a privacidade, a autonomia e a participação voluntária dos estudantes, considerando os princípios éticos discutidos na disciplina e a Lei Geral de Proteção de Dados (LGPD).

- **Voluntariedade e consentimento:** antes do preenchimento do questionário, os participantes receberão uma explicação sobre o objetivo acadêmico da pesquisa e a utilização pretendida das respostas. A participação será voluntária, sem qualquer prejuízo em caso de recusa.

- **Minimização de dados:** o questionário não solicitará nome completo, matrícula, CPF, telefone, endereço ou outras informações pessoais que não sejam necessárias para compreender as necessidades investigadas. Serão solicitados apenas dados pertinentes à pesquisa, confirmação de elegibilidade, faixa de semestre e um código aleatório para eventual solicitação de exclusão da resposta.

- **Privacidade e riscos:** como o estudo aborda experiências com serviços acadêmicos, existe a possibilidade de participantes mencionarem dificuldades relacionadas a setores ou procedimentos institucionais. Para reduzir riscos de exposição, será solicitado que não sejam compartilhados dados pessoais, situações identificáveis de terceiros ou informações acadêmicas sigilosas.

- **Gravação:** a técnica escolhida não prevê gravação de áudio ou vídeo.

- **Anonimização:** as respostas serão analisadas de forma agregada. Eventuais exemplos textuais utilizados na documentação serão revisados para evitar a identificação de participantes ou terceiros.

- **Armazenamento:** caso o questionário seja aplicado, os dados serão armazenados em ambiente digital com acesso restrito aos integrantes responsáveis pela atividade. O formulário não deverá coletar automaticamente endereços de e-mail.

- **Descarte:** os registros individuais serão mantidos apenas durante o período necessário à análise e avaliação acadêmica da atividade, sendo posteriormente excluídos. A documentação final poderá preservar resultados agregados e não identificáveis.

- **Desistência:** o participante poderá interromper o preenchimento a qualquer momento antes do envio, bastando fechar a página, sem necessidade de apresentar justificativa.

- **Exclusão de respostas:** antes da consolidação dos resultados, o participante poderá solicitar a exclusão de sua resposta utilizando o código anônimo informado durante o preenchimento e o contato disponibilizado no formulário. A equipe deverá confirmar que o registro corresponde ao código informado antes de realizar a exclusão.

- **Responsáveis e contato:** Matheus Dourado Valle e João Pedro Sabino Garcia são os responsáveis pela atividade. O meio de contato da equipe deverá permanecer disponível na descrição do formulário para esclarecimento de dúvidas e solicitação de exclusão de respostas.

- **Ausência de impacto acadêmico:** a participação, recusa ou desistência não terá qualquer consequência sobre notas, avaliações, relacionamento com professores ou benefícios acadêmicos.

A pesquisa não será utilizada para avaliar individualmente estudantes, professores ou funcionários da FEI.

### A02 — João Pedro Sabino Garcia

**Autor(a):** João Pedro Sabino Garcia — 22.224.032-7

#### Que dados coletar?

A coleta busca compreender como os estudantes da FEI interpretam, relacionam e organizam diferentes assuntos acadêmicos e administrativos, investigando quais agrupamentos e nomenclaturas são mais intuitivos para o público-alvo.

A técnica proposta permitirá identificar possíveis dificuldades na compreensão das categorias institucionais, contribuindo para decisões relacionadas à organização das sugestões de assuntos, exemplos de perguntas e linguagem do Assistente Virtual FEI.

| Dado/informação | Hipótese/lacuna relacionada | Por que é necessário | Qual decisão de design pode afetar |
|---|---|---|---|
| Forma como os estudantes agrupam diferentes assuntos acadêmicos. | H04/H05 | Investigar como os estudantes relacionam os conteúdos que procuram. | Organização dos exemplos de perguntas e assuntos sugeridos pelo assistente. |
| Nomes atribuídos aos agrupamentos de assuntos. | H09 | Identificar o vocabulário utilizado pelos estudantes e possíveis diferenças em relação à terminologia institucional. | Definição das nomenclaturas e da linguagem utilizadas na interface. |
| Assuntos frequentemente agrupados em uma mesma categoria. | H07/H08 | Compreender quais informações os estudantes consideram relacionadas. | Organização das sugestões de assuntos relacionados. |
| Assuntos que geram dúvidas durante a classificação. | H08/H09 | Identificar possíveis ambiguidades na interpretação das informações acadêmicas. | Revisão da apresentação e identificação dos conteúdos. |
| Diferenças entre os agrupamentos realizados pelos participantes. | H04/H05 | Investigar se diferentes estudantes possuem modelos mentais semelhantes sobre a organização dos assuntos acadêmicos. | Definição de exemplos e sugestões compreensíveis para diferentes perfis. |
| Necessidade de consultar assuntos relacionados durante uma mesma busca. | H07/H08 | Investigar possíveis relações entre diferentes necessidades informacionais. | Avaliação da necessidade de apresentar assuntos relacionados durante as consultas. |

A classificação de cartões não será utilizada para justificar automaticamente a criação de menus ou categorias obrigatórias de navegação, pois o projeto prioriza a interação por linguagem natural.

Os resultados poderão orientar elementos concretos da interface, como exemplos de perguntas apresentados na tela inicial, sugestões de assuntos relacionados e escolha de terminologias compreensíveis pelos estudantes.

#### De quem coletar?

O público será composto por estudantes de graduação da FEI, considerando que a organização das informações acadêmicas e administrativas deverá ser compreensível para os usuários finais do assistente virtual.

| Perfil/stakeholder | Critério de inclusão | Relação com persona/público |
|---|---|---|
| Estudantes de graduação da FEI. | Estar regularmente matriculado em um curso de graduação e aceitar voluntariamente participar da atividade. | Público principal representado pelas personas P01 — Lucas Almeida e P02 — Mariana Costa. |
| Estudantes de diferentes períodos da graduação. | Possuir experiências distintas com os serviços e procedimentos acadêmicos da instituição. | Permite investigar possíveis diferenças na compreensão e organização dos assuntos institucionais. |

A inclusão de estudantes com diferentes níveis de experiência acadêmica poderá contribuir para identificar se a organização das informações é compreensível tanto para alunos ingressantes quanto para aqueles que já possuem maior familiaridade com os procedimentos institucionais.

Para uma eventual aplicação da técnica, foi estabelecido o seguinte planejamento:

- **Meta de participantes:** cinco estudantes de graduação da FEI.
- **Estratégia de recrutamento:** convites voluntários a estudantes de diferentes períodos da graduação.
- **Modalidade:** presencial e individual.
- **Local previsto:** espaço de estudo da FEI, com mesa disponível para organização dos cartões.
- **Material:** cartões impressos, folhas em branco, caneta e ficha padronizada de registro.
- **Duração estimada:** 10 a 15 minutos por participante.
- **Critério de encerramento:** realização das cinco sessões planejadas ou término do prazo previamente estabelecido.
- **Responsável:** João Pedro Sabino Garcia.

A quantidade estabelecida possui caráter exploratório e não permite generalização estatística para todos os estudantes da instituição.

Nenhuma sessão de classificação de cartões foi realizada nesta etapa.

#### Aspectos éticos

A atividade deverá respeitar os princípios de voluntariedade, consentimento, privacidade e minimização de dados, considerando que os participantes realizarão uma classificação de assuntos relacionados ao ambiente acadêmico da FEI.

- **Voluntariedade e consentimento:** antes da atividade, os participantes receberão informações sobre o objetivo acadêmico da pesquisa, os procedimentos envolvidos e a utilização pretendida dos resultados. A participação será voluntária, sendo permitido interrompê-la a qualquer momento, sem qualquer prejuízo.

- **Minimização de dados:** não serão solicitados nome completo, matrícula, CPF, telefone, endereço ou informações acadêmicas individuais. Serão registrados apenas os agrupamentos realizados, os nomes atribuídos às categorias e eventuais dificuldades relatadas voluntariamente.

- **Privacidade e riscos:** a atividade utilizará assuntos acadêmicos genéricos e não exigirá acesso ao Portal do Aluno, apresentação de documentos pessoais ou compartilhamento de informações institucionais restritas. O principal risco considerado é a exposição indevida de dados caso o participante insira informações pessoais nos campos de resposta.

- **Gravação:** não serão realizadas gravações de áudio ou vídeo. Os resultados serão registrados por meio dos agrupamentos e das categorias produzidas durante a atividade.

- **Anonimização:** caso a técnica seja aplicada, os participantes serão identificados apenas por códigos, como CS01, CS02 e CS03, sem associação com seus dados pessoais.

- **Armazenamento:** os resultados serão armazenados em ambiente digital com acesso restrito aos integrantes responsáveis pela pesquisa, sendo utilizados exclusivamente para fins acadêmicos.

- **Descarte:** os registros individuais serão mantidos somente durante o período necessário à análise e avaliação da atividade. Após esse período, serão excluídos, podendo ser preservadas apenas informações consolidadas e não identificáveis.

- **Desistência e exclusão:** o participante poderá interromper a atividade sem justificativa e solicitar a exclusão de seu registro antes da consolidação dos resultados, utilizando o código anônimo atribuído à sessão.

- **Responsáveis e contato:** os integrantes da equipe serão identificados antes da atividade, disponibilizando o mesmo contato utilizado no questionário I01 para esclarecimento de dúvidas e solicitação de exclusão dos registros.

- **Ausência de impacto acadêmico:** a participação ou recusa não terá qualquer efeito sobre notas, avaliações ou benefícios acadêmicos.

A atividade não terá caráter avaliativo sobre o desempenho individual dos estudantes. Não existirão respostas certas ou erradas, pois o objetivo será compreender diferentes formas de organização das informações.

## Parte B — ferramentas de coleta

> Cada integrante deve preparar uma técnica/instrumento completo. As técnicas devem ser diferentes entre si e **questionário deve estar entre as técnicas escolhidas**, conforme o enunciado da disciplina.

### Instrumento I01 — Questionário

**Autor(a):** Matheus Dourado Valle — 22.224.023-6  
**Técnica:** Questionário estruturado, com perguntas fechadas e abertas.  
**Objetivo:** Investigar os hábitos, necessidades e dificuldades dos estudantes da FEI durante a busca por informações acadêmicas e administrativas, contribuindo para a avaliação das hipóteses estabelecidas nas entregas anteriores.  
**Público:** Estudantes de graduação da FEI.

#### Procedimento padronizado de aplicação

1. **Preparação:** o formulário digital foi elaborado e publicado utilizando o Google Forms, contemplando as perguntas, alternativas, orientações e aspectos éticos estabelecidos neste instrumento. A equipe realizou testes de funcionamento, acesso e encaminhamento entre as seções. Antes de eventual coleta, deverão ser eliminados os registros de teste e reconferidas as configurações de privacidade e o contato da equipe.

2. **Apresentação/consentimento:** apresentar uma breve explicação sobre o objetivo da pesquisa, seu caráter acadêmico e a participação voluntária. O participante deverá manifestar concordância antes de acessar as perguntas. Caso não concorde, o formulário será encerrado. Após o consentimento, será realizada a confirmação de elegibilidade do participante.

3. **Aplicação:** disponibilizar o questionário digitalmente aos estudantes da FEI. Cada participante responderá individualmente, sem necessidade de acompanhamento por um pesquisador. O tempo estimado de preenchimento será de 5 a 8 minutos.

4. **Encerramento:** apresentar uma mensagem de agradecimento ao finalizar o formulário, sem solicitar dados pessoais adicionais ou justificativas sobre as respostas fornecidas.

5. **Armazenamento/anonimização:** caso a coleta seja realizada, exportar os dados para análise e mantê-los em ambiente de acesso restrito. Os resultados poderão ser utilizados em tabelas, gráficos e sínteses textuais, evitando qualquer identificação individual.

#### Instrumento

**Título do questionário:** Pesquisa sobre a busca de informações acadêmicas na FEI.

**Link público para preenchimento:**

[Google Forms — Instrumento I01](https://docs.google.com/forms/d/e/1FAIpQLSdEVU2WLhhA-rumpGj_FIY1asA0vgKm6zGzQPv-tMY77aN_Rg/viewform?usp=publish-editor)

**Registro de validação do formulário:**

Em 25/11/2026, a equipe realizou a conferência funcional do questionário publicado, verificando os seguintes aspectos:

| Verificação | Resultado |
|---|---|
| Acesso ao formulário por meio do link público. | Funcionamento confirmado. |
| Acesso sem exigência de autenticação institucional. | Funcionamento confirmado. |
| Encerramento após recusa do consentimento. | Funcionamento confirmado. |
| Encerramento após identificação de participante inelegível. | Funcionamento confirmado. |
| Acesso às perguntas por participante elegível que aceitou o consentimento. | Funcionamento confirmado. |
| Preenchimento e envio das respostas pelo caminho elegível. | Funcionamento confirmado. |
| Configurações de privacidade e ausência de coleta automática de e-mail. | Funcionamento confirmado. |

Os testes foram realizados para verificar o funcionamento do instrumento, não constituindo uma coleta de dados de pesquisa.

**Situação da coleta:** o formulário encontra-se publicado e disponível para eventual aplicação. A equipe optou por não realizar a coleta de respostas nesta etapa. Consequentemente, não existem resultados empíricos provenientes deste instrumento.

**Texto de apresentação:**

Este questionário faz parte de uma atividade acadêmica da disciplina de Interação Humano-Computador (IHC), cujo projeto investiga as necessidades dos estudantes da FEI relacionadas à busca por informações acadêmicas e administrativas.

O objetivo é compreender como essas informações são procuradas atualmente, quais dificuldades podem ocorrer e quais necessidades devem ser consideradas no desenvolvimento de uma possível solução digital.

A participação é voluntária e o preenchimento leva aproximadamente de 5 a 8 minutos. Não serão solicitados nome, matrícula ou outros dados de identificação pessoal. As respostas serão utilizadas exclusivamente para fins acadêmicos.

A participação ou recusa não terá qualquer efeito sobre notas, avaliações ou benefícios acadêmicos, nem está vinculada a qualquer exigência de professores.

Você poderá desistir a qualquer momento antes de enviar o formulário, bastando fechar a página.

Os dados serão armazenados em ambiente digital de acesso restrito aos integrantes da equipe e excluídos após a conclusão da análise e da avaliação acadêmica da atividade. Apenas resultados agregados e não identificáveis poderão ser mantidos na documentação final.

Caso deseje solicitar a exclusão de sua resposta antes da consolidação dos resultados, utilize o código anônimo informado durante o preenchimento e entre em contato com a equipe responsável.

Ao responder, evite mencionar informações pessoais, dados acadêmicos sigilosos ou informações identificáveis de terceiros.

**Responsáveis:** Matheus Dourado Valle e João Pedro Sabino Garcia.

**Contato:** meio de contato disponibilizado na descrição do formulário publicado.

**Consentimento**

Você concorda voluntariamente em participar desta pesquisa, considerando as informações apresentadas?

- ( ) Sim, concordo.
- ( ) Não concordo.

Caso a resposta seja negativa, o formulário será encerrado imediatamente, sem apresentar as demais perguntas.

**Pergunta 1 — Você é estudante de graduação da FEI?**

Tipo: escolha única e obrigatória.

- ( ) Sim.
- ( ) Não.

Caso a resposta seja negativa, o formulário será encerrado, pois o participante não pertence ao público-alvo definido.

**Pergunta 2 — Com que frequência você costuma procurar informações acadêmicas ou administrativas relacionadas à FEI?**

Tipo: escolha única e obrigatória.

- ( ) Diariamente.
- ( ) Algumas vezes por semana.
- ( ) Algumas vezes por mês.
- ( ) Raramente.
- ( ) Nunca.
- ( ) Não sei informar.

**Pergunta 3 — Quais tipos de informações você costuma procurar?**

Tipo: caixas de seleção e obrigatória.

Instrução: caso selecione "Não costumo procurar essas informações", não marque outras alternativas.

- [ ] Matrícula e rematrícula.
- [ ] Calendário acadêmico.
- [ ] Notas e avaliações.
- [ ] Documentos e declarações.
- [ ] Mensalidades e assuntos financeiros.
- [ ] Estágio.
- [ ] Regras e procedimentos acadêmicos.
- [ ] Informações sobre cursos e disciplinas.
- [ ] Não costumo procurar essas informações.
- [ ] Outros: ________.

**Pergunta 4 — Quais meios você utiliza para encontrar essas informações?**

Tipo: caixas de seleção e obrigatória.

Instrução: caso selecione "Não utilizo nenhum desses meios", não marque outras alternativas.

- [ ] Site oficial da FEI.
- [ ] Portal do Aluno.
- [ ] Moodle.
- [ ] Pesquisa no Google ou outros buscadores.
- [ ] Contato com secretaria ou outros setores da FEI.
- [ ] Professores ou colegas.
- [ ] Assistentes de inteligência artificial.
- [ ] Não utilizo nenhum desses meios.
- [ ] Outros: ________.

**Pergunta 5 — Com que frequência você encontra dificuldades para localizar ou compreender as informações que procura?**

Tipo: escolha única e obrigatória.

- ( ) Sempre.
- ( ) Frequentemente.
- ( ) Às vezes.
- ( ) Raramente.
- ( ) Nunca.
- ( ) Não sei informar.

**Pergunta 6 — Quando encontra dificuldades, quais situações costumam ocorrer?**

Tipo: caixas de seleção e obrigatória.

Instrução: caso selecione "Não costumo encontrar dificuldades", não marque outras alternativas.

- [ ] Não sei em qual página ou sistema procurar.
- [ ] Preciso consultar diferentes páginas ou documentos.
- [ ] Encontro informações difíceis de compreender.
- [ ] Não consigo identificar se a informação está atualizada.
- [ ] Não encontro orientações completas sobre o procedimento.
- [ ] Preciso entrar em contato com algum setor para esclarecer a dúvida.
- [ ] Não costumo encontrar dificuldades.
- [ ] Outros: ________.

**Pergunta 7 — Você já enfrentou alguma consequência por não encontrar ou compreender corretamente uma informação acadêmica ou administrativa?**

Tipo: caixas de seleção e obrigatória.

Instrução: as opções "Não tive consequências desse tipo" e "Prefiro não responder" devem ser selecionadas isoladamente.

- [ ] Perdi ou quase perdi um prazo.
- [ ] Realizei alguma etapa de um procedimento incorretamente.
- [ ] Precisei procurar atendimento adicional para esclarecer a situação.
- [ ] Gastei mais tempo do que esperava para resolver uma dúvida.
- [ ] Não tive consequências desse tipo.
- [ ] Prefiro não responder.
- [ ] Outros: ________.

**Pergunta 8 — Ao consultar uma informação acadêmica, quais elementos você considera importantes para avaliar sua confiabilidade?**

Tipo: caixas de seleção e obrigatória.

Instrução: caso selecione "Não costumo verificar a confiabilidade dessas informações", não marque outras alternativas.

- [ ] Identificação da fonte institucional.
- [ ] Link para consultar a informação original.
- [ ] Clareza e detalhamento da resposta.
- [ ] Indicação da data ou atualização da informação.
- [ ] Possibilidade de confirmar a informação com um setor responsável.
- [ ] Não costumo verificar a confiabilidade dessas informações.
- [ ] Outros: ________.

**Pergunta 9 — Por qual dispositivo você costuma acessar informações acadêmicas?**

Tipo: caixas de seleção e obrigatória.

- [ ] Celular.
- [ ] Notebook.
- [ ] Computador de mesa.
- [ ] Tablet.
- [ ] Outros: ________.

**Pergunta 10 — Quais das seguintes necessidades você considera prioritárias ao utilizar uma possível ferramenta digital de consulta acadêmica?**

Tipo: caixas de seleção e obrigatória.

Instrução: as alternativas representam possibilidades de estudo, não funcionalidades garantidas. Caso selecione "Não considero necessária uma nova ferramenta" ou "Não sei informar", não marque outras alternativas.

- [ ] Fazer perguntas utilizando linguagem natural.
- [ ] Consultar as fontes utilizadas nas respostas.
- [ ] Visualizar orientações organizadas em etapas.
- [ ] Recuperar consultas realizadas anteriormente.
- [ ] Acessar informações pelo celular.
- [ ] Encontrar orientações para contatar o setor responsável quando necessário.
- [ ] Não considero necessária uma nova ferramenta para esse tipo de consulta.
- [ ] Não sei informar.
- [ ] Outros: ________.

**Pergunta 11 — Caso queira, descreva uma dificuldade que já tenha enfrentado ao procurar informações acadêmicas ou administrativas da FEI.**

Tipo: resposta aberta e opcional.

Instrução: não inclua informações pessoais ou dados identificáveis de terceiros.

__________________________________________________

**Pergunta 12 — Com que frequência você utiliza assistentes conversacionais ou ferramentas de inteligência artificial, como ChatGPT, Gemini ou similares?**

Tipo: escolha única e obrigatória.

- ( ) Diariamente.
- ( ) Algumas vezes por semana.
- ( ) Algumas vezes por mês.
- ( ) Raramente.
- ( ) Já utilizei, mas não utilizo atualmente.
- ( ) Nunca utilizei.

**Pergunta 13 — Para quais finalidades você utiliza ou já utilizou assistentes conversacionais ou ferramentas de inteligência artificial?**

Tipo: caixas de seleção e obrigatória.

Instrução: caso selecione "Nunca utilizei essas ferramentas", não marque outras alternativas.

- [ ] Esclarecimento de dúvidas acadêmicas.
- [ ] Pesquisa de informações.
- [ ] Auxílio em estudos e atividades acadêmicas.
- [ ] Programação e resolução de problemas.
- [ ] Atividades profissionais.
- [ ] Dúvidas e tarefas do cotidiano.
- [ ] Nunca utilizei essas ferramentas.
- [ ] Outros: ________.

**Pergunta 14 — Entre as necessidades apresentadas na pergunta 10, qual você considera mais importante e por quê?**

Tipo: resposta aberta e opcional.

__________________________________________________

**Pergunta 15 — Em qual etapa da graduação você está atualmente?**

Tipo: escolha única e obrigatória.

- ( ) 1º ou 2º semestre.
- ( ) 3º ou 4º semestre.
- ( ) 5º ou 6º semestre.
- ( ) 7º ou 8º semestre.
- ( ) 9º semestre ou superior.
- ( ) Prefiro não responder.

**Pergunta 16 — Crie um código anônimo de identificação da sua resposta.**

Tipo: resposta curta e obrigatória.

Instrução: escolha um código aleatório de oito caracteres, utilizando letras e números. Não utilize seu nome, RA, data de nascimento ou outros dados pessoais. Guarde esse código caso deseje solicitar a exclusão da resposta antes da consolidação dos resultados.

__________________________________________________

**Mensagem de encerramento:**

Obrigado!

Sua participação, caso tenha respondido ao questionário, poderá contribuir para compreender as necessidades dos estudantes da FEI e orientar decisões de interação relacionadas ao projeto acadêmico de IHC.

Caso deseje solicitar a exclusão de uma resposta antes da consolidação dos resultados, entre em contato com a equipe responsável utilizando o código anônimo informado durante o preenchimento.

#### Como os dados serão analisados

Caso o questionário seja aplicado, os dados serão analisados por meio de uma abordagem predominantemente descritiva, considerando as respostas obtidas em cada pergunta.

As questões fechadas serão organizadas em tabelas de frequência e percentuais, permitindo identificar padrões relacionados aos canais utilizados, assuntos mais procurados e dificuldades relatadas pelos estudantes.

Nas perguntas de múltiplas respostas, cada alternativa será contabilizada individualmente, considerando que um mesmo participante poderá selecionar mais de uma resposta.

As perguntas abertas serão analisadas por agrupamento temático, identificando problemas recorrentes, dificuldades específicas e necessidades não contempladas pelas alternativas fechadas.

Antes da análise, serão adotados os seguintes procedimentos:

- Excluir os registros utilizados exclusivamente para testar o formulário.
- Excluir registros de pessoas que não concordaram com o consentimento ou que não pertencem ao público-alvo.
- Excluir da análise principal respostas incompletas em campos essenciais.
- Não considerar campos opcionais em branco como respostas negativas.
- Identificar respostas incompatíveis nas questões que possuem alternativas mutuamente exclusivas.
- Desconsiderar a questão afetada quando houver incompatibilidade entre alternativas, registrando a quantidade de respostas válidas utilizada em cada cálculo.
- Analisar as respostas da alternativa "Outros" por agrupamento temático.
- Organizar as respostas abertas das perguntas 11 e 14 em temas recorrentes.
- Comparar descritivamente as respostas de estudantes de diferentes períodos, quando houver dados suficientes.
- Não utilizar o código anônimo de exclusão como variável de análise.

Os resultados serão relacionados às hipóteses documentadas na Entrega 1 e no arquivo `RASTREABILIDADE.md`, permitindo avaliar:

| Hipótese | Aspecto investigado | Possível utilização dos resultados |
|---|---|---|
| H04/H05 | Frequência e tipos de consultas acadêmicas. | Revisar a relevância e a priorização das tarefas propostas. |
| H06/H10/H16 | Consequências de informações não encontradas ou compreendidas incorretamente. | Orientar mecanismos de prevenção de erros e apresentação de orientações. |
| H07/H08 | Canais utilizados e dificuldades na localização de informações. | Avaliar a necessidade de centralização das consultas. |
| H09 | Dificuldades de compreensão das informações. | Orientar a apresentação de respostas e procedimentos. |
| H02/H14 | Elementos associados à confiabilidade das informações. | Orientar a apresentação de referências e fontes institucionais. |
| H12 | Dispositivos utilizados. | Apoiar decisões relacionadas à adaptação da interface. |
| H15 | Interesse na recuperação de consultas anteriores. | Investigar a relevância do histórico de conversas entre sessões. |
| H18 | Frequência e finalidade de utilização de assistentes conversacionais e ferramentas de IA. | Investigar a familiaridade declarada com o padrão conversacional adotado. |

A investigação da hipótese H15 estará relacionada à recuperação de conversas entre sessões distintas. Esse aspecto não será confundido com a continuidade do contexto durante uma mesma conversa.

A hipótese H11, relacionada ao contexto físico de utilização, permanecerá aberta, pois a identificação dos dispositivos utilizados não permite determinar diretamente o local em que as consultas ocorrem.

A análise deverá considerar as limitações da amostra, evitando generalizações para todos os estudantes da FEI caso a participação seja restrita.

As hipóteses poderão ser classificadas como sustentadas, refutadas ou refinadas conforme as evidências efetivamente obtidas, preservando o histórico das decisões de projeto.

Como a coleta não foi realizada nesta etapa, nenhuma hipótese será considerada confirmada ou refutada com base na publicação ou na validação funcional do questionário.

### Instrumento I02 — Classificação de Cartões (Card Sorting)

**Autor(a):** João Pedro Sabino Garcia — 22.224.032-7  
**Técnica:** Classificação de Cartões (Card Sorting aberto).  
**Objetivo:** Investigar como os estudantes da FEI organizam e relacionam assuntos acadêmicos e administrativos, identificando agrupamentos e nomenclaturas que possam orientar a organização das informações no Assistente Virtual FEI.  
**Público:** Estudantes de graduação da FEI.

#### Procedimento padronizado de aplicação

1. **Preparação:** imprimir e recortar os 16 cartões contendo assuntos acadêmicos e administrativos relacionados ao contexto da FEI. Os cartões deverão apresentar apenas os nomes dos assuntos, sem categorias previamente definidas. Preparar uma mesa, folhas em branco, caneta e ficha de registro para que os participantes possam organizar os cartões em grupos e atribuir nomes aos agrupamentos.

2. **Apresentação/consentimento:** apresentar aos participantes o objetivo acadêmico da pesquisa e explicar que a atividade pretende compreender como eles organizam diferentes informações institucionais. Informar que não existem respostas certas ou erradas e solicitar o consentimento voluntário antes do início.

3. **Aplicação:** disponibilizar os cartões ao participante e solicitar que organize os assuntos em grupos que considere relacionados. Cada grupo deverá receber um nome escolhido pelo próprio participante. A atividade será realizada individualmente, sem interferência do pesquisador nas decisões de classificação. O tempo estimado será de 10 a 15 minutos. O pesquisador poderá esclarecer apenas questões operacionais, como a movimentação dos cartões e o preenchimento dos nomes dos grupos, sem sugerir agrupamentos ou interpretar os assuntos pelo participante.

4. **Encerramento:** após a organização dos cartões, solicitar que o participante revise seus agrupamentos e confirme se representam adequadamente sua forma de compreender os assuntos apresentados. Caso a atividade não seja concluída dentro do tempo planejado, registrar a sessão como parcial. Finalizar com uma mensagem de agradecimento.

5. **Armazenamento/anonimização:** caso a atividade seja aplicada, registrar os agrupamentos e as nomenclaturas atribuídas, identificando cada participante por um código anônimo, como CS01, CS02 ou CS03. Os registros serão transcritos para uma planilha padronizada de acesso restrito, contendo os grupos, cartões associados e observações relevantes. Não serão realizadas gravações de áudio ou vídeo.

#### Instrumento

**Título da atividade:** Organização de informações acadêmicas da FEI.

**Texto de apresentação:**

Esta atividade faz parte de um projeto acadêmico da disciplina de Interação Humano-Computador (IHC), cujo objetivo é investigar como os estudantes compreendem e organizam diferentes assuntos relacionados à vida acadêmica na FEI.

Você receberá um conjunto de cartões contendo assuntos acadêmicos e administrativos.

Sua tarefa será organizar esses cartões em grupos, considerando quais assuntos fazem sentido juntos, e atribuir um nome a cada agrupamento.

Não existem respostas certas ou erradas. O interesse da pesquisa está em compreender sua percepção sobre a organização dessas informações.

A participação é voluntária e a atividade leva aproximadamente 10 a 15 minutos. Não serão solicitados dados de identificação pessoal.

A participação, recusa ou interrupção não terá impacto sobre notas, avaliações ou benefícios acadêmicos.

Você poderá interromper a atividade a qualquer momento e solicitar a exclusão de seu registro antes da consolidação dos resultados, utilizando o código anônimo atribuído à sessão.

Os dados serão utilizados exclusivamente para fins acadêmicos, armazenados em ambiente de acesso restrito e descartados após a análise e avaliação da atividade.

Os responsáveis pela atividade são João Pedro Sabino Garcia e Matheus Dourado Valle. O contato da equipe será disponibilizado antes da aplicação.

**Consentimento**

Você concorda voluntariamente em participar desta atividade, considerando as informações apresentadas?

- ( ) Sim, concordo.
- ( ) Não concordo.

Caso a resposta seja negativa, a atividade deverá ser encerrada.

**Cartões disponibilizados para classificação**

| ID | Conteúdo do cartão |
|---|---|
| C01 | Matrícula |
| C02 | Rematrícula |
| C03 | Calendário acadêmico |
| C04 | Horários das aulas |
| C05 | Notas e avaliações |
| C06 | Frequência nas disciplinas |
| C07 | Histórico escolar |
| C08 | Declaração de matrícula |
| C09 | Solicitação de documentos |
| C10 | Mensalidades |
| C11 | Bolsas e descontos |
| C12 | Estágio obrigatório |
| C13 | Aproveitamento de disciplinas |
| C14 | Trancamento de matrícula |
| C15 | Biblioteca |
| C16 | Contato com a secretaria acadêmica |

Os cartões serão apresentados sem categorias predefinidas, permitindo que o participante escolha livremente como organizar os assuntos.

**Tabuleiro de classificação e material de aplicação**

A atividade será realizada presencialmente, utilizando cartões impressos e um espaço livre para organização dos agrupamentos.

O tabuleiro deverá permitir que o participante:

- Visualize inicialmente os 16 cartões sem agrupamentos.
- Mova livremente cada cartão para o espaço de organização.
- Crie novos grupos conforme considerar necessário.
- Atribua nomes aos grupos utilizando folhas em branco.
- Revise e modifique os agrupamentos antes de finalizar.
- Entregue o resultado ao pesquisador para registro.

Representação do funcionamento do tabuleiro:

| Área inicial | Área de organização livre |
|---|---|
| 16 cartões apresentados sem categorias. | Espaço para criação e nomeação dos grupos pelo participante. |
| Cartões disponíveis para movimentação. | Cartões organizados conforme as relações identificadas pelo participante. |

O espaço não apresentará categorias previamente estabelecidas, evitando induzir os agrupamentos realizados.

**Instruções para o participante**

1. Leia os 16 cartões disponibilizados.
2. Organize os cartões em grupos que façam sentido para você.
3. Coloque juntos os assuntos que considera relacionados.
4. Crie quantos grupos julgar necessários.
5. Atribua um nome a cada grupo utilizando palavras que considere claras e intuitivas.
6. Revise sua organização antes de finalizar.

Não será exigido um número mínimo ou máximo de grupos. Cada cartão deverá ser colocado em apenas um grupo.

Caso o participante apresente dificuldade operacional, o pesquisador poderá explicar como movimentar os cartões ou registrar o nome de um grupo, sem interferir nas decisões de classificação.

**Registro dos agrupamentos**

O resultado de cada participante deverá ser registrado utilizando a seguinte estrutura:

| Campo | Registro |
|---|---|
| Código anônimo do participante | CS___ |
| Data da sessão | ___ |
| Consentimento | Sim / Não |
| Tempo aproximado | ___ |
| Resultado da atividade | Completa / Parcial |
| Auxílio operacional oferecido | ___ |

| Grupo criado | Nome atribuído pelo participante | Cartões incluídos |
|---|---|---|
| Grupo 1 | Preenchido pelo participante | IDs dos cartões selecionados |
| Grupo 2 | Preenchido pelo participante | IDs dos cartões selecionados |
| Grupo 3 | Preenchido pelo participante | IDs dos cartões selecionados |
| Outros grupos, se necessários | Preenchido pelo participante | IDs dos cartões selecionados |

O pesquisador deverá conferir se todos os cartões foram registrados apenas uma vez. Em sessões completas, os 16 cartões deverão estar associados aos grupos criados pelo participante.

Em sessões parciais, deverão ser identificados os cartões que não foram classificados.

Os registros serão transcritos para uma planilha de acesso restrito, utilizando exclusivamente o código anônimo correspondente à sessão.

**Perguntas de encerramento**

Após concluir os agrupamentos, o participante deverá responder:

**1. Algum cartão apresentou dificuldade de interpretação?**

- ( ) Sim.
- ( ) Não.

Se sim, qual(is)?

Resposta aberta: ______________________________

**2. Você encontrou dificuldade para decidir em qual grupo colocar algum assunto?**

- ( ) Sim.
- ( ) Não.

Se sim, qual(is)?

Resposta aberta: ______________________________

**3. Existe algum assunto acadêmico ou administrativo que você considera importante e que não apareceu nos cartões?**

Resposta aberta e opcional: ______________________________

**Mensagem de encerramento:**

Agradecemos sua participação! Sua contribuição poderá ajudar a compreender como os estudantes organizam mentalmente os assuntos acadêmicos e administrativos, orientando decisões relacionadas à organização das informações no Assistente Virtual FEI.

#### Como os dados serão analisados

Caso a atividade seja aplicada, os resultados serão analisados por meio da comparação dos agrupamentos realizados pelos participantes.

Inicialmente, serão registrados os grupos criados, os nomes atribuídos e os cartões associados a cada categoria.

Em seguida, será realizada uma análise comparativa para identificar assuntos frequentemente agrupados, possíveis diferenças de interpretação e nomenclaturas recorrentes.

Para cada par de cartões, será contabilizada a quantidade de sessões completas em que ambos foram inseridos no mesmo grupo.

A frequência de associação será calculada dividindo a quantidade de sessões em que os cartões foram agrupados conjuntamente pelo total de sessões completas válidas.

Serão preservadas as contagens absolutas e os percentuais correspondentes, considerando as limitações da amostra.

Os nomes atribuídos aos grupos serão comparados semanticamente, identificando nomenclaturas semelhantes, sem eliminar os registros originais produzidos pelos participantes.

As classificações divergentes serão analisadas separadamente, buscando compreender possíveis ambiguidades ou diferenças entre os modelos mentais dos estudantes.

Sessões parciais serão registradas e analisadas qualitativamente, sem serem incluídas no cálculo principal de frequência de associação.

A análise considerará:

- Frequência com que determinados cartões aparecem em um mesmo grupo.
- Semelhanças entre os nomes atribuídos às categorias.
- Assuntos que apresentam diferentes interpretações entre os participantes.
- Cartões que geraram dúvidas ou dificuldades de classificação.
- Sugestões de novos assuntos apresentadas nas perguntas de encerramento.

As respostas abertas serão analisadas por agrupamento temático, permitindo identificar dificuldades de compreensão, ambiguidades e necessidades informacionais não previstas inicialmente.

Os resultados serão relacionados às hipóteses estabelecidas na Entrega 1 e documentadas no arquivo `RASTREABILIDADE.md`.

| Hipótese | Aspecto investigado | Possível utilização dos resultados |
|---|---|---|
| H04/H05 | Organização dos assuntos acadêmicos considerados relevantes pelos estudantes. | Revisar a priorização dos conteúdos e exemplos de perguntas disponíveis. |
| H07/H08 | Relações estabelecidas entre diferentes informações acadêmicas. | Orientar sugestões de assuntos relacionados durante as consultas. |
| H09 | Compreensão e interpretação das nomenclaturas institucionais. | Definir uma linguagem mais próxima do vocabulário utilizado pelos estudantes. |

Os resultados poderão contribuir para sustentar, refutar ou refinar as hipóteses investigadas, considerando as evidências efetivamente obtidas.

As decisões de design derivadas dessa técnica deverão estar relacionadas a elementos efetivamente previstos na interface conversacional, especialmente exemplos de perguntas, sugestões de assuntos e terminologias utilizadas pelo assistente.

A técnica não será utilizada para justificar a criação de menus ou categorias obrigatórias sem evidências adicionais de necessidade.

A análise deverá reconhecer as limitações da amostra, evitando generalizar os agrupamentos realizados por um número restrito de participantes para todos os estudantes da FEI.

Até a realização da atividade, as hipóteses permanecerão pendentes de validação empírica, não sendo utilizados agrupamentos fictícios como evidências de pesquisa.

## Síntese

O conjunto de técnicas proposto pretende reduzir as lacunas de conhecimento relacionadas aos hábitos, necessidades, dificuldades e modelos mentais dos estudantes da FEI durante a busca por informações acadêmicas e administrativas.

Os dois instrumentos possuem objetivos complementares:

- **I01 — Questionário (Matheus Dourado Valle):** investigar a frequência das consultas, os principais canais utilizados, os assuntos procurados, as dificuldades enfrentadas, a familiaridade com assistentes conversacionais e os elementos considerados importantes pelos estudantes durante a obtenção de informações institucionais.

- **I02 — Classificação de Cartões (João Pedro Sabino Garcia):** investigar como os estudantes compreendem, relacionam e organizam diferentes assuntos acadêmicos e administrativos, identificando agrupamentos e nomenclaturas que possam orientar decisões relacionadas às sugestões de assuntos, exemplos de perguntas e linguagem do Assistente Virtual FEI.

A combinação das técnicas permitirá investigar não apenas quais informações os estudantes procuram, mas também como compreendem e organizam esses conteúdos.

O questionário contribuirá principalmente para a investigação das hipóteses H04, H05, H06, H07, H08, H09, H10, H12, H14, H15, H16 e H18, relacionadas às necessidades de consulta, dificuldades de utilização, confiabilidade das respostas, dispositivos utilizados, familiaridade com assistentes conversacionais e possíveis consequências de erros.

A classificação de cartões contribuirá especialmente para investigar as hipóteses H04, H05, H07, H08 e H09, relacionadas à organização das informações, compreensão dos assuntos acadêmicos e utilização de nomenclaturas intuitivas.

Após eventual aplicação e análise dos instrumentos, as hipóteses deverão ser classificadas como:

- **Sustentadas:** quando os dados coletados apresentarem evidências favoráveis à hipótese inicialmente estabelecida.
- **Refutadas:** quando as evidências obtidas contrariarem a hipótese formulada.
- **Refinadas:** quando os resultados indicarem necessidade de ajustes ou maior especificidade na hipótese original.

Até a realização da coleta, as hipóteses permanecerão pendentes de validação empírica, não sendo considerados resultados presumidos como evidências de confirmação.

Os resultados deverão ser interpretados considerando as limitações da amostra e do contexto acadêmico investigado, evitando generalizações indevidas para todos os estudantes da FEI.

Quando os dados forem efetivamente coletados e analisados, o histórico correspondente deverá ser atualizado em `RASTREABILIDADE.md`, preservando as decisões de projeto e as evidências associadas.

Após o feedback do professor, o questionário foi implementado no Google Forms, publicado por meio de um link público e validado funcionalmente pela equipe. Foram também refinados os aspectos éticos, os procedimentos de recrutamento, as perguntas relacionadas à familiaridade com inteligência artificial e os critérios de análise dos dados.

O instrumento de classificação de cartões foi complementado com a definição da modalidade de aplicação, dos materiais necessários, do tabuleiro, do protocolo de condução, da ficha de registro e dos critérios de análise comparativa.

| Instrumento | Responsável | Situação do instrumento | Situação da coleta |
|---|---|---|---|
| I01 — Questionário | Matheus Dourado Valle | Implementado, publicado e validado funcionalmente. | Não realizada. |
| I02 — Classificação de Cartões | João Pedro Sabino Garcia | Planejamento, material textual de aplicação e procedimento de registro definidos. | Não realizada. |

A Entrega 7 encontra-se concluída quanto ao planejamento e à preparação dos instrumentos. A equipe optou por não realizar a coleta de dados nesta etapa, mantendo as hipóteses investigadas abertas e preservando a distinção entre planejamento, validação funcional e evidência empírica.

## Checklist

- [x] Hipóteses/lacunas prioritárias da Entrega 1 foram revisitadas.
- [x] Se o escopo de IHC foi derivado de TCC técnico, a coleta investiga a plausibilidade do usuário, tarefa e contexto adotados.
- [x] Perguntas não pressupõem que dashboard, CRUD, filtros ou relatórios sejam necessários; investigam a necessidade.
- [x] Cada dado a coletar responde uma dúvida concreta do projeto ou justifica outra necessidade de informação.
- [x] Parte A identifica dados e perfis de coleta de forma específica.
- [x] Aspectos éticos são contextualizados para o projeto.
- [x] Há uma técnica completa por integrante e técnicas distintas.
- [x] Questionário está incluído entre as técnicas.
- [x] Cada instrumento possui objetivo, público, procedimento e conteúdo integral.
- [x] Perguntas evitam indução e coletam apenas dados necessários.
- [x] Está claro como os dados serão analisados e usados no design.
