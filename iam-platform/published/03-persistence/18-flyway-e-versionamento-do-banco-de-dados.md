# IAM Platform — 18 — Flyway e versionamento do banco de dados

## Status

- [x] Ideia registrada
- [x] Conteúdo estudado
- [x] Roteiro definido
- [x] Imagem criada
- [x] Descrição criada
- [x] Revisado
- [x] Agendado
- [x] Publicado

---

## Informações

- Série: IAM Platform
- Número: 18
- Tema: Flyway e versionamento do banco de dados
- Data de criação: 12/07/2026
- Data de publicação: 12/07/2026
- Link da publicação: https://www.linkedin.com/feed/update/urn:li:share:7482152149234405376/
- Branch ou feature relacionada:
  - feature/identity-database-migration
- Tecnologias relacionadas:
  - Java 21
  - Spring Boot
  - Flyway
  - PostgreSQL
  - Docker Compose
  - Maven

---

## Objetivo do post

Mostrar por que bancos de dados também precisam ser versionados e como o Flyway resolve esse problema utilizando migrações versionadas.

Explicar que alterações de banco devem fazer parte do código-fonte da aplicação e não serem executadas manualmente.

---

## Mensagem principal

O banco de dados faz parte da aplicação.

Versionar scripts SQL garante reprodutibilidade, rastreabilidade e consistência entre desenvolvimento, homologação e produção.

---

## Pontos que devem aparecer na imagem

- Problema de executar SQL manualmente.
- Conceito de migração versionada.
- Estrutura do Flyway.
- Exemplo:
    V1__create_users_table.sql
- Fluxo:

Developer
      ↓
Git
      ↓
Flyway
      ↓
PostgreSQL

- Benefícios:
    ✔ Histórico
    ✔ Reprodutibilidade
    ✔ Controle de versão
    ✔ Deploy automatizado

Mensagem final:

"Banco de dados também é código."

---

## Rascunho da descrição

Ideias para abordar:

- Muitas equipes ainda alteram bancos manualmente.
- Isso gera ambientes diferentes.
- O Flyway elimina esse problema.
- Cada alteração possui uma versão.
- O Spring Boot executa automaticamente as migrações.
- Isso facilita CI/CD.
- Na IAM Platform utilizei Flyway para criar a tabela users de forma controlada.

---

## Referências de estudo

- Documentação oficial do Flyway
- Spring Boot + Flyway
- PostgreSQL Documentation

---

## Observações

Relacionar este conteúdo com os próximos posts:

19 - LoginUserUseCase

20 - JWT

21 - RS256

Também mencionar que esta implementação faz parte da evolução da IAM Platform.

## Implementação na IAM Platform

### O que foi implementado

- Configuração do Flyway
- Estrutura da pasta db/migration
- Primeira migration V1__create_users_table.sql
- Integração com PostgreSQL
- Execução automática na inicialização
- Validação das migrations

### Arquivos importantes

- pom.xml
- application.yml
- V1__create_users_table.sql

### Aprendizados

- O Flyway controla a versão do banco através da tabela flyway_schema_history.
- Nunca alterar uma migration já aplicada em produção.
- Novas mudanças devem sempre ser feitas criando uma nova versão (V2, V3...).