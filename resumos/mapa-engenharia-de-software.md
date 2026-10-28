---
tipo: resumo
disciplina: ["Engenharia de Software e Ágil"]
assunto: "Mapa geral de Engenharia de Software"
data: 2026-10-24
atualizado: 2026-10-26
---

# Mapa geral · Engenharia de Software

**Criado em:** 24/10/2026 · **Versão 2:** 26/10/2026 (cada assunto com: pra que serve · onde é usado · por que é assim · conceitos técnicos)
**Base:** Sommerville (*Engenharia de Software*, material da UNIVESP), Pressman, Guia do Scrum 2020 e Manifesto Ágil, as fontes mais usadas pela FGV.

> **Como ler cada ficha:**
> 🎯 **Pra que serve** (o problema que resolve) · 🏛️ **Onde é usado** (tipo de projeto, com exemplo do Judiciário) · 🤔 **Por que é assim** (a decisão por trás) · 🔧 **Conceitos técnicos** (o que cai na prova) · 📌 **Regra/pegadinha FGV**
>
> Os exemplos do Judiciário (PJe, consulta processual, peticionamento) são **ilustrativos**, para fixar a ideia. Não descrevem como cada tribunal desenvolve de fato.

---

## 0. Por que a Engenharia de Software existe

| | |
|---|---|
| 🎯 **Pra que serve** | Produzir software **confiável, no prazo e no custo**, de forma repetível, e não por "talento individual" |
| 🤔 **Por que surgiu** | Na **"crise do software"** dos anos 1960, os projetos atrasavam, estouravam o orçamento e entregavam sistemas cheios de defeitos. O termo *engenharia de software* foi popularizado na **conferência da OTAN de 1968** (Garmisch, Alemanha): a proposta era tratar o software com a disciplina de uma engenharia |
| 🔧 **Conceito-chave** | Software não é só código: inclui **documentação, dados de configuração e programas** que fazem o sistema funcionar (Sommerville) |

**Atributos de um bom software (Sommerville):**

| Atributo | Significado | Exemplo (PJe) |
|---|---|---|
| **Manutenibilidade** | Fácil de evoluir quando as regras mudam | Nova lei altera prazo processual → mudar sem quebrar o resto |
| **Confiança e proteção** | Não falha, não causa dano e resiste a ataques | Processo sigiloso não pode vazar |
| **Eficiência** | Não desperdiça recursos (tempo de resposta, memória) | Consulta processual rápida no pico do dia |
| **Aceitabilidade** | Compreensível, usável e compatível para quem usa | Advogado consegue peticionar sem treinamento longo |

📌 **Ideia-mãe da disciplina:** quanto mais tarde um erro é descoberto, **mais caro** é corrigir. Os modelos de processo são **respostas diferentes** a esse problema: os tradicionais tentam **evitar a mudança** (planejar tudo antes); os ágeis tentam **baratear a mudança** (ciclos curtos e feedback rápido).

---

## Mapa em uma linha

**Atividades fundamentais** → organizadas de forma **sequencial, iterativa ou incremental** → aplicadas por um **modelo** (tradicional: cascata, V, espiral, RUP · ágil: Scrum, XP, Kanban) → apoiadas por **áreas transversais** (requisitos, estimativa, testes, arquitetura, DevOps).

```
GRUPO 1 · Atividades fundamentais (O QUE todo processo faz)
      │
      ▼
GRUPO 2 · Formas de organizar ("adjetivos": sequencial, iterativo, incremental)
      │
      ▼
MODELOS ("substantivos")
 ├── GRUPO 3 · Tradicionais / dirigidos a planos: Cascata, V, Incremental, Prototipação, Espiral, RUP
 └── GRUPO 4 · Ágeis: Manifesto, Scrum, XP, Kanban, Lean, SAFe
      │
      ▼
GRUPO 5 · Áreas transversais (valem para qualquer modelo): requisitos, estimativa, testes, arquitetura, DevOps
```

**Comparação-chave:** iterativo e incremental funcionam como **adjetivos**; os modelos são os **substantivos**. Você diz "o RUP é iterativo e incremental" do mesmo jeito que diz "o Scrum é iterativo e incremental". Iterativo e incremental **não são** o RUP: são características que vários modelos têm.

---

## Grupo 1 · A base: o que todo processo faz

| | |
|---|---|
| 🎯 **Pra que serve** | Dar um "esqueleto comum" para comparar qualquer modelo |
| 🤔 **Por que é assim** | Qualquer software precisa ser **definido, construído, conferido e mantido**. Os modelos não eliminam essas etapas: só mudam **a ordem e quantas vezes** elas acontecem |

| Atividade (Sommerville) | Pergunta que responde | Produtos típicos |
|---|---|---|
| **1. Especificação** | O que o sistema deve fazer e com quais restrições? | Documento de requisitos, histórias de usuário |
| **2. Projeto e implementação** | Como ele será estruturado e codificado? | Arquitetura, modelos, código |
| **3. Validação** (V&V) | Ele faz o que o cliente precisa? | Testes, revisões, inspeções |
| **4. Evolução** | Como ele se adapta às mudanças? | Novas versões, manutenção |

🔧 **Verificação × Validação** (Boehm):
- **Verificação:** "estamos construindo o produto **corretamente**?" → confere contra a **especificação**.
- **Validação:** "estamos construindo o produto **certo**?" → confere contra a **necessidade real do cliente**.

📌 Evolução também é atividade do processo: a maior parte do custo do software está **depois** da entrega (manutenção).

---

## Grupo 2 · Os "adjetivos": formas de organizar as atividades

| Forma | Ideia | Imagem | 🤔 Por que existe |
|---|---|---|---|
| **Sequencial** | Faz cada atividade uma vez, em ordem | Prédio: projeto aprovado → obra → entrega | Controle e previsibilidade quando os requisitos são estáveis |
| **Incremental** | Entrega o sistema **em pedaços prontos**, um de cada vez | Primeiro a consulta processual, depois o peticionamento, depois as certidões | Usuário recebe valor cedo; o risco fica dividido em partes |
| **Iterativo** | **Refaz e melhora** o mesmo produto em ciclos | Rascunho → versão 2 → versão 3 do mesmo texto | Ninguém acerta tudo na primeira vez; o feedback corrige o rumo |
| **Evolucionário** | Iterativo + incremental juntos | O que quase todo método moderno faz | Junta as vantagens dos dois |

📌 Incremental **acrescenta**; iterativo **refina**.

---

## Grupo 3 · Modelos tradicionais (dirigidos a planos)

**Filosofia comum:** planejar e documentar **antes** de construir, medir o progresso **contra o plano** e controlar as mudanças formalmente.

**🤔 Por que essa filosofia faz sentido?** Na época (anos 1970–80), mudar software custava caro (sem testes automatizados, ferramentas, nem integração contínua). Se mudar é caro, a estratégia racional é **decidir tudo antes**. Até hoje ela faz sentido quando a mudança é **proibida ou perigosa** (sistema crítico, contrato fechado, regulação).

### 3.1 Cascata (Waterfall)

|                           |                                                                                                                                                                                                                  |
| ------------------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| 🎯 **Pra que serve**      | Organizar o projeto em fases fechadas, com aprovação formal entre elas                                                                                                                                           |
| 🏛️ **Onde é usado**      | Requisitos **estáveis e bem entendidos**, contratos de escopo fechado, sistemas embarcados ou críticos, integração com hardware. Ex.: adequar um sistema a um layout de arquivo já definido em norma             |
| 🤔 **Por que é assim**    | Copia as engenharias tradicionais (civil, mecânica): projeto aprovado antes de construir. Dá **visibilidade gerencial**, porque cada fase gera um documento que pode ser cobrado                                 |
| 🔧 **Conceitos técnicos** | Fases: requisitos → projeto → implementação → testes → operação e manutenção · cada fase **só começa após a aprovação** da anterior · documentação forte · cliente vê o software só no fim (**feedback tardio**) |
| ⚠️ **Problema**           | Requisitos mudam; descobrir um erro de requisito na fase de testes custa muito caro                                                                                                                              |

📌 Winston **Royce (1970)** descreveu o modelo sequencial **para criticá-lo**: ele mesmo recomendava iteração e feedback. O nome "cascata" veio depois.

### 3.2 Modelo em V

| | |
|---|---|
| 🎯 **Pra que serve** | Ligar **cada fase de especificação a um nível de teste** |
| 🏛️ **Onde é usado** | Sistemas críticos e regulados (defesa, saúde, automotivo, setor público com contrato formal) |
| 🤔 **Por que é assim** | Na cascata, o teste vira uma "fase do fim" improvisada. No V, os testes **são planejados junto** com a especificação correspondente |
| 🔧 **Conceitos técnicos** | Lado esquerdo desce (requisitos → arquitetura → projeto detalhado) · base = codificação · lado direito sobe (unitário → integração → sistema → aceitação) |

| Especificação (esquerda) | ↔ | Teste (direita) |
|---|---|---|
| Requisitos do usuário | ↔ | Teste de **aceitação** |
| Requisitos do sistema / arquitetura | ↔ | Teste de **sistema** |
| Projeto de módulos | ↔ | Teste de **integração** |
| Codificação | ↔ | Teste **unitário** |

📌 O V é **sequencial** (variação do cascata), não iterativo.

### 3.3 Incremental

| | |
|---|---|
| 🎯 **Pra que serve** | Entregar o sistema em **partes funcionais**, cada uma já usada pelo cliente |
| 🏛️ **Onde é usado** | Sistemas de negócio em que dá para priorizar funções. Ex.: entregar primeiro a consulta processual e depois o peticionamento |
| 🤔 **Por que é assim** | Reduz o **custo da mudança** (refaz-se menos), dá **feedback real** e entrega valor cedo |
| 🔧 **Conceitos técnicos** | 1º incremento = **núcleo** do produto (Pressman) · cada incremento passa por especificação, desenvolvimento e validação · prioridade pelo valor |
| ⚠️ **Problemas (Sommerville)** | Processo **pouco visível** (não compensa documentar cada versão) · a **estrutura degrada** sem refatoração · difícil em sistemas grandes, de vida longa e com várias equipes |

### 3.4 Prototipação

| | |
|---|---|
| 🎯 **Pra que serve** | **Validar requisitos** (e interface) quando o cliente não sabe dizer exatamente o que quer |
| 🏛️ **Onde é usado** | Telas novas, sistemas com muita interação com o usuário. Ex.: protótipo da tela de peticionamento para os advogados testarem |
| 🤔 **Por que é assim** | É mais fácil reagir a algo concreto ("não era isso") do que descrever no papel |
| 🔧 **Conceitos técnicos** | **Descartável** (*throwaway*): joga fora depois de entender o requisito · **Evolutivo**: o protótipo vira o sistema · ciclo: comunicação → plano rápido → modelagem → construção do protótipo → feedback |
| ⚠️ **Risco** | Cliente achar que o protótipo "já está pronto" · protótipo descartável **não deve** virar produto: ignora requisitos não funcionais e tem estrutura ruim |

### 3.5 Espiral (Boehm)

| | |
|---|---|
| 🎯 **Pra que serve** | Conduzir projetos **grandes e arriscados**, decidindo cada passo pela **análise de risco** |
| 🏛️ **Onde é usado** | Projetos caros, com tecnologia nova ou incerteza alta. Ex.: migrar o sistema processual inteiro para uma nova plataforma |
| 🤔 **Por que é assim** | O maior desperdício é descobrir tarde um risco fatal. A cada volta, o projeto pode **mudar de rumo ou ser cancelado** antes de gastar mais |
| 🔧 **Conceitos técnicos** | Cada **volta** = uma fase · 4 setores por volta: (1) definir objetivos, alternativas e restrições → (2) **avaliar e reduzir riscos** (protótipos) → (3) desenvolver e validar → (4) planejar a próxima volta · é um **metamodelo**: pode usar cascata, prototipação etc. dentro das voltas |

📌 Palavra-chave: **risco**. O espiral é **iterativo** e **evolucionário** (Pressman).

### 3.6 RUP (Rational Unified Process)

| | |
|---|---|
| 🎯 **Pra que serve** | Processo completo e configurável para **sistemas grandes orientados a objetos**, unindo UML, casos de uso e arquitetura |
| 🏛️ **Onde é usado** | Muito usado nos anos 2000 em grandes empresas e governo (muitos editais e documentos de órgãos públicos ainda trazem termos do RUP: caso de uso, documento de arquitetura) |
| 🤔 **Por que é assim** | Une o melhor dos dois mundos da época: a **disciplina** dos tradicionais (fases, marcos, documentos) com a **iteração** (reduzir risco cedo). Criado pela Rational, com os autores da UML (Jacobson, Booch e Rumbaugh); hoje é da IBM |
| 🔧 **Definição clássica** | **Dirigido a casos de uso, centrado na arquitetura, iterativo e incremental** |

**3 perspectivas (Sommerville):**

| Perspectiva | Mostra | Pergunta |
|---|---|---|
| **Dinâmica** | As **fases** ao longo do tempo | *Quando?* |
| **Estática** | As **atividades/disciplinas** (workflows) | *O quê?* |
| **Prática** | As **boas práticas** recomendadas | *Como fazer bem?* |

**4 fases (perspectiva dinâmica) e o que cada uma entrega:**

| Fase | Foco | Produto principal | Marco |
|---|---|---|---|
| **Concepção** | Vale a pena fazer? | **Caso de negócio**, escopo, atores principais | Objetivos do ciclo de vida |
| **Elaboração** | Entender o problema e definir a base técnica | **Arquitetura** + maioria dos **casos de uso** + plano; riscos principais tratados | Arquitetura do ciclo de vida |
| **Construção** | Construir | Software funcionando + documentação para o usuário | Capacidade operacional inicial |
| **Transição** | Levar ao usuário | Sistema implantado no ambiente real (beta, treinamento) | Release do produto |

**Disciplinas (perspectiva estática):** 6 de engenharia (modelagem de negócios, requisitos, análise e projeto, implementação, teste, implantação) + 3 de apoio (gerência de configuração e mudança, gerência de projeto, ambiente).
**Boas práticas (perspectiva prática):** desenvolver iterativamente · gerenciar requisitos · usar arquitetura baseada em componentes · modelar visualmente (UML) · verificar a qualidade · controlar as mudanças.

🔧 Ponto-chave: as fases **não são** as disciplinas. **Toda disciplina pode ocorrer em qualquer fase**, com intensidade diferente, e cada fase tem iterações.

📌 Elaboração = **arquitetura**. Concepção = **caso de negócio**.

#### O RUP é ágil? **Não.**

| | RUP | Ágil (Scrum, XP) |
|---|---|---|
| Iterativo e incremental | ✅ Sim | ✅ Sim |
| Planejamento | Detalhado, com fases e marcos formais | Leve, a cada ciclo |
| Documentação | Muita (modelos UML, casos de uso, documento de arquitetura) | Mínima ("software funcionando mais que documentação") |
| Papéis e processo | Muitos papéis, atividades e artefatos definidos | Poucos papéis, equipe auto-organizada |
| Época | Final dos anos 1990 | Manifesto de 2001 (reação a processos "pesados" como o RUP) |
| Classificação | Processo **pesado** e prescritivo | Processo **leve** |

- **Variações ágeis existem:** **AUP** (Agile Unified Process, Scott Ambler) e **OpenUP** são versões enxutas derivadas, não o RUP em si.

📌 **Pegadinha FGV:** "o RUP, por ser iterativo e incremental, é um método ágil" → **falso**. Iterativo e incremental é característica; ágil é filosofia (Manifesto).

### Quando escolher dirigido a planos (Sommerville)

Sistema **crítico** (precisa de análise formal antes) · **regulação externa** exige documentação · especificação precisa ser **aprovada antes** de codificar (contrato) · equipe **grande ou distribuída** · ciclo de vida muito longo.

---

## Grupo 4 · Métodos ágeis (o contraponto)

**🤔 Por que surgiram:** nos anos 1990, os processos pesados geravam muita documentação que **envelhecia** antes do software ficar pronto, e os requisitos de negócio mudavam mais rápido que o plano. Com ferramentas melhores (testes automatizados, integração contínua), **mudar ficou barato**. Então a estratégia virou: em vez de evitar a mudança, **abraçá-la com ciclos curtos**.

### 4.1 Manifesto Ágil (2001)

| | |
|---|---|
| 🎯 **Pra que serve** | Ser a "constituição" do ágil: **4 valores e 12 princípios** que qualquer método ágil segue |
| 🤔 **Origem** | 17 autores de métodos "leves" (Scrum, XP etc.) se reuniram em Snowbird (EUA), em 2001, para achar o que tinham em comum |

| Valorizamos mais... | ...que |
|---|---|
| **Indivíduos e interações** | processos e ferramentas |
| **Software em funcionamento** | documentação abrangente |
| **Colaboração com o cliente** | negociação de contratos |
| **Responder a mudanças** | seguir um plano |

Princípios que mais caem: entregar software funcionando **com frequência** (semanas a meses, preferindo o mais curto) · aceitar **mudanças de requisitos, mesmo tarde** · negócio e desenvolvedores trabalham **juntos diariamente** · **conversa face a face** é o meio mais eficiente · **software funcionando é a principal medida de progresso** · **ritmo sustentável** · **simplicidade** (maximizar o trabalho não feito) · equipes **auto-organizáveis** · reflexão periódica para melhorar.

📌 É "**mais que**", não "**em vez de**": o próprio Manifesto diz que **há valor nos itens à direita**. Questão que diz "o ágil dispensa documentação/planejamento" → **falsa**.

### 4.2 Scrum

| | |
|---|---|
| 🎯 **Pra que serve** | Framework **leve de gestão** para resolver problemas complexos, entregando valor em ciclos curtos (Sprints) |
| 🏛️ **Onde é usado** | É o método ágil mais adotado no mundo; também em fábricas de software e equipes de TI do setor público. Ex.: equipe que evolui o módulo de audiências em Sprints de 2 semanas |
| 🤔 **Por que é assim** | Baseia-se no **empirismo**: em problemas complexos não dá para prever tudo, então se decide pelo que **se observa**. Por isso os eventos são pontos fixos de **inspeção e adaptação** |
| 🔧 **Origem** | Ken Schwaber e Jeff Sutherland (apresentado em 1995) · referência atual: **Guia do Scrum 2020** |

**🔧 Conceitos técnicos (Guia 2020):**

| Elemento | Conteúdo |
|---|---|
| **3 pilares do empirismo** | Transparência · Inspeção · Adaptação |
| **5 valores** | Compromisso · Foco · Abertura · Respeito · Coragem |
| **Scrum Team** (até ~10 pessoas, sem sub-times nem hierarquia) | **Product Owner** (maximiza o valor; dono do Product Backlog) · **Scrum Master** (eficácia do time; líder que serve) · **Developers** (criam o Incremento; donos do Sprint Backlog) |

| Evento | Timebox (Sprint de 1 mês) | Pra que serve |
|---|---|---|
| **Sprint** | Até 1 mês | "Contêiner" de todos os eventos |
| **Sprint Planning** | 8h | Por que (Sprint Goal), o que e como |
| **Daily Scrum** | 15 min | Developers inspecionam o progresso rumo à Sprint Goal |
| **Sprint Review** | 4h | Inspecionar o **produto** com stakeholders |
| **Sprint Retrospective** | 3h | Inspecionar o **processo** (pessoas, interações, ferramentas, DoD) |

| Artefato | → Compromisso (o que dá transparência) |
|---|---|
| Product Backlog | → **Product Goal** |
| Sprint Backlog | → **Sprint Goal** |
| Incremento | → **Definition of Done (DoD)** |

📌 Só o **PO** cancela a Sprint (se a Sprint Goal ficar obsoleta) · DoD **não** é artefato, é compromisso · refinamento **não** é evento · SM **não** distribui tarefas.

### 4.3 XP (Extreme Programming)

| | |
|---|---|
| 🎯 **Pra que serve** | Garantir **qualidade técnica do código** com mudanças constantes: é o método das **práticas de engenharia** |
| 🏛️ **Onde é usado** | Equipes pequenas e médias, requisitos que mudam muito. Na prática, suas práticas (TDD, CI, refatoração, pares) são usadas **junto com o Scrum** |
| 🤔 **Por que é assim** | Kent Beck (fim dos anos 1990) levou boas práticas ao "extremo": se revisar código é bom, revise o tempo todo (**programação em pares**); se testar é bom, teste antes (**test-first**); se integrar é bom, integre várias vezes ao dia (**CI**) |
| 🔧 **Valores** | Comunicação · Simplicidade · Feedback · Coragem · Respeito |

| Prática | O que é | 🤔 Por quê |
|---|---|---|
| **Histórias de usuário** + **jogo do planejamento** | Requisitos em cartões, priorizados pelo cliente | Planejar com o cliente, em pedaços pequenos |
| **Releases pequenos** | Entregas frequentes | Feedback rápido |
| **Test-first / TDD** | Teste que falha → código mínimo → refatorar | O teste vira especificação e rede de segurança |
| **Refatoração** | Mudar a estrutura **sem mudar o comportamento** | Evitar que o código degrade |
| **Projeto simples** | Só o necessário agora | Não gastar com o que talvez nunca seja usado |
| **Programação em pares** | Dois em um computador | Revisão contínua e conhecimento espalhado |
| **Propriedade coletiva** | **Qualquer um** altera qualquer parte do código | Sem "dono" que vire gargalo |
| **Integração contínua** | Integrar e testar várias vezes ao dia | Erro de integração aparece cedo |
| **Ritmo sustentável** | Sem horas extras em excesso | Cansaço gera defeitos |
| **Cliente no local** | Representante do usuário junto do time | Dúvida de requisito resolvida na hora |

📌 Histórias de usuário e cliente no local **nasceram na XP**, não são exclusivas do Scrum. Scrum = **gestão** · XP = **engenharia**.

**Escalamento (Sommerville):** **scaling up** = usar ágil em **sistema grande** (várias equipes) · **scaling out** = espalhar o ágil pela **organização inteira**.

### 4.4 Kanban

| | |
|---|---|
| 🎯 **Pra que serve** | Gerenciar **fluxo contínuo** de trabalho, tornando gargalos visíveis |
| 🏛️ **Onde é usado** | Sustentação, suporte, manutenção, demandas que chegam a qualquer hora. Ex.: fila de chamados de correção do sistema processual |
| 🤔 **Por que é assim** | Vem do Sistema Toyota de Produção (cartão *kanban* = sinal). Em trabalho que não cabe em Sprints, o que importa é o **fluxo**. Começar muitas coisas ao mesmo tempo **atrasa tudo**, por isso o WIP é limitado. Adaptado ao software por **David Anderson** |
| 🔧 **Conceitos técnicos** | **Quadro** com colunas (ex.: A fazer → Fazendo → Teste → Feito) · **limite de WIP** por coluna · **sistema puxado** (*pull*): só puxa um item novo quando há capacidade · políticas explícitas · melhoria contínua · **sem Sprints e sem papéis obrigatórios** |

| Métrica | Mede | Começa quando |
|---|---|---|
| **Lead time** | Visão do **cliente** | O pedido **entra** (é solicitado) → entrega |
| **Cycle time** | Visão do **time** | O trabalho **começa** → termina |
| **Throughput** (vazão) | Itens entregues por período | — |

📌 Lead time ≥ cycle time (o lead time inclui a espera na fila). Lei de Little: WIP médio = vazão × lead time médio → **menos WIP, menor lead time**.

### 4.5 Lean (Desenvolvimento de Software Enxuto)

| | |
|---|---|
| 🎯 **Pra que serve** | **Eliminar desperdício**: tudo o que não gera valor para o cliente |
| 🏛️ **Onde é usado** | Mais filosofia do que método. Sustenta o Kanban, o DevOps e a melhoria de processos |
| 🤔 **Por que é assim** | Adapta ao software a produção enxuta da Toyota. Adaptado por **Mary e Tom Poppendieck** |
| 🔧 **7 princípios** | Eliminar desperdícios · Construir qualidade (integrada) · Criar conhecimento · Adiar decisões (decidir o mais tarde possível, com mais informação) · Entregar rápido · Respeitar as pessoas · Otimizar o todo |

| 7 desperdícios no software (Poppendieck) | Exemplo |
|---|---|
| Trabalho parcialmente feito | Código pronto que não foi para produção |
| Funcionalidades extras | Relatório que ninguém usa |
| Reaprendizado | Redescobrir algo que não foi documentado |
| Transferências (*handoffs*) | Passar a demanda por muitas equipes |
| Atrasos (espera) | Esperar aprovação para começar |
| Troca de tarefas | Pessoa alocada em 4 projetos ao mesmo tempo |
| Defeitos | Bug que volta do usuário |

📌 A lista tem versões diferentes conforme o livro/edição (a da Toyota é: superprodução, espera, transporte, processamento extra, estoque, movimentação, defeitos). Na prova, reconheça a **ideia de desperdício**, não decore uma única lista.

### 4.6 SAFe (Scaled Agile Framework) · detalhar na Semana 2

| | |
|---|---|
| 🎯 **Pra que serve** | Aplicar ágil com **muitas equipes** e alinhar com estratégia e orçamento da organização |
| 🏛️ **Onde é usado** | Grandes empresas e órgãos com dezenas de equipes |
| 🤔 **Por que é assim** | O Scrum foi desenhado para **um** time; com 10 times no mesmo produto, é preciso sincronizar planejamento e entregas |
| 🔧 **Conceitos técnicos** | Configurações: Essential, Large Solution, Portfolio, Full · **ART** (Agile Release Train, "trem" de equipes) · **PI Planning** (planejamento de todo o trem, por incremento de programa) · **RTE** (Release Train Engineer, um "Scrum Master do trem") · criado por **Dean Leffingwell** |

📌 Todos os métodos deste grupo são **iterativos e incrementais**. A diferença em relação ao Grupo 3 é o foco: pessoas, software funcionando e resposta a mudanças, em vez de plano e documentação.

---

## Grupo 5 · Áreas transversais (valem para qualquer modelo)

### 5.1 Engenharia de requisitos (26 e 27/10)

| | |
|---|---|
| 🎯 **Pra que serve** | Descobrir, documentar e conferir **o que** o sistema deve fazer e **sob quais restrições** |
| 🤔 **Por que importa** | Erro de requisito é o **mais caro** de corrigir: ele contamina projeto, código e testes. Muitos fracassos de projeto começam aqui |

**Processo (Sommerville):**

| Etapa | O que faz | Técnicas / conceitos |
|---|---|---|
| **Elicitação** (descoberta) | Descobrir as necessidades com os **stakeholders** | Entrevistas (abertas/fechadas) · **etnografia** (observar o trabalho real) · cenários · casos de uso · workshops · prototipação |
| **Análise** | Classificar, organizar, **priorizar e negociar conflitos** | Ex.: a secretaria quer um campo obrigatório, o advogado quer simplicidade |
| **Especificação** | Registrar de forma clara | Documento de requisitos, casos de uso, histórias de usuário |
| **Validação** | Conferir se os requisitos são o que o cliente **realmente quer** | Revisões, **prototipação**, geração de casos de teste |
| **Gerenciamento** (contínuo) | Controlar mudanças e **rastreabilidade** | Matriz de rastreabilidade |

🔧 **Checagens da validação:** validade · consistência (sem conflitos) · completude · realismo (dá para fazer) · verificabilidade (dá para testar).
📌 É um processo **iterativo** (espiral): as etapas se repetem, não é uma sequência única.

**Tipos de requisito:**

| Tipo | Definição | Exemplo |
|---|---|---|
| **De usuário** | Alto nível, linguagem natural e diagramas, para o cliente | "O advogado deve poder peticionar on-line" |
| **De sistema** | Detalhado e preciso, pode ser **base do contrato** | "O sistema aceitará PDF de até 10 MB, assinado com certificado ICP-Brasil" |
| **Funcional (RF)** | **O que** o sistema faz | "Emitir certidão negativa" |
| **Não funcional (RNF)** | **Restrição/qualidade**: como, com que desempenho e segurança | "Responder em até 3 s com 5.000 usuários" |
| **Regra de negócio** | Política do negócio, que **existe mesmo sem o sistema** | "Prazo em dobro para a Defensoria" |

**RNF em 3 subtipos** (teste: "**quem exige isso?**"):

| Subtipo | Quem exige | Exemplos |
|---|---|---|
| **De produto** | O próprio **software** (comportamento) | Desempenho, disponibilidade, usabilidade, segurança |
| **Organizacional** | A **organização** (norma interna) | Linguagem obrigatória, processo de desenvolvimento, ambiente |
| **Externo** | **Fora** da organização (lei, regulação) | LGPD, normas do CNJ, acessibilidade legal |

📌 RNF precisa ser **mensurável e verificável**: "fácil de usar" é meta; "usuário treinado executa a tarefa em até 2 min" é requisito.

### 5.2 Histórias de usuário e critérios de aceitação (28/10)

| | |
|---|---|
| 🎯 **Pra que serve** | Descrever requisitos **do ponto de vista do valor** para o usuário, em pedaços pequenos |
| 🤔 **Por que é assim** | A história é um **lembrete de conversa**, não uma especificação completa: o detalhe vem do diálogo e dos critérios de aceitação |
| 🔧 **Formato** | "**Como** [papel], **quero** [funcionalidade], **para** [benefício]" |
| 🔧 **3 Cs** (Ron Jeffries) | **Cartão** (card) · **Conversa** · **Confirmação** (critérios de aceitação) |
| 🔧 **INVEST** (Bill Wake) | **I**ndependente · **N**egociável · **V**aliosa · **E**stimável · **S**mall (pequena) · **T**estável |
| 🔧 **Gherkin** (vem do BDD) | **Dado** [contexto] · **Quando** [ação] · **Então** [resultado esperado] (+ **E**, **Mas**) · é texto executável por ferramentas como o Cucumber |

Exemplo:
```gherkin
Cenário: Petição sem assinatura digital
  Dado que o advogado anexou uma petição em PDF sem assinatura
  Quando ele clicar em "Protocolar"
  Então o sistema deve recusar o envio
  E exibir a mensagem "Documento sem assinatura digital"
```

### 5.3 Estimativa ágil (29/10)

| | |
|---|---|
| 🎯 **Pra que serve** | Prever o tamanho do trabalho para planejar Sprints e releases |
| 🤔 **Por que é assim** | Pessoas estimam mal em horas absolutas, mas bem **por comparação** ("esta é o dobro daquela"). Por isso o ágil usa **tamanho relativo** |
| 🔧 **Story points** | Medida **relativa** que junta esforço + complexidade + incerteza · **velocidade** = pontos entregues por Sprint (serve para o próprio time; não compara times) |
| 🔧 **Planning Poker** | Cada um escolhe uma carta (sequência de Fibonacci modificada: 1, 2, 3, 5, 8, 13, 20, 40, 100) · **revelam ao mesmo tempo** (evita a **ancoragem**) · os extremos explicam e votam de novo até convergir · baseado no Wideband Delphi |
| 🔧 **T-shirt sizing** | PP, P, M, G, GG: estimativa grosseira para itens grandes ou backlog inicial |
| 🔧 **APF** (Semana 2) | Mede o **tamanho funcional** pela visão do usuário, independente da tecnologia. Muito usada em **contratos públicos** de software (paga-se por ponto de função) |

📌 Por que Fibonacci? Os intervalos crescem: quanto maior o item, **maior a incerteza**, então não faz sentido discutir 20 × 21.

### 5.4 Outras áreas (semanas seguintes)

| Área | Pra que serve | Assuntos | No plano |
|---|---|---|---|
| **Testes e qualidade** | Achar defeitos cedo e dar segurança para mudar | Níveis e tipos de teste, TDD, SAST/DAST, SonarQube | Semana 2 |
| **Projeto e arquitetura** | Organizar o código para ser fácil de mudar | UML, GoF, SOLID, arquitetura | Semanas seguintes |
| **Evolução e DevOps** | Entregar mudanças com frequência e segurança | Manutenção, CI/CD, gestão de configuração | Semana 10 |

---

## Linha do tempo (o "porquê" em uma olhada)

| Época | Marco | Problema que tentou resolver |
|---|---|---|
| 1968 | Conferência da OTAN cria o termo "engenharia de software" | Crise do software |
| 1970 | Royce descreve o modelo sequencial (cascata) | Falta de disciplina e controle |
| Anos 1980 | Espiral (Boehm) e Modelo em V | Risco e testes esquecidos no fim |
| Fim dos anos 1990 | RUP, UML, XP e Scrum | Processos rígidos × requisitos que mudam |
| 2001 | Manifesto Ágil | Documentação e plano em excesso |
| Anos 2000–2010 | Kanban no software, Lean, SAFe, DevOps | Fluxo contínuo, escala e entrega frequente |

---

## Como usar na prova

**Pegadinhas FGV clássicas:** "o RUP é sequencial" · "o espiral é incremental, e não iterativo" · "o ágil dispensa documentação" · "o Scrum Master cancela a Sprint" · "DoD é artefato". Para não cair:

1. Pergunte **em qual grupo** o item está (atividade, forma, modelo tradicional, ágil ou área).
2. Depois pergunte **qual "adjetivo"** ele tem (sequencial, iterativo, incremental).
3. Confira a **palavra-chave**:

| Palavra no enunciado | Pense em |
|---|---|
| Requisitos estáveis, aprovação de fase, documentação entre fases | **Cascata** |
| Cada fase com um nível de teste | **Modelo em V** |
| Entregas parciais já em uso | **Incremental** |
| Validar requisitos com o usuário, modelo descartável | **Prototipação** |
| Risco, voltas, cancelar o projeto | **Espiral** |
| Casos de uso, arquitetura, UML, 4 fases | **RUP** |
| Empirismo, Sprint, PO/SM/Developers | **Scrum** |
| Pares, TDD, refatoração, propriedade coletiva | **XP** |
| WIP, fluxo, lead/cycle time, puxado | **Kanban** |
| Desperdício, valor, otimizar o todo | **Lean** |
| ART, PI Planning, RTE | **SAFe** |

4. Em afirmações absolutas ("sempre", "dispensa", "somente", "em vez de"), desconfie e confira com a regra 📌.
