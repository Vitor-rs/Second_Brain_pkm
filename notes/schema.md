---
id: schema
title: Esquema do PKM
desc: 'Visão geral da estrutura e esquema do PKM'
created: 2023-07-01
---

# Esquema do PKM

Este documento define o esquema de organização para o seu PKM, garantindo consistência e facilidade de navegação.

## Estrutura de Namespaces

O PKM segue uma estrutura hierárquica com os seguintes namespaces principais:

```
root
├── projects
│   ├── faculdade
│   ├── pessoal
│   └── trabalho
├── areas
│   ├── academica
│   ├── saude
│   ├── profissional
│   └── pessoal
├── resources
│   ├── programacao
│   ├── livros
│   ├── artigos
│   ├── documentarios
│   └── cursos
├── archives
│   ├── projetos-concluidos
│   └── semestres-anteriores
├── inbox
├── zettelkasten
│   ├── fleeting
│   ├── literature
│   └── permanent
└── mental-models
    ├── decision-making
    ├── systems-thinking
    └── problem-solving
```

## Convenções de Nomenclatura

### Projetos
- `projects.categoria.nome-do-projeto`
- Ex: `projects.faculdade.tcc`

### Áreas
- `areas.categoria.nome-da-area`
- Ex: `areas.academica.desenvolvimento-web`

### Recursos
- `resources.categoria.nome-do-recurso`
- Ex: `resources.livros.building-second-brain`

### Arquivos
- `archives.categoria.nome-do-arquivo`
- Ex: `archives.projetos-concluidos.site-2023`

### Zettelkasten
- Notas Passageiras: `fleeting.YYYY-MM-DD-HH-mm`
- Notas de Literatura: `literature.autor.titulo-abreviado`
- Notas Permanentes: `permanent.YYYY-MM-DD-HH-mm` ou `permanent.conceito-chave`

### Modelos Mentais
- `mental-models.categoria.nome-do-modelo`
- Ex: `mental-models.decision-making.second-order-thinking`

## Frontmatter Padrão

Cada nota deve incluir o seguinte frontmatter:

```yaml
---
id: [namespace.nome-da-nota]
title: [Título legível]
desc: '[Descrição breve]'
created: [YYYY-MM-DD]
updated: [YYYY-MM-DD]
tags: [tag1, tag2]
---
```

Campos adicionais por tipo de nota:

### Projetos
```yaml
status: active|planning|on-hold|completed
deadline: [YYYY-MM-DD]
```

### Recursos
```yaml
source: [Origem]
author: [Autor]
```

### Notas de Literatura
```yaml
author: [Autor]
source: [Referência completa]
```

## Hierarquia de Tags

Use tags para categorização transversal:

- Tipo de Conteúdo: #artigo, #livro, #curso, #video
- Status: #active, #completed, #archived
- Áreas de Conhecimento: #programacao, #banco-dados, #web
- Metodologias: #oop, #agile, #design-patterns

## Convenções de Links

- Use links explícitos com texto descritivo: `[[id-da-nota|Texto descritivo]]`
- Prefira links hierárquicos para navegar verticalmente na estrutura
- Use links associativos para conectar ideias relacionadas horizontalmente
- Evite links quebrados - verifique periodicamente
