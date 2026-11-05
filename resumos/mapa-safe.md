---
tipo: resumo
disciplina: ["APF, SAFe e Testes"]
assunto: "Mapa de SAFe (ART, PI, papéis, backlog, PI Planning, WSJF, configurações)"
data: 2026-11-05
atualizado: 2026-11-05
---

# Mapa · SAFe (Scaled Agile Framework)

**Criado em:** 05/11/2026 · **Nível no plano:** 🟡 (Semana 2) · **Base:** SAFe 6.0 (framework.scaledagile.com), com as diferenças da versão 5 indicadas.

> **Como ler cada ficha:**
> 🎯 **Pra que serve** · 🏛️ **Onde é usado** · 🤔 **Por que é assim** · 🔧 **Conceitos técnicos** · 📌 **Regra/pegadinha FGV**
>
> O "Novo PJe-PB" usado nos exemplos é **fictício**, só para fixar a ideia. Não descreve como o TJPB trabalha.

> ⚠️ **Versão:** no SAFe 6.0, *Program Increment* virou **Planning Interval** (a sigla PI continua), *Program Backlog* virou **ART Backlog**, *Program Board* virou **ART Planning Board** e *Scrum Master* virou **Scrum Master/Team Coach**. Provas mais antigas podem usar os nomes da versão 5. O edital não diz qual versão a FGV usa.

---

## 0. Por que o SAFe existe

| | |
|---|---|
| 🎯 **Pra que serve** | Fazer **vários times** trabalharem como um só no mesmo sistema: mesmo calendário, mesmo planejamento, mesma demo, mesma fila de prioridades |
| 🏛️ **Onde é usado** | Organizações grandes e tradicionais (bancos, governo, telecom, defesa, indústria). As big techs, em geral, **não** usam SAFe |
| 🤔 **Por que é assim** | Com vários times em Scrum isolado, cada um tem seu calendário, as dependências aparecem tarde, ninguém testa o sistema inteiro e as prioridades entram em conflito |
| 🔧 **Ideia central** | **SAFe = Scrum escalado.** Dentro de cada time continua o Scrum (ou o Kanban). O SAFe acrescenta as camadas **acima** dos times |

**Exemplo:** o "Novo PJe-PB" com 8 times (peticionamento, intimações, custas, painel do magistrado, integração com o Gov.br…).

---

## 1. ART (Agile Release Train): o trem

| | |
|---|---|
| 🎯 **Pra que serve** | Juntar os times que entregam um mesmo fluxo de valor num "time de times" |
| 🤔 **Por que "trem"** | Sai no horário e não espera ninguém (cadência fixa: a feature atrasada vai no próximo trem) · todos os vagões andam juntos (as mesmas datas para todos) · o trem é permanente |
| 🔧 **Conceitos** | **5 a 12 times · 50 a 125 pessoas** (limite de Dunbar) · **permanente** (não é desmontado no fim do projeto) · organizado em torno de um **fluxo de valor**, não de um projeto |

📌 ART = time de times, **permanente**, organizado por **valor**, de **50 a 125 pessoas**, com cadência sincronizada.

---

## 2. Calendário: iteração e PI

```
              ←──────────── 1 PI (8 a 12 semanas) ────────────→
 PI Planning │ Iteração 1 │ Iteração 2 │ Iteração 3 │ Iteração 4 │ IP │ → PI Planning do próximo
   (2 dias)  │  2 semanas │  2 semanas │  2 semanas │  2 semanas │    │
                    ↓            ↓            ↓            ↓       ↓
               System Demo  System Demo  System Demo  System Demo  Inspect & Adapt
```

| Peça | O que é | No Scrum seria… |
|---|---|---|
| **Iteração** | Sprint de cada time, normalmente de **2 semanas**, com as **mesmas datas para todos** | Sprint |
| **PI** | Em geral, **4 iterações de desenvolvimento + 1 IP** (8 a 12 semanas) | "Sprint grande" do trem |
| **PI Planning** | Planejamento do PI com **todo o ART** (2 dias) | Sprint Planning em escala |
| **System Demo** | Demo do **sistema integrado**, no fim de **cada iteração** | Sprint Review (integrada) |
| **IP Iteration** | Inovação e Planejamento | — |
| **Inspect & Adapt** | Retrospectiva no **fim do PI** | Retrospectiva em escala |

📌 **Iteração = 2 semanas (time) · PI = 8 a 12 semanas (trem).**

---

## 3. Papéis: o mesmo trio em cada andar

| Função | Time | **ART** | Solution Train |
|---|---|---|---|
| Define **o quê** (conteúdo e prioridade) | Product Owner | **Product Management** | Solution Management |
| **Facilita** (líder-servidor) | Scrum Master/Team Coach | **RTE** (Release Train Engineer) | STE (Solution Train Engineer) |
| **Como técnico** | (os Developers) | **System Architect** | Solution Architect |

- **Business Owners:** os "donos do negócio" do ART. Respondem pelo retorno do investimento e **dão nota de valor de negócio (1 a 10)** aos objetivos do PI de cada time.
- **System Architect:** cuida da **Architectural Runway** (a "pista" técnica já pronta para as próximas features).

| Exemplo no Novo PJe-PB | Papel |
|---|---|
| Conduz o PI Planning, remove impedimentos entre os times e acompanha os riscos | **RTE** |
| Decide quais features o trem faz no PI | **Product Management** |
| Escreve e prioriza as stories do time de custas | **Product Owner** |
| Define que os módulos vão conversar por mensageria | **System Architect** |
| Aprova o investimento e pontua o valor dos objetivos | **Business Owner** |

📌 **RTE = Scrum Master do trem.** É líder-servidor, **não é gerente**, não define escopo e não manda nos times. Quem define o escopo do ART é o **Product Management**.

---

## 4. Backlog: o tamanho decide o nível

| Item | Tamanho | Onde vive | Dono | Exemplo |
|---|---|---|---|---|
| **Épico** | Vários PIs. Precisa de **Lean Business Case** + **MVP** | Portfólio | Epic Owner | "Peticionamento 100% digital com triagem automática" |
| **Capability** | Cabe num PI, mas envolve **vários ARTs** | Solution Train | Solution Management | (só no Large Solution) |
| **Feature** | **Cabe em 1 PI**. Tem **hipótese de benefício** + critérios de aceite | ART Backlog | **Product Management** | "Assinatura ICP-Brasil no peticionamento" |
| **Story** | **Cabe em 1 iteração** | Team Backlog | **PO** | "Como advogado, quero anexar PDF de até 10 MB…" |

- **Enabler:** item **técnico** (arquitetura, infraestrutura, exploração, conformidade). Pode existir em **qualquer nível**. Constrói a Architectural Runway.

📌 **Épico > Capability > Feature (1 PI) > Story (1 iteração).** Feature → Product Management · Story → PO.

---

## 5. PI Planning

| | |
|---|---|
| 🎯 **Pra que serve** | Alinhar **todo o ART** sobre o que será entregue no PI e descobrir as **dependências** antes de começar |
| 🔧 **Formato** | **2 dias**, ART inteiro (presencial ou remoto) |

| Dia 1 | Dia 2 |
|---|---|
| Contexto de negócio (Business Owners) | Ajustes da gestão |
| Visão do produto (Product Management) e de arquitetura (System Architect) | **Breakout 2**: os times fecham o plano; os **Business Owners dão valor de 1 a 10** aos objetivos |
| **Breakout 1**: cada time quebra as features em stories, distribui pela **capacidade** e marca dependências | Revisão final dos planos |
| Revisão do rascunho | **Riscos do ART (ROAM)** |
| Revisão da gestão (à noite, ajusta escopo) | **Voto de confiança** (1 a 5 dedos). Confiança baixa → **o plano é retrabalhado na hora** |
| | Retrospectiva do PI Planning |

**ROAM (riscos):**

| Letra | Significado | Exemplo |
|---|---|---|
| **R**esolved | Resolvido, deixou de ser risco | "A licença já foi comprada" |
| **O**wned | Alguém assume a responsabilidade de tratar | "O Diego acompanha a API do Gov.br" |
| **A**ccepted | Aceito; não há o que fazer | "Pode haver greve; aceitamos" |
| **M**itigated | Há um plano para reduzir o impacto | "Se o Gov.br atrasar, login local temporário" |

**Saídas:**

| Saída | O que é |
|---|---|
| **Objetivos do PI** | O que cada time (e o ART) pretende entregar, em linguagem de negócio: **comprometidos** × **não comprometidos** |
| **ART Planning Board** (antigo *Program Board*) | Features por iteração, **marcos** e **dependências** entre times ("barbante vermelho") |

- **Não comprometido:** **está no plano e consome capacidade**, mas tem incerteza alta. Também recebe valor de negócio. Se não sair, não é promessa quebrada. Serve para dar **previsibilidade**.

📌 Objetivo não comprometido **não é "extra se sobrar tempo"**: entra no plano e na capacidade, só não conta como compromisso.

---

## 6. Durante o PI

| Evento | Quando | Quem | Para quê |
|---|---|---|---|
| Eventos Scrum | Toda iteração | Cada time | Planning, Daily, Review, Retro |
| **ART Sync** = Coach Sync + PO Sync | Semanal | — | Sincronizar o trem |
| ↳ **Coach Sync** (no SAFe 5, *Scrum of Scrums*) | Semanal | RTE + Scrum Masters | Impedimentos e dependências |
| ↳ **PO Sync** | Semanal | Product Management + POs | Escopo e prioridade |
| **System Demo** | Fim de **cada iteração** | ART + stakeholders | **Sistema integrado** funcionando |

📌 **System Demo = sistema integrado**, não cada time mostrando seu pedaço. É o princípio nº 5: o progresso se mede por **sistema funcionando**, não por documento.

---

## 7. Fim do PI

**IP Iteration (Inovação e Planejamento):**

| Serve para | Não serve para |
|---|---|
| Inovação, hackathon, explorar tecnologia | Planejar features nela |
| Capacitação, infraestrutura, dívida técnica | Ser a "lixeira" do trabalho atrasado |
| Inspect & Adapt e PI Planning do próximo PI | — |
| **Margem de estimativa** (*buffer*) | — |

**Inspect & Adapt (3 partes):**
1. **Demo do PI** (tudo o que o trem entregou);
2. **Medição**, incluindo a **previsibilidade** (valor de negócio entregue ÷ planejado; faixa saudável de 80% a 100%);
3. **Workshop de solução de problemas** (causa raiz: 5 porquês, espinha de peixe), cujas ações entram no próximo PI Planning.

---

## 8. Priorização: WSJF

> **WSJF = Custo do Atraso ÷ Tamanho do trabalho**
>
> **Custo do Atraso = Valor para o negócio/usuário + Criticidade de tempo + Redução de risco/Habilitação de oportunidade**

Notas relativas em Fibonacci (1, 2, 3, 5, 8, 13, 20).

| Feature | Valor | Tempo | Risco/Oport. | Custo do Atraso | Tamanho | **WSJF** |
|---|---|---|---|---|---|---|
| A · Assinatura ICP-Brasil | 8 | 5 | 2 | 15 | 5 | **3,0** |
| B · Painel com IA | 13 | 8 | 3 | 24 | 13 | **1,8** |
| C · Aviso de prazo por e-mail | 3 | 2 | 1 | 6 | 1 | **6,0** |

**Ordem: C → A → B.** A B tem o maior valor, mas fica por último porque é grande demais.

📌 **WSJF divide pelo tamanho:** maior WSJF primeiro. "Maior valor primeiro" e "menor tarefa primeiro" são pegadinhas.

---

## 9. Entrega: "develop on cadence, release on demand"

| Frase | Significado |
|---|---|
| **Develop on cadence** | O **desenvolvimento** segue o ritmo fixo (iterações e PIs) |
| **Release on demand** | A **entrega ao usuário** acontece quando o negócio quiser |

**Continuous Delivery Pipeline (4 aspectos):**

```
Continuous Exploration → Continuous Integration → Continuous Deployment → Release on Demand
(o que construir?          (build + testes           (vai para produção,       (libera para o
 hipóteses, pesquisa)       automatizados)            pode ficar oculto)        usuário)
```

📌 **Deploy ≠ Release.** Deploy = colocar em produção (pode ficar oculto atrás de uma **feature toggle**). Release = disponibilizar ao usuário.

---

## 10. Portfólio (🟡: só o essencial)

| Conceito | O que é |
|---|---|
| **LPM** (*Lean Portfolio Management*) | Estratégia, financiamento e governança do portfólio |
| **Orçamento lean** | **Financia fluxos de valor (trens), não projetos**, com limites (*guardrails*) |
| **Portfolio Kanban** | Fluxo dos épicos: Funil → Revisão → Análise → Pronto → Implementação → Concluído |
| **Épico** | Exige **Lean Business Case** + **MVP** |
| **Temas estratégicos** | Objetivos de negócio que guiam o portfólio |

📌 **SAFe financia fluxo de valor, não projeto.** Por isso o ART é permanente.

---

## 11. As 4 configurações

| Configuração | Quando usar | O que acrescenta |
|---|---|---|
| **Essential** | Um sistema com até ~125 pessoas | Times + ART + PI Planning. **Base de todas** |
| **Large Solution** | A solução exige **vários ARTs e fornecedores** | **Solution Train**, Capabilities, STE, Solution Management, Solution Demo |
| **Portfolio** | Ligar estratégia e orçamento aos trens | Épicos, LPM, orçamento lean, Portfolio Kanban |
| **Full** | Organizações gigantes | Tudo junto |

**Caso real de Large Solution:** a Telia Finlândia (telecom) adotou o Large Solution para coordenar **mais de 200 sistemas** e **vários fornecedores externos**. Hoje opera **2 ARTs e 2 Solution Trains, com cerca de 350 pessoas** (fonte: caso publicado pela própria Scaled Agile, que é material de divulgação).

📌 **Large Solution = coordenar vários ARTs e fornecedores numa solução só.** O gatilho é a **complexidade e a dependência entre trens**, não só o número de pessoas.

---

## 12. Fundamentos (podem cair em I/II/III)

**Valores centrais:**

| SAFe 6.0 | SAFe 5.x |
|---|---|
| Alinhamento | Alinhamento |
| Transparência | Transparência |
| Respeito pelas pessoas | Qualidade embutida (*Built-in Quality*) |
| Melhoria incessante | Execução do programa |

**Os 10 princípios Lean-Agile:**

| # | Princípio | Onde aparece |
|---|---|---|
| 1 | Visão **econômica** | WSJF, custo do atraso |
| 2 | **Pensamento sistêmico** | Otimizar o todo, não cada time |
| 3 | Assumir a **variabilidade**, preservar opções | Não decidir cedo demais |
| 4 | Construir **incrementalmente**, com ciclos rápidos e integrados de aprendizado | Iterações + System Demo |
| 5 | Marcos baseados em **avaliação objetiva de sistemas funcionando** | System Demo, não documento |
| 6 | Fazer o **valor fluir sem interrupções** (no 5.x: limitar o WIP, reduzir lotes, gerenciar filas) | Kanban |
| 7 | **Cadência** + sincronização com planejamento entre domínios | PI Planning |
| 8 | Liberar a **motivação intrínseca** | Autonomia |
| 9 | **Descentralizar** decisões | Frequentes → times · estratégicas → gestão |
| 10 | **Organizar em torno de valor** | ARTs por fluxo de valor |

---

## 🎯 Se lembrar só de 10 coisas

1. SAFe = Scrum escalado; dentro do time continua o Scrum.
2. **ART** = 5 a 12 times, 50 a 125 pessoas, **permanente**, organizado por valor.
3. **Iteração** = 2 semanas · **PI** = 8 a 12 semanas (4 iterações + IP).
4. **RTE** = Scrum Master do trem (líder-servidor, não gerente).
5. **Product Management** → Features · **PO** → Stories.
6. Feature cabe em **1 PI** · Story cabe em **1 iteração**.
7. **PI Planning**: 2 dias, ART inteiro, **objetivos do PI** + **ART Planning Board**, **ROAM**, **voto de confiança**.
8. **System Demo** = integrado, a cada iteração · **I&A** = fim do PI.
9. **WSJF = Custo do Atraso ÷ Tamanho.**
10. **Develop on cadence, release on demand** · deploy ≠ release.

## Pegadinhas FGV

| A alternativa diz… | Errado porque… |
|---|---|
| "O RTE é o PO do ART" | O RTE é o Scrum Master do ART. O "PO do ART" é o Product Management |
| "O PI Planning ocorre a cada iteração" | Ocorre a cada **PI** |
| "A Feature deve caber numa iteração" | Quem cabe numa iteração é a **Story**. A Feature cabe num **PI** |
| "A IP Iteration serve para concluir o trabalho atrasado" | É para inovação e planejamento. A margem é efeito colateral |
| "A release só ocorre ao fim do PI" | **Release on demand** |
| "O ART tem até 50 pessoas" | São **50 a 125** |
| "Objetivos não comprometidos ficam fora do plano" | Entram no plano e na capacidade, só não contam como compromisso |
| "O ART é desmontado ao fim do projeto" | É **permanente**: o SAFe financia fluxos de valor |

---

**Fontes:** [SAFe · Solution Train](https://framework.scaledagile.com/solution-train) · [SAFe · Large Solution](https://framework.scaledagile.com/large-solution) · [Caso Telia Finlândia (Scaled Agile)](https://scaledagile.com/case_study/telia-finland/)

Voltar: [[APF, SAFe e Testes]] · [[00-HOME]]
