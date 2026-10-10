# Entrega 7 — Coleta de dados, necessidades e aspectos éticos

**Data:** 10/10/2026  
**Status:** 🟨 em andamento

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

As personas e os cenários definidos anteriormente serão tratados como hipóteses de projeto, e não como evidências suficientes para confirmar as necessidades do público-alvo.

## Hipóteses e lacunas prioritárias herdadas da Entrega 1

As hipóteses estabelecidas anteriormente orientam a definição dos dados necessários e das perguntas presentes no instrumento de coleta.

| ID | Hipótese/lacuna | Evidência atual | Decisão que depende da resposta | Prioridade |
|---|---|---|---|---|
| H04/H05 | Necessidades relacionadas à frequência e aos tipos de consultas acadêmicas. | Hipóteses e cenários definidos nas entregas anteriores, ainda sem validação direta com usuários. | Priorização das tarefas e dos conteúdos contemplados pela interface. | Alta |
| H07/H08 | Dificuldades relacionadas aos canais utilizados e à localização de informações institucionais. | Análise inicial do contexto de utilização e dos canais institucionais existentes. | Organização do fluxo de consulta e apresentação das informações. | Alta |
| H09 | Possíveis dificuldades de compreensão das informações acadêmicas. | Hipótese de projeto ainda não verificada diretamente com estudantes. | Definição da linguagem e da estrutura das respostas. | Alta |
| H02/H14 | Necessidade de apresentar fontes institucionais para apoiar a confiabilidade das respostas. | Requisito considerado na proposta inicial do assistente virtual. | Forma de exibição das fontes consultadas e referências institucionais. | Alta |
| H11/H12 | Necessidades relacionadas aos dispositivos utilizados pelos estudantes. | Contexto de uso previsto nas entregas anteriores. | Adaptação da interface para diferentes dispositivos. | Média |
| H15 | Necessidade de recuperar informações consultadas anteriormente. | Funcionalidade considerada no projeto, ainda sem confirmação de sua relevância para os usuários. | Priorização do histórico de conversas. | Média |
| H06/H10/H16 | Possíveis consequências de erros ou dificuldades durante a obtenção de informações acadêmicas. | Riscos considerados nos cenários e hipóteses anteriores. | Definição de mecanismos de prevenção de erros e apresentação de orientações. | Alta |

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
| Dispositivos utilizados para realizar consultas. | H11/H12 | Compreender o contexto tecnológico de utilização. | Adaptação da interface para diferentes dispositivos. |
| Necessidade de recuperar informações consultadas anteriormente. | H15 | Investigar se o histórico de consultas representa uma necessidade real dos estudantes. | Priorização do recurso de histórico e recuperação de conversas. |

#### De quem coletar?

O público principal será composto por estudantes de graduação da FEI, considerando que o assistente virtual foi proposto para apoiar a resolução de dúvidas acadêmicas e administrativas desse público.

| Perfil/stakeholder | Critério de inclusão | Relação com persona/público |
|---|---|---|
| Estudantes de graduação da FEI. | Estar regularmente matriculado em um curso de graduação da instituição e concordar voluntariamente em participar da pesquisa. | Público principal representado pelas personas P01 — Lucas Almeida e P02 — Mariana Costa. |
| Estudantes de diferentes períodos da graduação. | Estar em qualquer etapa do curso, preferencialmente contemplando experiências distintas com os serviços institucionais. | Permite investigar se as necessidades variam conforme a experiência acadêmica. |

A participação de estudantes de diferentes períodos poderá contribuir para identificar necessidades relacionadas tanto à adaptação à instituição quanto a procedimentos acadêmicos específicos de etapas mais avançadas da graduação.

As personas utilizadas anteriormente representam hipóteses de perfis de usuários, não sendo consideradas evidências suficientes para confirmar suas necessidades reais.

#### Aspectos éticos

A coleta de dados deverá respeitar a privacidade, a autonomia e a participação voluntária dos estudantes, considerando os princípios éticos discutidos na disciplina e a Lei Geral de Proteção de Dados (LGPD).

- **Voluntariedade e consentimento:** antes do preenchimento do questionário, os participantes receberão uma explicação sobre o objetivo acadêmico da pesquisa e a utilização pretendida das respostas. A participação será voluntária, sem qualquer prejuízo em caso de recusa.

- **Minimização de dados:** o questionário não solicitará nome completo, matrícula, CPF, telefone, endereço ou outras informações pessoais que não sejam necessárias para compreender as necessidades investigadas. Será solicitado apenas que o respondente confirme pertencer ao público-alvo da pesquisa.

- **Privacidade e riscos:** como o estudo aborda experiências com serviços acadêmicos, existe a possibilidade de participantes mencionarem dificuldades relacionadas a setores ou procedimentos institucionais. Para reduzir riscos de exposição, será solicitado que não sejam compartilhados dados pessoais, situações identificáveis de terceiros ou informações acadêmicas sigilosas.

- **Gravação:** a técnica escolhida não prevê gravação de áudio ou vídeo.

- **Anonimização:** as respostas serão analisadas de forma agregada. Eventuais exemplos textuais utilizados na documentação serão revisados para evitar a identificação de participantes ou terceiros.

- **Armazenamento:** caso o questionário seja aplicado, os dados serão armazenados em ambiente digital com acesso restrito aos integrantes responsáveis pela atividade. O formulário será configurado para não coletar automaticamente endereços de e-mail.

- **Descarte:** os registros individuais serão mantidos apenas durante o período necessário à análise e avaliação acadêmica da atividade, sendo posteriormente excluídos. A documentação final poderá preservar resultados agregados e não identificáveis.

A pesquisa não será utilizada para avaliar individualmente estudantes, professores ou funcionários da FEI.

## Parte B — ferramentas de coleta

> Cada integrante deve preparar uma técnica/instrumento completo. As técnicas devem ser diferentes entre si e **questionário deve estar entre as técnicas escolhidas**, conforme o enunciado da disciplina.

### Instrumento I01 — Questionário

**Autor(a):** Matheus Dourado Valle — 22.224.023-6  
**Técnica:** Questionário estruturado, com perguntas fechadas e abertas.  
**Objetivo:** Investigar os hábitos, necessidades e dificuldades dos estudantes da FEI durante a busca por informações acadêmicas e administrativas, contribuindo para a avaliação das hipóteses estabelecidas nas entregas anteriores.  
**Público:** Estudantes de graduação da FEI.

#### Procedimento padronizado de aplicação

1. **Preparação:** elaborar um formulário digital utilizando o Google Forms, preservando a ordem, as alternativas e as orientações estabelecidas neste instrumento. Antes da disponibilização, verificar a clareza das perguntas, o funcionamento do formulário e a configuração de privacidade, desabilitando a coleta automática de endereços de e-mail.

2. **Apresentação/consentimento:** apresentar uma breve explicação sobre o objetivo da pesquisa, seu caráter acadêmico e a participação voluntária. O participante deverá manifestar concordância antes de acessar as perguntas.

3. **Aplicação:** disponibilizar o questionário digitalmente aos estudantes da FEI. Cada participante responderá individualmente, sem necessidade de acompanhamento por um pesquisador. O tempo estimado de preenchimento será de 5 a 8 minutos.

4. **Encerramento:** apresentar uma mensagem de agradecimento ao finalizar o formulário, sem solicitar dados pessoais adicionais ou justificativas sobre as respostas fornecidas.

5. **Armazenamento/anonimização:** caso a coleta seja realizada, exportar os dados para análise e mantê-los em ambiente de acesso restrito. Os resultados poderão ser utilizados em tabelas, gráficos e sínteses textuais, evitando qualquer identificação individual.

#### Instrumento

**Título do questionário:** Pesquisa sobre a busca de informações acadêmicas na FEI.

**Texto de apresentação:**

Este questionário faz parte de uma atividade acadêmica da disciplina de Interação Humano-Computador (IHC), cujo projeto investiga as necessidades dos estudantes da FEI relacionadas à busca por informações acadêmicas e administrativas.

O objetivo é compreender como essas informações são procuradas atualmente, quais dificuldades podem ocorrer e quais necessidades devem ser consideradas no desenvolvimento de uma possível solução digital.

A participação é voluntária e o preenchimento leva aproximadamente 5 a 8 minutos. Não serão solicitados nome, matrícula ou outros dados de identificação pessoal. As respostas serão utilizadas exclusivamente para fins acadêmicos.

Ao responder, evite mencionar informações pessoais ou dados identificáveis de terceiros.

**Consentimento**

Você concorda voluntariamente em participar desta pesquisa, considerando as informações apresentadas?

- ( ) Sim, concordo.
- ( ) Não concordo.

Caso a resposta seja negativa, o formulário deverá ser encerrado.

**Pergunta 1 — Você é estudante de graduação da FEI?**

Tipo: escolha única.

- ( ) Sim.
- ( ) Não.

Caso a resposta seja negativa, o formulário deverá ser encerrado, pois o participante não pertence ao público-alvo definido.

**Pergunta 2 — Com que frequência você costuma procurar informações acadêmicas ou administrativas relacionadas à FEI?**

Tipo: escolha única.

- ( ) Diariamente.
- ( ) Algumas vezes por semana.
- ( ) Algumas vezes por mês.
- ( ) Raramente.
- ( ) Nunca.
- ( ) Não sei informar.

**Pergunta 3 — Quais tipos de informações você costuma procurar?**

Tipo: múltipla escolha.

- [ ] Matrícula e rematrícula.
- [ ] Calendário acadêmico.
- [ ] Notas e avaliações.
- [ ] Documentos e declarações.
- [ ] Mensalidades e assuntos financeiros.
- [ ] Estágio.
- [ ] Regras e procedimentos acadêmicos.
- [ ] Informações sobre cursos e disciplinas.
- [ ] Outros: ________.
- [ ] Não costumo procurar essas informações.

**Pergunta 4 — Quais meios você utiliza para encontrar essas informações?**

Tipo: múltipla escolha.

- [ ] Site oficial da FEI.
- [ ] Portal do Aluno.
- [ ] Moodle.
- [ ] Pesquisa no Google ou outros buscadores.
- [ ] Contato com secretaria ou outros setores da FEI.
- [ ] Professores ou colegas.
- [ ] Assistentes de inteligência artificial.
- [ ] Outros: ________.
- [ ] Não utilizo nenhum desses meios.

**Pergunta 5 — Com que frequência você encontra dificuldades para localizar ou compreender as informações que procura?**

Tipo: escolha única.

- ( ) Sempre.
- ( ) Frequentemente.
- ( ) Às vezes.
- ( ) Raramente.
- ( ) Nunca.
- ( ) Não sei informar.

**Pergunta 6 — Quando encontra dificuldades, quais situações costumam ocorrer?**

Tipo: múltipla escolha.

- [ ] Não sei em qual página ou sistema procurar.
- [ ] Preciso consultar diferentes páginas ou documentos.
- [ ] Encontro informações difíceis de compreender.
- [ ] Não consigo identificar se a informação está atualizada.
- [ ] Não encontro orientações completas sobre o procedimento.
- [ ] Preciso entrar em contato com algum setor para esclarecer a dúvida.
- [ ] Outros: ________.
- [ ] Não costumo encontrar dificuldades.

**Pergunta 7 — Você já enfrentou alguma consequência por não encontrar ou compreender corretamente uma informação acadêmica ou administrativa?**

Tipo: múltipla escolha.

- [ ] Perdi ou quase perdi um prazo.
- [ ] Realizei alguma etapa de um procedimento incorretamente.
- [ ] Precisei procurar atendimento adicional para esclarecer a situação.
- [ ] Gastei mais tempo do que esperava para resolver uma dúvida.
- [ ] Não tive consequências desse tipo.
- [ ] Outros: ________.
- [ ] Prefiro não responder.

**Pergunta 8 — Ao consultar uma informação acadêmica, quais elementos você considera importantes para avaliar sua confiabilidade?**

Tipo: múltipla escolha.

- [ ] Identificação da fonte institucional.
- [ ] Link para consultar a informação original.
- [ ] Clareza e detalhamento da resposta.
- [ ] Indicação da data ou atualização da informação.
- [ ] Possibilidade de confirmar a informação com um setor responsável.
- [ ] Outros: ________.
- [ ] Não costumo verificar a confiabilidade dessas informações.

**Pergunta 9 — Por qual dispositivo você costuma acessar informações acadêmicas?**

Tipo: múltipla escolha.

- [ ] Celular.
- [ ] Notebook.
- [ ] Computador de mesa.
- [ ] Tablet.
- [ ] Outros: ________.

**Pergunta 10 — Em uma possível ferramenta digital de consulta acadêmica, quais recursos seriam úteis para você?**

Tipo: múltipla escolha.

- [ ] Fazer perguntas utilizando linguagem natural.
- [ ] Consultar as fontes utilizadas nas respostas.
- [ ] Visualizar orientações organizadas em etapas.
- [ ] Recuperar consultas realizadas anteriormente.
- [ ] Acessar informações pelo celular.
- [ ] Encontrar orientações para contatar o setor responsável quando necessário.
- [ ] Outros: ________.
- [ ] Não considero necessária uma nova ferramenta para esse tipo de consulta.
- [ ] Não sei informar.

**Pergunta 11 — Caso queira, descreva uma dificuldade que já tenha enfrentado ao procurar informações acadêmicas ou administrativas da FEI.**

Tipo: resposta aberta e opcional.

__________________________________________________

**Mensagem de encerramento:**

Agradecemos sua participação! Suas respostas poderão contribuir para compreender as necessidades dos estudantes e orientar decisões de interação relacionadas ao projeto acadêmico.

#### Como os dados serão analisados

Caso o questionário seja aplicado, os dados serão analisados por meio de uma abordagem predominantemente descritiva, considerando as respostas obtidas em cada pergunta.

As questões fechadas serão organizadas em tabelas de frequência e percentuais, permitindo identificar padrões relacionados aos canais utilizados, assuntos mais procurados e dificuldades relatadas pelos estudantes.

Nas perguntas de múltipla escolha, cada alternativa será contabilizada individualmente, considerando que um mesmo participante poderá selecionar mais de uma resposta.

A pergunta aberta será analisada por agrupamento temático, identificando problemas recorrentes, dificuldades específicas e necessidades não contempladas pelas alternativas fechadas.

Os resultados serão relacionados às hipóteses documentadas na Entrega 1 e no arquivo `RASTREABILIDADE.md`, permitindo avaliar:

| Hipótese | Aspecto investigado | Possível utilização dos resultados |
|---|---|---|
| H04/H05 | Frequência e tipos de consultas acadêmicas. | Revisar a relevância e a priorização das tarefas propostas. |
| H06/H10/H16 | Consequências de informações não encontradas ou compreendidas incorretamente. | Orientar mecanismos de prevenção de erros e apresentação de orientações. |
| H07/H08 | Canais utilizados e dificuldades na localização de informações. | Avaliar a necessidade de centralização das consultas. |
| H09 | Dificuldades de compreensão das informações. | Orientar a apresentação de respostas e procedimentos. |
| H02/H14 | Elementos associados à confiabilidade das informações. | Orientar a apresentação de referências e fontes institucionais. |
| H11/H12 | Dispositivos utilizados. | Apoiar decisões relacionadas à adaptação da interface. |
| H15 | Interesse na recuperação de consultas anteriores. | Investigar a relevância do histórico de conversas. |

A análise deverá considerar as limitações da amostra, evitando generalizações para todos os estudantes da FEI caso a participação seja restrita.

As hipóteses poderão ser classificadas como sustentadas, refutadas ou refinadas conforme as evidências efetivamente obtidas, preservando o histórico das decisões de projeto.

## Síntese

A coleta proposta pretende reduzir as lacunas de conhecimento relacionadas aos hábitos, necessidades e dificuldades dos estudantes da FEI durante a busca por informações acadêmicas e administrativas.

O questionário desenvolvido no Instrumento I01 permitirá investigar a frequência das consultas, os principais canais utilizados, os assuntos procurados e os problemas enfrentados pelos estudantes.

Espera-se que os dados obtidos contribuam para avaliar as hipóteses H04, H05, H07, H08 e H09, relacionadas às necessidades de consulta e às dificuldades de localização e compreensão das informações.

Também serão investigadas as hipóteses H02, H14 e H15, referentes à confiabilidade das respostas, apresentação de fontes institucionais e necessidade de recuperação de consultas anteriores.

As hipóteses H06, H10 e H16 serão consideradas na investigação das consequências de erros ou dificuldades durante a obtenção de informações acadêmicas, enquanto H11 e H12 poderão orientar decisões relacionadas aos dispositivos utilizados pelos estudantes.

Após eventual aplicação e análise dos instrumentos, as hipóteses deverão ser classificadas como sustentadas, refutadas ou refinadas, conforme as evidências obtidas.

Até a realização da coleta, as hipóteses permanecerão pendentes de validação empírica, não sendo considerados resultados presumidos como evidências de confirmação.

Quando os dados forem efetivamente coletados e analisados, o histórico correspondente deverá ser atualizado em `RASTREABILIDADE.md`.

## Checklist

- [x] Hipóteses/lacunas prioritárias da Entrega 1 foram revisitadas.
- [x] Se o escopo de IHC foi derivado de TCC técnico, a coleta investiga a plausibilidade do usuário, tarefa e contexto adotados.
- [x] Perguntas não pressupõem que dashboard, CRUD, filtros ou relatórios sejam necessários; investigam a necessidade.
- [x] Cada dado a coletar responde uma dúvida concreta do projeto ou justifica outra necessidade de informação.
- [x] Parte A identifica dados e perfis de coleta de forma específica.
- [x] Aspectos éticos são contextualizados para o projeto.
- [ ] Há uma técnica completa por integrante e técnicas distintas.
- [x] Questionário está incluído entre as técnicas.
- [x] Cada instrumento possui objetivo, público, procedimento e conteúdo integral.
- [x] Perguntas evitam indução e coletam apenas dados necessários.
- [x] Está claro como os dados serão analisados e usados no design.
