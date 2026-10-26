---
tipo: disciplina
disciplina: "Segurança"
tags: [disciplina]
---

# Segurança

**Quando:** Semana 11 (04–10/01) · **Peso:** Conhecimentos Específicos

Voltar: [[00-HOME]] · Conteúdo detalhado: [[plano-tjpb]], seção 4.1

## Material

- Regras estudadas: [[regras-tjpb#Segurança]]

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
    - 'disciplina.contains("Segurança")'
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
