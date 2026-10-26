---
tipo: disciplina
disciplina: "Português"
tags: [disciplina]
---

# Português

**Quando:** Todo dia no almoço (seg, qua, sex) · **Peso:** Objetiva · 10 questões · meta 8

Voltar: [[00-HOME]] · Conteúdo detalhado: [[plano-tjpb]], seção 4.1

## Material

- Regras estudadas: [[regras-tjpb#Português]]
- Prova oficial: [[2026-10-23_Semana-00_FGV-DATAPREV_Portugues_PROVA]] · correção: [[2026-10-23_Semana-00_FGV-DATAPREV_Portugues_CORRECAO_v3]]

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
    - 'disciplina.contains("Português")'
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
