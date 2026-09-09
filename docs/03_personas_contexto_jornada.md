# Entrega 3 — Personas, mapa de empatia, contexto de uso e jornada

**Data:** {{dd/mm/aaaa}}  
**Status:** 🟨 em andamento
**Responsabilidade:** 1 persona por integrante; 1 mapa de empatia, 1 contexto de uso consolidado e 1 jornada por equipe (salvo orientação diferente do docente).

## Objetivo da atividade

Representar grupos de usuários de forma útil para decisões de design. Persona não é personagem decorativo: suas características devem alterar requisitos, prioridades, linguagem, fluxos ou critérios de avaliação.

## Atenção a projetos técnicos

Em TCCs sem interface original, a persona pode representar um **profissional que se apropria da contribuição técnica**: DBA, analista, cientista de dados, administrador, pesquisador, técnico, operador, gestor ou especialista de domínio.

Não escolha um perfil apenas porque “parece combinar” com a tecnologia. Explique **qual objetivo esse perfil teria e qual parte da contribuição do TCC produziria valor para ele**. Se ainda for hipótese, mantenha como hipótese/proto-persona a validar.

Também considere papéis diferentes quando houver tarefas distintas, por exemplo:

- operador que executa análises;
- administrador que configura e gerencia permissões;
- especialista que interpreta resultados;
- gestor que consulta relatórios e decide;
- auditor que revisa histórico.

## Entradas da Entrega 1

Antes de criar personas, retome os tipos de usuários, características relevantes, objetivos e hipóteses registradas na Entrega 1. A persona **não deve transformar uma hipótese inicial em fato por meio de uma história fictícia**.

| Item da Entrega 1 | Status inicial | Evidência disponível agora | Como será tratado nesta entrega |
|---|---|---|---|
| Estudante da FEI como usuário direto prioritário | F | O TCC e a Entrega 1 definem o estudante da FEI como principal usuário da interface de consulta acadêmico-administrativa | Incorporar como base das personas primárias |
| A01 — Localizar e compreender uma informação acadêmica ou administrativa | F | Atividade priorizada na Entrega 1 a partir do escopo definido para a interface do TCC | Incorporar como objetivo de uma das personas |
| A02 — Entender como realizar um procedimento acadêmico ou administrativo e quais etapas, regras ou prazos devem ser observados | F | Atividade priorizada na Entrega 1 a partir do escopo definido para a interface do TCC | Incorporar como objetivo de uma das personas |
| Estudantes podem enfrentar dificuldade ou esforço excessivo para localizar informações distribuídas entre páginas, documentos e canais institucionais | H | A situação é apresentada como motivação do TCC, mas ainda não foi validada diretamente com estudantes da FEI | Manter como hipótese e utilizar apenas como ponto a investigar nas personas |
| Estudantes podem possuir diferentes níveis de familiaridade com regras, procedimentos e terminologia institucional | H | Ainda não foi realizado levantamento direto com estudantes sobre conhecimento do domínio | Manter como hipótese e considerar diferenças de familiaridade entre as personas |
| Algumas consultas relacionadas a regras, prazos e procedimentos podem possuir maior criticidade ou urgência | H | A Entrega 1 identificou essa possibilidade, mas ainda não há dados sobre frequência ou gravidade percebida pelos estudantes | Manter como hipótese e considerar principalmente na persona associada à A02 |
| O histórico de conversas pode ajudar o estudante a retomar consultas anteriores | H | O recurso foi observado em ChatGPT e Gemini na Entrega 2, mas sua necessidade para estudantes da FEI ainda não foi validada | Não tratar como necessidade da persona; manter como possibilidade de design |
| Dispositivo predominante utilizado para realizar consultas acadêmicas e administrativas | ? | Ainda não há levantamento sobre preferência entre computador, notebook ou celular | Manter em aberto e evitar definir um dispositivo principal como característica da persona |
| Necessidades específicas de acessibilidade do público-alvo | ? | Ainda não foi realizado levantamento com usuários sobre necessidades de acessibilidade | Manter em aberto e não inventar restrições individuais para as personas |

### Persona P01 — Lucas Almeida

**Autor(a):** Matheus Dourado Valle — 22.224.023-6  
**Tipo:** primária  
**Base de evidências:** proto-persona a validar, construída a partir do escopo do TCC, da Entrega 1 e dos padrões observados na análise de concorrência  
**Hipóteses da Entrega 1 relacionadas:** H01

![Persona P01](../assets/03_personas/persona_p01.svg)

| Campo | Descrição |
|---|---|
| Faixa etária / contexto relevante | Estudante de graduação da FEI. A idade específica não é considerada relevante para as decisões de design neste momento. |
| Ocupação/papel | Estudante da FEI e usuário direto do assistente para consulta de informações acadêmicas e administrativas. |
| Conhecimento do domínio | [H] Possui conhecimento parcial sobre regras, serviços e procedimentos institucionais, mas pode não conhecer a terminologia exata ou onde determinada informação está disponível. |
| Experiência tecnológica | [H] Está familiarizado com interfaces digitais utilizadas no contexto acadêmico, como Portal do Aluno e Moodle, e pode ter contato com interfaces conversacionais de IA. |
| Objetivos | Localizar e compreender rapidamente uma informação acadêmica ou administrativa necessária para esclarecer uma dúvida ou tomar uma decisão. |
| Necessidades | Formular a dúvida com suas próprias palavras; receber uma resposta clara; identificar a fonte institucional relacionada à informação; conseguir complementar a pergunta quando necessário. |
| Dores/frustrações | [H] Pode ter dificuldade ou gastar esforço excessivo quando precisa descobrir em qual página, documento ou canal institucional determinada informação está disponível. |
| Motivadores | Obter uma orientação compreensível e fundamentada em informação institucional sem precisar conhecer previamente a estrutura das fontes disponíveis. |
| Restrições/acessibilidade | [?] Ainda não foram identificadas necessidades específicas de acessibilidade ou restrições de uso para esse perfil. Essas características deverão ser investigadas com usuários reais. |
| Ambiente típico de uso | A consulta pode ocorrer dentro ou fora do campus e por diferentes dispositivos. |
| Comportamentos relevantes | [H] Pode iniciar a busca formulando diretamente sua dúvida e realizar perguntas complementares quando a primeira resposta não for suficiente. |

**Decisões de design influenciadas por P01:**

- Manter a formulação da dúvida em linguagem natural como ação principal da interface.
- Evitar exigir que o estudante conheça previamente categorias, páginas ou documentos antes de realizar uma consulta.
- Apresentar respostas em linguagem clara e próxima ao contexto acadêmico do estudante.
- Apresentar a fonte institucional relacionada à resposta de forma visível e compreensível.
- Permitir que o estudante complemente ou reformule uma dúvida durante a interação.
- Informar claramente quando não houver evidência institucional suficiente para responder.
- Não tratar histórico de conversas, dispositivo predominante ou necessidades específicas de acessibilidade como requisitos confirmados antes de investigação com usuários.

### Persona P02 — Mariana Costa

**Autor(a):** João Pedro Sabino Garcia — 22.224.032-7  
**Tipo:** primária  
**Base de evidências:** proto-persona a validar, construída a partir do escopo do TCC, da Entrega 1 e dos padrões observados na análise de concorrência  
**Hipóteses da Entrega 1 relacionadas:** hipóteses relacionadas à necessidade de compreender procedimentos, regras, etapas e prazos acadêmico-administrativos

![Persona P02](../assets/03_personas/persona_p01.svg)

| Campo | Descrição |
|---|---|
| Faixa etária / contexto relevante | Estudante de graduação da FEI que precisa compreender como realizar um procedimento acadêmico ou administrativo. A idade específica não é considerada relevante para as decisões de design neste momento. |
| Ocupação/papel | Estudante da FEI e usuário direto do assistente para obter orientação sobre procedimentos acadêmicos e administrativos. |
| Conhecimento do domínio | [H] Conhece parte da rotina acadêmica, mas pode não dominar todas as regras, etapas, documentos necessários, prazos ou termos associados a procedimentos menos frequentes. |
| Experiência tecnológica | [H] Está familiarizada com sistemas digitais utilizados no contexto acadêmico, como Portal do Aluno e Moodle, e pode possuir experiência com interfaces conversacionais. O nível dessa familiaridade ainda precisa ser validado. |
| Objetivos | Entender corretamente como realizar um procedimento acadêmico ou administrativo, identificando etapas, regras, prazos e orientações relevantes para sua situação. |
| Necessidades | Receber uma orientação organizada e compreensível; identificar etapas do procedimento; compreender requisitos e prazos quando estiverem disponíveis; acessar a fonte institucional relacionada; poder esclarecer dúvidas complementares. |
| Dores/frustrações | [H] Pode ter dificuldade para reunir e interpretar informações necessárias quando um procedimento envolve diferentes páginas, documentos, regras ou orientações institucionais. |
| Motivadores | Realizar corretamente um procedimento e reduzir a incerteza sobre quais ações devem ser tomadas, quais regras se aplicam e onde consultar a informação oficial. |
| Restrições/acessibilidade | [?] Ainda não foram identificadas necessidades específicas de acessibilidade ou outras restrições para esse perfil. Essas características deverão ser investigadas com usuários reais. |
| Ambiente típico de uso | [?] A consulta pode ocorrer dentro ou fora do campus e por diferentes dispositivos. Ainda não existem evidências suficientes para determinar ambiente, horário ou equipamento predominante. |
| Comportamentos relevantes | [H] Pode formular inicialmente uma dúvida ampla sobre um procedimento e, após receber uma primeira orientação, realizar perguntas complementares sobre etapas, requisitos ou prazos específicos. Esse comportamento ainda precisa ser validado com estudantes reais. |

**Decisões de design influenciadas por P02:**

- Permitir que o estudante formule dúvidas sobre procedimentos utilizando linguagem natural.
- Organizar respostas sobre procedimentos de forma clara, destacando etapas, requisitos ou prazos quando essas informações estiverem presentes nas fontes institucionais.
- Evitar apresentar como obrigatória qualquer etapa que não esteja sustentada pelas fontes recuperadas.
- Apresentar de forma visível a fonte institucional utilizada para fundamentar a orientação.
- Permitir perguntas complementares dentro da mesma interação para esclarecer partes específicas do procedimento.
- Informar explicitamente quando determinada etapa, regra ou prazo não puder ser confirmado pela base documental.
- Evitar linguagem excessivamente técnica e explicar termos institucionais quando necessário.
- Não assumir como confirmados o dispositivo predominante, a frequência das consultas ou necessidades específicas de acessibilidade sem validação com usuários.

> Repita para P02, P03... Cada integrante deve produzir ao menos uma persona.

### Síntese das personas

Explique diferenças entre os perfis e qual persona é prioritária. Evite personas duplicadas que só mudam nome/foto.

## 2. Mapa de empatia — equipe

**Persona escolhida:** {{P01}}  
**Justificativa:** {{por que esse perfil é relevante}}

![Mapa de empatia](../assets/03_personas/mapa_empatia.svg)

Documente também em texto: o que vê; ouve; diz/faz; pensa/sente; dores; ganhos. Diferencie **evidência** de **hipótese**.

## 3. Contexto de uso — consolidação

| Dimensão | Descrição | Implicação de design |
|---|---|---|
| Usuários | {{...}} | {{...}} |
| Tarefas | {{...}} | {{...}} |
| Equipamentos | {{...}} | {{...}} |
| Ambiente físico | {{...}} | {{...}} |
| Ambiente social/organizacional | {{...}} | {{...}} |
| Papéis/permissões/governança | {{...}} | {{...}} |
| Volume de dados/histórico | {{...}} | {{...}} |

## 4. Jornada do usuário — equipe

**Persona:** {{P01}}  
**Objetivo da jornada:** {{...}}  
**Início e fim da jornada:** {{...}}

| Etapa | Situação/ação | Objetivo | Pensamento/emoção | Dor | Oportunidade de design | Evidência |
|---|---|---|---|---|---|---|
| 1 | {{...}} | {{...}} | {{...}} | {{...}} | {{...}} | {{...}} |

> A jornada pode incluir etapas **antes, durante e depois** do uso do produto. Não transforme a jornada em lista de telas.

## Síntese

Quais necessidades e objetivos devem obrigatoriamente aparecer nos cenários e nas tarefas seguintes?

## Checklist

- [ ] Existe pelo menos uma persona por integrante.
- [ ] As personas não são apenas diferenças demográficas superficiais.
- [ ] Está claro o que é dado real e o que é hipótese/proto-persona.
- [ ] A persona não “validou por ficção” uma hipótese da Entrega 1; afirmações continuam marcadas como hipótese quando não há evidência.
- [ ] Objetivos e dores têm consequência para o design.
- [ ] Contexto de uso está coerente com a Entrega 1.
- [ ] Em TCC sem interface original, a persona possui relação explícita com a contribuição técnica.
- [ ] Papéis administrativos, técnicos e decisórios só foram criados quando possuem objetivos/tarefas diferentes.
- [ ] Jornada possui etapas, dores e oportunidades e não é apenas wireflow.
- [ ] IDs das personas foram adicionados à rastreabilidade.
