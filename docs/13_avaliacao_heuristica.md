# Entrega 13 — Avaliação de IHC por inspeção heurística

**Data:** {{14/11/2026}}  
**Status:** 🟨 em andamento  
**Responsabilidade:** 1 avaliação completa por integrante, sobre todas as telas/estados relevantes do projeto.

## Objetivo da atividade

Encontrar problemas de usabilidade por inspeção sistemática da interface com as **10 heurísticas de Nielsen**. Cada avaliador trabalha individualmente primeiro; depois a equipe consolida problemas duplicados e prioridades.

> **Parte de violações:** registre somente problemas reais. Não invente uma violação para “preencher” cada heurística. Para provar que todas foram exercitadas, use a **matriz de cobertura H1–H10**. Para heurísticas sem violação, a disciplina solicita um exemplo didático de boa prática.

## 1. Heurísticas adotadas

1. Visibilidade do status do sistema
2. Compatibilidade entre o sistema e o mundo real
3. Controle e liberdade do usuário
4. Consistência e padrões
5. Prevenção de erros
6. Reconhecimento em vez de memorização
7. Flexibilidade e eficiência de uso
8. Estética e design minimalista
9. Ajudar usuários a reconhecer, diagnosticar e recuperar-se de erros
10. Ajuda e documentação

## Cobertura especial para interfaces administrativas e analíticas

Quando existirem, não limite a avaliação às “telas principais”. Inspecione também:

- dashboard em estados normal, vazio e erro;
- filtros sem resultado e filtros combinados;
- relatórios e exportação;
- histórico/listas longas;
- formulários CRUD (criação, edição, exclusão, validação);
- alteração de perfil/permissão;
- confirmações de ações destrutivas;
- processamento/loading/progresso;
- falha e recuperação;
- comparação de resultados;
- mensagens de termos técnicos, métricas e recomendações;
- ajuda/documentação contextual.

Em TCCs técnicos, observe especialmente se a interface comunica o estado do processamento e traduz informações técnicas para o vocabulário do usuário escolhido.


## 2. Escopo da inspeção

| Item | Definição |
|---|---|
| Versão avaliada | Protótipo no Figma — Assistente Virtual Acadêmico da FEI, em 14/11/2026. |
| Link | https://www.figma.com/design/H0YnqyGWkswU88IUZIgDuW |
| Telas/estados | F01–F16, contemplando início, carregamento, respostas acadêmicas, ausência de evidências, histórico, categorias, falhas, esclarecimentos, contexto insuficiente, encerramento e consulta de fontes. |
| Fluxos | M01 — Matheus e M02 — João. |
| Dispositivo/viewport | Desktop — interface web, com dimensões de 1280 × 768 pixels no Figma. |
| Avaliador | Matheus Dourado Valle (A01). |

## 3. Procedimento individual

Cada avaliador deve:

1. percorrer os fluxos/telas ao menos uma vez para familiarização;
2. inspecionar novamente aplicando sistematicamente H1–H10;
3. registrar cada problema com evidência e contexto;
4. atribuir severidade **depois de compreender bem o problema**, justificando a decisão;
5. não discutir achados com os demais antes de terminar a inspeção individual, quando o objetivo for preservar independência.

A inspeção do avaliador A01 considerou os principais fluxos e estados do protótipo, observando a facilidade de utilização, clareza das informações, apresentação das fontes, navegação, feedback e recuperação de erros.

A avaliação considera exclusivamente a qualidade da interação e da interface do protótipo, não o desempenho técnico ou a precisão científica dos modelos de inteligência artificial.

### Escala de severidade (0–4)

| Grau | Interpretação |
|---:|---|
| 0 | não é considerado problema de usabilidade |
| 1 | problema cosmético; corrigir se houver tempo |
| 2 | problema menor; baixa prioridade |
| 3 | problema maior; alta prioridade |
| 4 | catástrofe de usabilidade; correção imperativa antes de disponibilizar |

Ao justificar, considere **frequência, impacto e persistência** do problema no contexto real de uso.

---

## Avaliador A01 — Matheus Dourado Valle

### 4. Matriz de cobertura das 10 heurísticas

| Heurística | Telas/fluxos examinados | Houve violação? | IDs dos achados | Exemplo de boa prática se não violada |
|---|---|---|---|---|
| H1 — Visibilidade do status do sistema | F02 e F11 | não | — | As mensagens de carregamento informam que o assistente está consultando fontes institucionais e processando a pergunta. |
| H2 — Compatibilidade entre sistema e mundo real | F02 e F11 | sim | V01 | — |
| H3 — Controle e liberdade do usuário | F04 e F08 | não | — | O usuário possui opções para reformular perguntas, cancelar consultas e tentar novamente. |
| H4 — Consistência e padrões | F01–F16 | não | — | O menu lateral, cabeçalho e estrutura de conversação mantêm uma organização consistente entre as telas. |
| H5 — Prevenção de erros | F01 e F04 | não | — | As sugestões de perguntas e alternativas de consulta ajudam o estudante a formular dúvidas e encontrar caminhos adequados. |
| H6 — Reconhecimento em vez de memorização | F03, F07, F15 e F16 | sim | V02 | — |
| H7 — Flexibilidade e eficiência de uso | F01 e F04 | não | — | O usuário pode iniciar uma consulta por sugestões ou formular sua própria pergunta, além de acessar diferentes alternativas de interação. |
| H8 — Estética e design minimalista | F01 e F04 | não* | — | As telas apresentam mensagens principais e ações relacionadas ao contexto, mantendo o foco na interação. |
| H9 — Ajudar usuários a reconhecer, diagnosticar e recuperar-se de erros | F04 e F08 | não | — | Quando ocorre uma falha ou ausência de evidências, são apresentadas alternativas para continuar a interação. |
| H10 — Ajuda e documentação | F01 | não | — | A tela inicial apresenta orientações para começar a utilizar o assistente e exemplos de dúvidas que podem ser consultadas. |

*Na H8, não foi identificada uma violação na organização do conteúdo observado. Contraste e legibilidade visual não foram avaliados em profundidade.*

### 5. Declaração de violações

| ID | Heurística | Tela/estado | Problema observado | Evidência | Severidade | Justificativa da severidade | Recomendação |
|---|---|---|---|---|---:|---|---|
| V01 | H2 | F02 e F11 | Durante o processamento, são apresentadas opções como "Ver resposta simulada", "Sem evidências" e "Simular falha", que representam controles de demonstração do protótipo e não ações naturais de um estudante utilizando o assistente. | [F02](../assets/11_figma/f02.png) e [F11](../assets/11_figma/f11.png). | 2 | Pode gerar dúvidas sobre a finalidade dos controles e prejudicar a naturalidade da interação, embora não impeça necessariamente a continuidade do fluxo. | Restringir os controles de simulação ao ambiente de avaliação ou substituí-los por ações adequadas ao estudante. |
| V02 | H6 | F03, F07, F15 e F16 | As fontes são apresentadas com identificações genéricas, como "Secretaria / Serviços ao aluno" e "Edital de ingresso / Pós-graduação", sem identificação de documentos específicos ou links oficiais para consulta. | [F03](../assets/11_figma/f03.png), [F07](../assets/11_figma/f07.png), [F15](../assets/11_figma/f15.png) e [F16](../assets/11_figma/f16.png). | 3 | Dificulta a identificação e a verificação das informações utilizadas pelo assistente. Como a consulta às fontes é uma funcionalidade central do projeto, o problema pode comprometer a confiança do estudante nas respostas. | Apresentar o título completo do documento, setor responsável, data ou versão e link direto para a fonte institucional. |

**Qualidade do relato:** os problemas foram identificados em telas e elementos específicos do protótipo, considerando suas consequências para a experiência do estudante.

**Evidências do problema V01**

![F02 - Carregamento de Lucas](../assets/11_figma/f02.png)

![F11 - Carregamento de Mariana](../assets/11_figma/f11.png)

**Evidências do problema V02**

![F03 - Resposta acadêmica](../assets/11_figma/f03.png)

![F07 - Resposta sobre ingresso no mestrado](../assets/11_figma/f07.png)

![F15 - Verificação da fonte acadêmica](../assets/11_figma/f15.png)

![F16 - Verificação da fonte do mestrado](../assets/11_figma/f16.png)

### 6. Boas práticas — heurísticas não violadas (atividade didática)

| Heurística sem violação | Exemplo no sistema | Evidência | Por que atende |
|---|---|---|---|
| H1 — Visibilidade do status do sistema | F02 e F11 — mensagens de carregamento. | [F02](../assets/11_figma/f02.png) e [F11](../assets/11_figma/f11.png). | O sistema informa que está consultando fontes institucionais e orienta o usuário a aguardar o processamento. |
| H3 — Controle e liberdade do usuário | F04 e F08 — alternativas para reformular perguntas, tentar novamente ou encerrar a consulta. | [F04](../assets/11_figma/f04.png) e [F08](../assets/11_figma/f08.png). | O usuário possui alternativas para modificar o caminho da interação quando necessário. |
| H4 — Consistência e padrões | F01, F02, F03, F04, F07, F08, F11, F15 e F16 — estrutura de navegação e cabeçalho. | [F01](../assets/11_figma/f01.png) e [F03](../assets/11_figma/f03.png). | Os elementos principais de navegação e interação mantêm uma organização semelhante entre as diferentes telas. |
| H5 — Prevenção de erros | F01 — sugestões de perguntas e opções iniciais de consulta. | [F01](../assets/11_figma/f01.png). | As sugestões ajudam o estudante a formular dúvidas e identificar possibilidades de consulta. |
| H7 — Flexibilidade e eficiência de uso | F01 — sugestões iniciais e campo para digitação de perguntas próprias. | [F01](../assets/11_figma/f01.png). | O usuário pode escolher entre utilizar uma sugestão ou formular sua própria pergunta, oferecendo diferentes maneiras de iniciar uma consulta. |
| H8 — Estética e design minimalista | F04 — apresentação da ausência de evidências. | [F04](../assets/11_figma/f04.png). | A tela concentra a informação na mensagem principal e nas alternativas de continuidade, sem apresentar informações funcionais desnecessárias. |
| H9 — Recuperação de erros | F08 — opções para tentar novamente, reformular a pergunta ou encerrar a consulta. | [F08](../assets/11_figma/f08.png). | O usuário recebe orientações e alternativas para recuperar a interação após uma falha de processamento. |
| H10 — Ajuda e documentação | F01 — orientações iniciais e exemplos de perguntas. | [F01](../assets/11_figma/f01.png). | A tela inicial orienta o usuário sobre como começar a utilizar o assistente e apresenta exemplos que facilitam a compreensão de suas possibilidades. |


## 7. Consolidação da equipe

Problemas iguais ou muito semelhantes encontrados por avaliadores diferentes devem ser consolidados, preservando quem os encontrou.

| ID consolidado | Achados individuais | Heurística | Problema | Severidade final | Prioridade | Responsável pela correção |
|---|---|---|---|---:|---|---|
| HC01 | V01(A01), V04(A02) | H1 | {{...}} | {{...}} | alta | {{...}} |

## 8. Síntese e plano de melhoria

- Quantidade de problemas por heurística e severidade.
- Problemas críticos/graves que bloqueiam teste ou release.
- Padrões recorrentes entre telas.
- Correções que serão feitas antes/para a avaliação com usuários.

## Checklist

- [ ] Cada integrante fez uma inspeção completa e identificada.
- [ ] Todas as telas/estados relevantes foram examinados.
- [ ] Estados administrativos, filtros, relatórios, históricos, processamento e erros foram incluídos quando existentes.
- [ ] A inspeção avaliou a interface/protótipo, não o mérito técnico do algoritmo/modelo.
- [ ] H1–H10 aparecem na matriz de cobertura de cada avaliador.
- [ ] Parte de violações contém apenas violações, sem “forçar” exemplos.
- [ ] Todo problema tem print/localização e contexto.
- [ ] Severidade possui justificativa, não apenas número.
- [ ] Recomendação resolve a causa ou reduz o impacto.
- [ ] Achados duplicados foram consolidados ao final.
