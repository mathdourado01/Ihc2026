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
| Formulação de perguntas em linguagem natural            | O usuário digita sua solicitação em um campo de texto e envia a mensagem para iniciar ou continuar a conversa                                      | `../assets/02_concorrencia/c01_chatgpt_pergunta.png`     | O campo de entrada concentra a principal ação da interface e permite que o usuário formule a dúvida com suas próprias palavras                    |
| Resposta em formato conversacional                      | A resposta é apresentada na sequência da pergunta, mantendo a estrutura de diálogo entre usuário e assistente                                      | `../assets/02_concorrencia/c01_chatgpt_resposta.png`     | A associação visual entre pergunta e resposta facilita o acompanhamento da interação e permite perguntas complementares                           |
| Continuidade da conversa                                | O usuário pode realizar novas perguntas no mesmo diálogo, utilizando o contexto das mensagens anteriores                                           | `../assets/02_concorrencia/c01_chatgpt_continuidade.png` | Reduz a necessidade de repetir todo o contexto e permite refinar uma pergunta quando a primeira resposta não é suficiente                         |
| Apresentação de fontes em respostas com pesquisa na web | Quando a pesquisa na web é utilizada, a resposta pode apresentar citações associadas às informações utilizadas e uma área para consulta das fontes | `../assets/02_concorrencia/c01_chatgpt_fontes.png`       | A presença de fontes fornece um caminho para que o usuário consulte a origem de determinada informação, padrão especialmente relevante para o TCC |
| Histórico de conversas                                  | Conversas anteriores podem ser retomadas posteriormente por meio da navegação da interface                                                         | `../assets/02_concorrencia/c01_chatgpt_historico.png`    | Pode facilitar a retomada de uma consulta anterior, embora a necessidade desse recurso para os estudantes da FEI ainda precise ser investigada    |

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


## 2. Concorrentes diretos/indiretos

### Análise C01 — {{produto}}

**Autor(a):** {{nome — matrícula}}  
**Tipo:** direto / indireto / análogo  
**Link oficial:** {{URL}}  
**Data de acesso:** {{dd/mm/aaaa}}

#### Contexto e proposta

{{...}}

#### Funcionalidades relevantes

| Funcionalidade | Como é realizada | Evidência/print | Observação de IHC |
|---|---|---|---|
| {{...}} | {{...}} | `../assets/02_concorrencia/...` | {{...}} |

#### Experiência do usuário e opiniões

Use avaliações públicas, relatos, estudos, testes próprios ou outra fonte identificável. Não trate opinião isolada como verdade universal.

#### Preço/modelo de negócio

{{...}}

#### Padrões e tendências percebidos

{{...}}

#### Pontos positivos, limitações e lições

| Ponto | Evidência | Implicação para nosso projeto |
|---|---|---|
| {{...}} | {{...}} | {{...}} |

> Repita a subseção para C02, C03... até atender à quantidade da equipe.

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
