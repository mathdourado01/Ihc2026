# Entrega 2 — Público-alvo e análise de concorrência

**Data:** 26/08/2026  
**Status:** 🟨 em andamento 
**Responsabilidade mínima:** cada integrante analisa pelo menos 1 concorrente/interface representativa; a equipe produz síntese comparativa.

## Objetivo da atividade

Compreender soluções do mesmo domínio **e também interfaces familiares ao público-alvo**. O objetivo não é copiar telas, mas identificar convenções, padrões, affordances percebidas, problemas recorrentes, expectativas e oportunidades de design.

> **Concorrente não precisa ser idêntico ao produto.** Pode atuar na mesma área, resolver objetivo semelhante ou disputar a mesma necessidade. Quando não houver concorrente direto, use produtos análogos e softwares que o público já utiliza.

### Para TCCs que não previam interface

Não procure apenas um “concorrente do algoritmo”. Investigue **interfaces profissionais que materializam atividades semelhantes** às que o usuário escolhido precisaria realizar.

Exemplos:

- TCC de banco de dados → consoles de administração, ferramentas para DBA, monitoramento e análise de consultas;
- TCC de LLM/ML → painéis de experimentos, gestão de modelos/datasets, comparação de métricas, revisão de resultados;
- TCC de análise de dados → dashboards, ferramentas de BI, filtros, relatórios e exploração;
- TCC de infraestrutura/API → portais administrativos, observabilidade, logs, gestão de credenciais e uso;
- TCC de cibersegurança → consoles de alertas, triagem, histórico e auditoria.

A pergunta é: **“que convenções esse perfil já conhece para executar tarefas equivalentes?”**

## Entrada obrigatória da Entrega 1

Retome o mapa inicial de alternativas e produtos citado na Entrega 1. Aqui a equipe deixa de trabalhar apenas com impressão inicial e passa a **investigar sistematicamente** cada solução.

| Item citado na Entrega 1 | Tipo | Por que foi citado | Status inicial | Decisão nesta entrega |
|---|---|---|---|---|
| Site, páginas e documentos institucionais da FEI | ferramenta cotidiana | São meios disponíveis para consulta de informações acadêmicas, administrativas, serviços, regras e orientações institucionais | F | analisar |
| Portal e sistemas acadêmicos da instituição | ferramenta cotidiana | Fazem parte do ambiente digital utilizado pelos estudantes para consultar informações e realizar atividades relacionadas à vida acadêmica | F | analisar de forma complementar |
| Canais de atendimento e contato com profissionais da instituição | processo manual | Representam uma alternativa para o estudante buscar esclarecimentos sobre dúvidas acadêmicas e administrativas | F | analisar de forma complementar |
| Mecanismos de busca na Internet | ferramenta cotidiana / análogo | Podem ser utilizados para localizar páginas, documentos ou informações relacionadas a uma dúvida | H | analisar de forma complementar |
| Assistentes de IA de propósito geral, como ChatGPT, Gemini e Copilot | análogo | Permitem realizar perguntas em linguagem natural e obter respostas ou orientações, apresentando um modelo de interação semelhante ao proposto no TCC | H | analisar |

Se uma hipótese da Entrega 1 for confirmada ou refutada durante esta análise, atualize `H01`, `H02`... em [`../RASTREABILIDADE.md`](../RASTREABILIDADE.md).

## 1. Público-alvo desta análise

O público-alvo prioritário desta análise é composto por estudantes da FEI que precisam localizar e compreender informações acadêmicas ou administrativas, como regras, prazos, serviços, orientações institucionais e procedimentos relacionados à vida acadêmica.

Esse público retoma o recorte definido na Entrega 1, na qual o estudante da FEI foi identificado como o usuário direto prioritário do projeto de IHC. Entre as principais atividades consideradas estão a localização e compreensão de informações acadêmico-administrativas e o entendimento de como realizar determinados procedimentos.

Nesta entrega, as soluções serão analisadas considerando principalmente como suas interfaces apoiam atividades de busca, formulação de dúvidas, compreensão de respostas, apresentação de informações e orientação do usuário, além dos padrões de interação que possam ser familiares ou relevantes para esse público.

## 2. Concorrentes diretos/indiretos
### Análise C01 — ChatGPT

**Autor(a):** João Pedro Sabino Garcia — 22.224.032-7
**Tipo:** análogo
**Link oficial:** ChatGPT — OpenAI
**Data de acesso:** 26/08/2026

#### Contexto e proposta

O ChatGPT é um assistente de Inteligência Artificial de propósito geral que permite ao usuário formular perguntas e solicitações em linguagem natural e receber respostas em formato conversacional. A ferramenta pode manter o contexto de uma conversa, receber diferentes tipos de entrada e, quando utiliza pesquisa na web, apresentar citações e links relacionados às fontes consultadas.

Embora não tenha sido desenvolvido especificamente para responder dúvidas acadêmicas e administrativas da FEI, o ChatGPT é relevante como produto análogo por utilizar um modelo de interação semelhante ao proposto no TCC: o usuário apresenta uma dúvida em linguagem natural, recebe uma resposta e pode continuar a interação com novas perguntas.

Para o projeto de IHC, sua análise é especialmente útil para observar padrões de interface conversacional, apresentação de respostas, continuidade do diálogo, acesso a fontes e tratamento de diferentes tipos de entrada.

#### Funcionalidades relevantes

| Funcionalidade                                          | Como é realizada                                                                                                                                   | Evidência/print                                          | Observação de IHC                                                                                                                                 |
| ------------------------------------------------------- | -------------------------------------------------------------------------------------------------------------------------------------------------- | -------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------- |
| Formulação de perguntas em linguagem natural            | O usuário digita sua solicitação em um campo de texto e envia a mensagem para iniciar ou continuar a conversa                                      | print pergunta | O campo de entrada concentra a principal ação da interface e permite que o usuário formule a dúvida com suas próprias palavras                    |
| Resposta em formato conversacional                      | A resposta é apresentada na sequência da pergunta, mantendo a estrutura de diálogo entre usuário e assistente                                      | print resposta     | A associação visual entre pergunta e resposta facilita o acompanhamento da interação e permite perguntas complementares                           |
| Continuidade da conversa                                | O usuário pode realizar novas perguntas no mesmo diálogo, utilizando o contexto das mensagens anteriores                                           | print continuidade | Reduz a necessidade de repetir todo o contexto e permite refinar uma pergunta quando a primeira resposta não é suficiente                         |
| Apresentação de fontes em respostas com pesquisa na web | Quando a pesquisa na web é utilizada, a resposta pode apresentar citações associadas às informações utilizadas e uma área para consulta das fontes | print fontegpt   | A presença de fontes fornece um caminho para que o usuário consulte a origem de determinada informação, padrão especialmente relevante para o TCC |
| Histórico de conversas                                  | Conversas anteriores podem ser retomadas posteriormente por meio da navegação da interface                                                         | print historico    | Pode facilitar a retomada de uma consulta anterior, embora a necessidade desse recurso para os estudantes da FEI ainda precise ser investigada    |

#### Experiência do usuário e opiniões

Estudos com estudantes universitários indicam que a facilidade de uso e a rapidez das respostas estão entre os aspectos positivamente percebidos no uso do ChatGPT. Um estudo publicado em 2025 identificou avaliações positivas para facilidade de uso, rapidez das respostas, disponibilidade e experiência amigável, além da possibilidade de realizar perguntas complementares.

Uma pesquisa multi-institucional publicada em 2026 também identificou que estudantes valorizam o acesso rápido à informação e a possibilidade de esclarecer conceitos. Entretanto, o mesmo estudo registrou preocupações relacionadas a respostas incorretas, dependência excessiva da ferramenta e limitações das versões gratuitas.

Outros estudos sobre uso de ChatGPT no ensino superior também relatam experiências positivas relacionadas à rapidez e facilidade de interação, mas apontam como limitações a ocorrência de imprecisões, dificuldades em determinadas perguntas e necessidade de avaliação crítica das respostas.

Para o projeto, essas evidências indicam que a simplicidade da interação conversacional pode ser uma referência relevante, mas que a facilidade de obter uma resposta não deve ser confundida com garantia de que a informação apresentada esteja correta ou seja adequada ao contexto institucional.

#### Preço/modelo de negócio

O ChatGPT adota um modelo **freemium**, oferecendo uma versão gratuita com limites de utilização e planos pagos que ampliam o acesso a modelos e funcionalidades.

Na data desta análise, o plano ChatGPT Plus é oferecido por **US$ 20 por mês**, enquanto também existem outras modalidades destinadas a diferentes níveis de uso e a organizações.

Para esta análise de IHC, o aspecto mais relevante não é o preço específico dos planos, mas o fato de que determinadas funcionalidades e limites de utilização podem variar conforme a modalidade de acesso do usuário.

#### Padrões e tendências percebidos

Os principais padrões de interação observados são:

* campo de texto como elemento central para iniciar a interação;
* uso de linguagem natural como principal forma de entrada;
* organização da interação em formato de conversa;
* permanência do contexto para realização de perguntas complementares;
* apresentação progressiva de pergunta e resposta em uma mesma sequência;
* possibilidade de consultar fontes quando a resposta utiliza pesquisa externa;
* histórico para retomada de conversas anteriores;
* possibilidade de anexar arquivos e utilizar diferentes formas de entrada.

Esses padrões reduzem a necessidade de o usuário aprender uma estrutura complexa de navegação antes de realizar sua principal tarefa. Entretanto, nem todos devem ser automaticamente incorporados ao projeto da FEI, sendo necessário avaliar sua relação com as atividades A01 e A02 definidas na Entrega 1.

#### Pontos positivos, limitações e lições

| Ponto                                                                                     | Evidência                                                          | Implicação para nosso projeto                                                                                                                                              |
| ----------------------------------------------------------------------------------------- | ------------------------------------------------------------------ | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| A interação principal pode ser iniciada diretamente por uma pergunta em linguagem natural | Interface do ChatGPT e documentação oficial                        | Manter uma forma simples e evidente para o estudante formular sua dúvida pode reduzir etapas desnecessárias antes da tarefa principal                                      |
| A conversa permite perguntas complementares mantendo o contexto anterior                  | Observação da interface                                            | Pode ser interessante permitir que o estudante refine ou complemente uma dúvida sem precisar reiniciar toda a consulta                                                     |
| Respostas provenientes de pesquisa podem apresentar citações e acesso às fontes           | Documentação oficial e print da interface                          | A apresentação da fonte institucional associada à resposta é especialmente relevante para o TCC, no qual a fundamentação documental é parte central da solução             |
| Estudos com universitários apontam rapidez e facilidade de uso como aspectos positivos    | Estudos sobre percepção e utilização do ChatGPT no ensino superior | A interface do projeto deve priorizar um fluxo de consulta simples, com baixa quantidade de etapas entre formular a dúvida e compreender a resposta                        |
| Estudos também relatam preocupação com imprecisões e confiança nas respostas              | Estudos sobre uso do ChatGPT no ensino superior                    | O projeto deve deixar claro o escopo da informação, utilizar fontes institucionais e tratar explicitamente situações em que não existe evidência suficiente para responder |
| O histórico permite retomar conversas anteriores                                          | Interface do ChatGPT                                               | Pode ser uma possibilidade de interação para o projeto, mas não deve ser considerada requisito até que sua utilidade para os estudantes seja investigada                   |
### Análise C02 — Virtual University Support Agent

**Autor(a):** Matheus Dourado Valle — 22.224.023-6  
**Tipo:** direto  
**Link oficial:** https://www.sciencedirect.com/science/article/pii/S1877050924015217  
**Data de acesso:** 27/08/2026

#### Contexto e proposta

O trabalho de Ilagan e Ilagan (2024) apresenta um protótipo de agente virtual universitário baseado em modelo de linguagem, desenvolvido para responder perguntas relacionadas às políticas e orientações presentes no *student handbook* de uma universidade.

O sistema permite que estudantes e outros membros da comunidade universitária realizem perguntas em linguagem natural sobre informações institucionais, utilizando o conteúdo do manual do estudante como base para apoiar a geração das respostas.

Consideramos esse sistema um concorrente direto por apresentar uma proposta bastante próxima do nosso TCC. Assim como no assistente que estamos desenvolvendo para a FEI, o usuário realiza uma pergunta em linguagem natural e recebe uma resposta baseada em conteúdo institucional. A principal diferença está no escopo documental: o protótipo de Ilagan e Ilagan concentra-se principalmente no *student handbook*, enquanto o nosso projeto pretende utilizar diferentes fontes institucionais da FEI para responder dúvidas acadêmicas e administrativas mais variadas.

#### Funcionalidades relevantes

| Funcionalidade | Como é realizada | Evidência/print | Observação de IHC |
|---|---|---|---|
| Perguntas em linguagem natural | O usuário formula perguntas relacionadas às políticas e orientações da universidade por meio de uma interface de perguntas e respostas | Artigo de Ilagan e Ilagan (2024) | Esse padrão é semelhante ao que pretendemos utilizar no nosso assistente, permitindo que o estudante formule a dúvida com suas próprias palavras, sem precisar conhecer previamente a estrutura dos documentos |
| Respostas em formato conversacional | O sistema utiliza um modelo de linguagem para interpretar a pergunta e apresentar uma resposta textual | Artigo de Ilagan e Ilagan (2024) | O formato pergunta–resposta se aproxima do fluxo que estamos propondo para a FEI e pode tornar a consulta mais direta do que a busca manual em páginas ou documentos |
| Uso de documentos institucionais | O conteúdo do *student handbook* é utilizado como base de conhecimento para as consultas realizadas pelo usuário | Artigo de Ilagan e Ilagan (2024) | Esse ponto é bastante próximo do nosso TCC, pois também pretendemos fundamentar as respostas em informações institucionais, embora utilizando uma base documental mais ampla |
| Uso de LLM para geração das respostas | O sistema utiliza um modelo de linguagem para interpretar as perguntas e gerar respostas | Artigo de Ilagan e Ilagan (2024) | Assim como no nosso projeto, o uso de LLM permite maior flexibilidade na formulação das dúvidas, mas exige cuidados para evitar respostas incorretas ou sem fundamento |

#### Experiência do usuário e opiniões

O trabalho apresenta principalmente a construção e demonstração de um protótipo. Não foi identificada, no artigo de 2024, uma avaliação formal de usabilidade com métricas como satisfação, tempo de execução de tarefas ou facilidade de uso.

Mesmo assim, o protótipo mostra uma forma de substituir parte da busca manual em um documento institucional por uma consulta em linguagem natural. Esse aspecto é especialmente relevante para o nosso projeto, pois também pretendemos facilitar o acesso às informações da FEI sem exigir que o estudante saiba previamente em qual página, documento ou setor determinada informação está disponível.

Do ponto de vista de IHC, consideramos que o formato conversacional é uma referência interessante para o nosso assistente por tornar a consulta mais direta. Entretanto, como o artigo não apresenta uma avaliação detalhada com usuários, não podemos concluir que essa abordagem seja necessariamente mais fácil ou mais satisfatória para estudantes.

Essa limitação também reforça a importância de avaliarmos, nas próximas etapas da disciplina, como os estudantes da FEI realmente percebem e utilizam uma interface desse tipo.

#### Preço/modelo de negócio

O sistema é apresentado como um **protótipo acadêmico de pesquisa**.

Não foram encontradas informações indicando que o sistema tenha sido comercializado, oferecido por assinatura ou disponibilizado como produto comercial.

Para a nossa comparação, esse aspecto possui menor relevância, pois o principal interesse está nas características da interação e na forma como o sistema utiliza informações institucionais para responder às dúvidas dos usuários.

#### Padrões e tendências percebidos

Os principais padrões de interação observados são:

- interface baseada em perguntas e respostas;
- uso de linguagem natural como forma principal de interação;
- geração de respostas textuais;
- utilização de documentos institucionais como base para as respostas;
- preocupação com possíveis respostas incorretas geradas pelo modelo de linguagem.

Esses padrões possuem relação direta com o que estamos propondo para o assistente da FEI. Principalmente, o uso de linguagem natural e de uma base institucional reforça a ideia de que o estudante possa realizar uma consulta sem precisar navegar previamente pela estrutura dos documentos.

Ao mesmo tempo, não foi possível confirmar no artigo a existência de funcionalidades como histórico de conversas, apresentação detalhada das fontes ao usuário, avaliação das respostas ou mensagens específicas para perguntas sem informação disponível.

Esses pontos são relevantes para o nosso projeto porque podem representar oportunidades de melhoria na experiência de interação, principalmente na apresentação das fontes e no tratamento de situações em que o sistema não encontre evidências suficientes para responder.

#### Pontos positivos, limitações e lições

| Ponto | Evidência | Implicação para nosso projeto |
|---|---|---|
| Permite realizar perguntas em linguagem natural | Artigo de Ilagan e Ilagan (2024) | Reforça a nossa decisão de utilizar linguagem natural como principal forma de interação com o assistente da FEI |
| Utiliza conteúdo institucional como base para as respostas | O sistema utiliza o *student handbook* | É bastante próximo da proposta do nosso TCC e reforça a importância de fundamentarmos as respostas em fontes institucionais da FEI |
| Utiliza uma interface simples de perguntas e respostas | Descrição do protótipo no artigo | Podemos manter um fluxo de consulta simples, evitando etapas desnecessárias antes de o estudante formular sua dúvida |
| O sistema está limitado principalmente ao conteúdo do *student handbook* | Descrição da base utilizada pelo protótipo | Nosso projeto pode ampliar esse escopo utilizando diferentes fontes institucionais da FEI, cobrindo uma variedade maior de dúvidas acadêmicas e administrativas |
| O artigo reconhece o risco de respostas incorretas produzidas por modelos de linguagem | Discussão sobre alucinações no artigo | Esse ponto reforça a necessidade de tratarmos explicitamente situações em que não exista informação suficiente para responder e de mantermos as respostas fundamentadas nas fontes recuperadas |
| Não há uma avaliação de usabilidade detalhada no artigo de 2024 | Avaliação apresentada no estudo | Podemos aprofundar esse aspecto no nosso projeto por meio das avaliações de IHC com estudantes da FEI previstas nas próximas entregas |
## 3. Softwares que o público-alvo usa no cotidiano

Analise interfaces que moldam a expectativa do público, mesmo que não sejam concorrentes.

| Software | Por que o público usa | Padrões relevantes | Prints | O que aprender |
|---|---|---|---|---|
| {{...}} | {{...}} | {{...}} | {{link local}} | {{...}} |

## 3.1 Padrões de interface relevantes ao escopo de IHC

Registre somente padrões encontrados nas soluções analisadas e que possam ter relação com objetivos reais da equipe.

| Padrão observado | Produto(s) | Para qual tarefa serve | Vantagem percebida | Risco/limitação | Aplicável ao nosso escopo? |
|---|---|---|---|---|---|
| dashboard | {{...}} | {{...}} | {{...}} | {{...}} | sim/não/talvez |
| relatório | {{...}} | {{...}} | {{...}} | {{...}} | {{...}} |
| histórico + filtros | {{...}} | {{...}} | {{...}} | {{...}} | {{...}} |
| administração/CRUD | {{...}} | {{...}} | {{...}} | {{...}} | {{...}} |
| comparação de resultados | {{...}} | {{...}} | {{...}} | {{...}} | {{...}} |

> O objetivo não é concluir “todo concorrente tem dashboard, então teremos um”. O padrão só será adotado se apoiar uma tarefa rastreável.

## 4. Síntese comparativa da equipe

| Critério | C01 | C02 | C03 | Oportunidade para o projeto |
|---|---|---|---|---|
| Navegação |  |  |  |  |
| Feedback/estado |  |  |  |  |
| Prevenção/recuperação de erro |  |  |  |  |
| Terminologia |  |  |  |  |
| Acessibilidade |  |  |  |  |
| Eficiência |  |  |  |  |

## 5. Recomendações derivadas

Liste recomendações com origem explícita.

- **RC01:** {{recomendação}} — derivada de {{C01/C02/evidência}}.
- **RC02:** {{...}}

## Referências

{{fontes dos produtos, avaliações e literatura}}

## Checklist

- [ ] O mapa inicial de alternativas da Entrega 1 foi revisitado e aprofundado.
- [ ] Hipóteses relevantes sobre mercado/padrões foram atualizadas na rastreabilidade quando surgiram evidências.
- [ ] Há pelo menos uma análise completa por integrante.
- [ ] Cada análise contém prints legíveis da interface.
- [ ] Prints mostram telas/estados relevantes, não apenas logos/homepage.
- [ ] Foram analisados concorrentes e/ou interfaces representativas ao público.
- [ ] Em TCC sem interface original, foram investigadas ferramentas profissionais análogas às atividades do usuário escolhido.
- [ ] Padrões como dashboard, relatório, filtros e CRUD foram analisados como soluções para tarefas, não como requisitos automáticos.
- [ ] Opiniões de UX têm fonte.
- [ ] A síntese compara critérios comuns e produz recomendações.
- [ ] Não há “copiar porque o concorrente faz”; há justificativa de adequação ao público/contexto.
