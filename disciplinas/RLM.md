---
tipo: disciplina
disciplina: "RLM"
tags: [disciplina]
---

# RLM

**Quando:** Almoço (ter e qui) · **Peso:** Objetiva · 10 questões · meta 8

Voltar: [[00-HOME]] · Conteúdo detalhado: [[plano-tjpb]], seção 4.1

## Material

- Regras estudadas: [[regras-tjpb#Raciocínio Lógico-Matemático]]
- Prioridades: [[mapa-rlm-prioridades]]
- 56 questões FGV com gabarito: [[2026-10-26_FGV-RLM_Aula04-Problemas-de-Raciocinio_56-questoes.pdf]]

## Desempenho e arquivos

Tudo o que tiver `disciplina` igual a esta nota (blocos, correções, simulados, resumos):

```base
formulas:
  aproveitamento: 'if(total, (acertos / total * 100).round() + "%", "")'
properties:
  formula.aproveitamento:
    displayName: Aproveitamento
filters:
  and:
    - '!file.inFolder("modelos")'
    - 'disciplina.contains("RLM")'
    - 'tipo != "disciplina"'
views:
  - type: table
    name: Histórico
    order:
      - note.data
      - note.tipo
      - note.assunto
      - note.acertos
      - note.total
      - formula.aproveitamento
      - file.name
    sort:
      - property: note.data
        direction: DESC
```
