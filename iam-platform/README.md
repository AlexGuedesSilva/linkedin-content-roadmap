# IAM Platform

Esta área acompanha a construção progressiva de uma plataforma de Identity and Access Management (IAM). Ela funciona ao mesmo tempo como roadmap editorial da série, documentação da implementação, histórico cronológico do projeto e material didático para estudo e entrevistas técnicas.

## Objetivo da série

A série registra decisões, conceitos e incrementos da IAM Platform em ordem numérica. Cada post relaciona um assunto técnico à evolução da plataforma, sem tratar a existência de um roteiro como evidência de que a respectiva feature já foi implementada.

## Tecnologias e temas principais

Java 21, Spring Boot, Spring Security, PostgreSQL, Flyway, JWT, JWS, RS256, JWKS, DDD, Clean Architecture, arquitetura hexagonal, monólito modular, persistência, autenticação, autorização e segurança de sessões.

## Como navegar

- [Sumário técnico](SUMMARY.md): leitura em formato de livro, organizada por capítulo e número.
- [Roadmap](roadmap.md): visão editorial e técnica, incluindo branches ou features quando documentadas.
- [Glossário](glossary.md): definições curtas dos principais conceitos da série.
- Por status: `backlog`, `in-progress` e `published` indicam o estado editorial.
- Por capítulo: dentro de cada status, as pastas numeradas agrupam conteúdos do mesmo tema.

Os capítulos atuais são:

1. `01-foundation`
2. `02-identity`
3. `03-persistence`
4. `04-authentication`
5. `05-token-and-session`
6. `06-authorization`
7. `07-api-keys`
8. `08-audit`
9. `09-architecture-evolution`

Pastas de capítulo só existem em um status quando há conteúdo correspondente, evitando diretórios vazios sem perder a convenção de nomes.

## Posts, branches e features

O campo **Branch ou feature relacionada** de cada post conecta o conteúdo editorial à implementação quando essa informação está disponível. Uma branch citada documenta uma relação com o código; um post no backlog continua sendo apenas conteúdo planejado e não confirma que a feature esteja pronta. O [roadmap](roadmap.md) explicita essa diferença.

## Fluxo editorial

```text
backlog
   ↓
in-progress
   ↓
published
```

Mover um arquivo, mantendo o mesmo capítulo, representa a evolução editorial do conteúdo. O checklist e os metadados do próprio post devem ser atualizados apenas quando cada etapa realmente ocorrer.

## Situação atual

| Status | Quantidade | Significado |
|---|---:|---|
| Publicado | 21 | Conteúdo com publicação registrada no arquivo |
| Em andamento | 0 | Conteúdo em produção |
| Backlog | 10 | Conteúdo planejado, sem pressupor implementação |
| **Total** | **31** | Posts existentes |

## Próximos passos

Para iniciar um conteúdo, mova-o de `backlog/<capitulo>/` para `in-progress/<capitulo>/`. Depois da publicação, mova-o para `published/<capitulo>/`, preencha data e link reais e atualize o [sumário](SUMMARY.md), o [roadmap](roadmap.md) e as contagens relevantes. Consulte também o [guia de contribuição](../CONTRIBUTING.md).
