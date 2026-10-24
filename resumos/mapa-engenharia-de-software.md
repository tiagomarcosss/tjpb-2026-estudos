# Mapa geral · Engenharia de Software

**Criado em:** 24/10/2026 · Base: Sommerville (*Engenharia de Software*, material da UNIVESP) e Pressman, os autores mais usados pela FGV.

> Objetivo: se situar. Saber **em qual grupo** cada assunto está e **como os grupos se relacionam**.

---

## Mapa em uma linha

**Atividades fundamentais** → organizadas de forma **sequencial, iterativa ou incremental** → aplicadas por um **modelo** (tradicional: cascata, V, espiral, RUP · ágil: Scrum, XP, Kanban) → apoiadas por **áreas transversais** (requisitos, testes, arquitetura, DevOps).

```
GRUPO 1 · Atividades fundamentais (o QUE todo processo faz)
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

Não importa o modelo, todo processo de software passa por **4 atividades** (Sommerville):

**Especificação → Projeto e implementação → Validação → Evolução**

O que muda de um modelo para outro é **a ordem e quantas vezes** essas atividades se repetem.

---

## Grupo 2 · Os "adjetivos": formas de organizar as atividades

| Forma | Ideia | Imagem |
|---|---|---|
| **Sequencial** | Faz cada atividade uma vez, em ordem | Construir um prédio andar por andar, do projeto à entrega |
| **Incremental** | Entrega o sistema **em pedaços prontos**, um de cada vez | Primeiro a consulta, depois o peticionamento, depois as certidões |
| **Iterativo** | **Refaz e melhora** o mesmo produto em ciclos | Rascunho → versão 2 → versão 3 do mesmo texto |
| **Evolucionário** | Iterativo + incremental juntos | O que quase todo método moderno faz |

📌 Incremental **acrescenta**; iterativo **refina**.

---

## Grupo 3 · Os "substantivos": modelos tradicionais (dirigidos a planos)

Planejam tudo antes e documentam muito.

| Modelo | De quem | Forma | Palavra-chave na prova |
|---|---|---|---|
| **Cascata** | Winston Royce (1970), que na verdade o criticava | Sequencial | Requisitos estáveis, fase só começa após aprovação da anterior |
| **Modelo em V** | Variação do cascata | Sequencial | Cada fase tem um nível de teste correspondente |
| **Incremental** | Classificação do Sommerville e do Pressman | Incremental | Entregas parciais já em uso |
| **Prototipação** | Abordagem geral, sem autor único | Iterativa | Validar requisitos com um modelo descartável |
| **Espiral** | Barry Boehm (1986/88) | Iterativo, guiado por **risco** | Análise de riscos a cada volta |
| **RUP** | Rational Software (Jacobson, Booch e Rumbaugh, os criadores da UML), hoje da IBM | **Iterativo e incremental** | 4 fases (Concepção → Elaboração → Construção → Transição), UML, casos de uso |

📌 O RUP é o "meio-termo": tem fases, documentação e UML como os tradicionais, mas já é iterativo e incremental por dentro.

---

## Grupo 4 · Os métodos ágeis (o contraponto)

| Item | De quem | O que é |
|---|---|---|
| **Manifesto Ágil** | 17 autores (2001) | Os 4 valores e os 12 princípios, a "constituição" do ágil |
| **Scrum** | Schwaber e Sutherland | Framework de **gestão** (papéis, eventos, artefatos) |
| **XP** | Kent Beck | Práticas de **engenharia** (TDD, pares, refatoração, integração contínua) |
| **Kanban** | Origem na Toyota; adaptado ao software por David Anderson | **Fluxo** contínuo com limite de WIP, sem sprints |
| **Lean** | Origem na Toyota; adaptado ao software pelos Poppendieck | Eliminar desperdícios (7 desperdícios) |
| **SAFe** (escalamento) | Dean Leffingwell | Ágil para muitas equipes e para a organização inteira |

📌 Todos são **iterativos e incrementais**. A diferença em relação ao grupo 3 é o foco: pessoas, software funcionando e resposta a mudanças, em vez de plano e documentação.

---

## Grupo 5 · Áreas transversais (valem para qualquer modelo)

| Área | Assuntos | No plano |
|---|---|---|
| **Requisitos** | Elicitação, RF × RNF, usuário × sistema, histórias de usuário (INVEST), Gherkin | Semana 1 |
| **Estimativa e medição** | Planning Poker, story points, **APF** | Semanas 1–2 |
| **Testes e qualidade** | Níveis e tipos de teste, TDD | Semana 2 |
| **Projeto e arquitetura** | UML, padrões (GoF), SOLID, arquitetura | Semanas seguintes |
| **Evolução e DevOps** | Manutenção, integração e entrega contínuas, gestão de configuração | Semana 10 |

---

## Como usar na prova

**Pegadinha FGV clássica:** "o RUP é sequencial" ou "o espiral é incremental, e não iterativo". Para não cair nela:

1. Pergunte **em qual grupo** o item está (atividade, forma, modelo tradicional, ágil ou área).
2. Depois pergunte **qual "adjetivo"** ele tem (sequencial, iterativo, incremental).
3. Confira a **palavra-chave** da tabela: estável/aprovação → cascata · risco → espiral · validar requisitos → prototipação · arquitetura/casos de uso/UML → RUP.
