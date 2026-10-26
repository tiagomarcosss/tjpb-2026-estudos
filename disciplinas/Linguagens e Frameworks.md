---
tipo: disciplina
disciplina: "Linguagens e Frameworks"
tags: [disciplina]
---

# Linguagens e Frameworks

**Quando:** Semana 8 (14–20/12) · **Peso:** Conhecimentos Específicos

Voltar: [[00-HOME]] · Conteúdo detalhado: [[plano-tjpb]], seção 4.1

## Material

- Regras estudadas: [[regras-tjpb#Linguagens e Frameworks]]

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
    - 'disciplina.contains("Linguagens e Frameworks")'
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
