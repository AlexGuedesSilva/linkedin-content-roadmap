# Como contribuir

Este repositório usa um fluxo simples, baseado no estado editorial de cada post.

## Fluxo geral

1. Registre a ideia e confirme a série e o próximo número disponível.
2. Copie [o template](templates/post-template.md) para a pasta `backlog` da série, usando a convenção `NN-titulo-em-kebab-case.md`.
3. Marque **Ideia registrada** e preencha as informações já conhecidas, sem inventar datas, branches ou links.
4. Ao iniciar a produção, mova o arquivo para `in-progress` e atualize a navegação da série.
5. Preencha objetivo, mensagem principal, pontos da imagem, descrição, referências e observações; atualize o checklist durante o trabalho.
6. Depois da revisão e publicação, mova o arquivo para `published`, marque **Publicado** e mantenha **Agendado** conforme o processo realmente usado.
7. Adicione a data e o link reais da publicação.
8. Atualize a navegação e as contagens da série.
9. Atualize a tabela geral do README principal.

## Novo post da IAM Platform

A IAM Platform usa a estrutura `iam-platform/<status>/<capitulo>/NN-titulo.md`.

1. Confirme o próximo número e verifique se ele já existe em qualquer um dos três status.
2. Escolha o capítulo pelo assunto principal:
   - `01-foundation`: propósito, arquitetura inicial, módulos, DDD e Clean Architecture.
   - `02-identity`: identidade, entidades, Value Objects e casos de uso de usuário.
   - `03-persistence`: repositórios, adapters, JPA, mapeamento, banco e migrações.
   - `04-authentication`: credenciais, login, hashing e autenticação.
   - `05-token-and-session`: JWT, chaves, refresh token, sessões e revogação.
   - `06-authorization`: roles, permissions, RBAC, ABAC e policies.
   - `07-api-keys`: geração, hashing, escopos e revogação de API keys.
   - `08-audit`: auditoria, eventos de segurança e observabilidade de IAM.
   - `09-architecture-evolution`: evolução arquitetural, mensageria e microsserviços.
3. Copie o template para `iam-platform/backlog/<capitulo>/` e crie a pasta do capítulo apenas se houver um post para ela.
4. Nomeie o arquivo em kebab-case, com número de dois dígitos: `NN-titulo-em-kebab-case.md`. Use `refresh-token`, nunca `refreshtoken`.
5. Preserve a numeração histórica. Lacunas não devem ser preenchidas por renumeração automática.
6. Adicione o post ao [sumário](iam-platform/SUMMARY.md) e ao [roadmap](iam-platform/roadmap.md), com status **Backlog**.

## Mudança de status na IAM Platform

O capítulo não muda quando o post avança no fluxo:

```text
iam-platform/backlog/<capitulo>/
               ↓
iam-platform/in-progress/<capitulo>/
               ↓
iam-platform/published/<capitulo>/
```

Ao iniciar o trabalho:

1. Mova o arquivo para `in-progress/<capitulo>/`.
2. Atualize o status no `SUMMARY.md` e no `roadmap.md`.
3. Preencha branch ou feature somente quando essa relação existir.

Ao publicar:

1. Mova o arquivo para `published/<capitulo>/`.
2. Marque apenas as etapas realmente concluídas no checklist.
3. Preencha data e link reais da publicação.
4. Atualize caminhos, status e evidências de implementação no `SUMMARY.md` e no `roadmap.md`.
5. Atualize as contagens em `iam-platform/README.md` e no README principal.

## Verificação final

Antes de concluir, confira:

* estrutura e sintaxe do Markdown;
* número do post no arquivo, no título e no nome;
* nome em kebab-case;
* ausência do mesmo número em outro status;
* links relativos nos READMEs, no sumário e no roadmap;
* data e link de publicação somente quando conhecidos;
* preservação das instruções e do conteúdo técnico existente.
