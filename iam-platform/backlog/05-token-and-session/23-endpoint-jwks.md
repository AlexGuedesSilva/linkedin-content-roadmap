# IAM Platform — 23 — Endpoint JWKS

## Status

* [x] Ideia registrada
* [x] Conteúdo estudado
* [x] Roteiro definido
* [x] Imagem criada
* [ ] Descrição criada
* [ ] Revisado
* [ ] Agendado
* [ ] Publicado

---

## Informações

* **Série:** IAM Platform
* **Número:** 23
* **Tema:** Endpoint JWKS
* **Data de criação:** 16/07/2026
* **Data de publicação:**
* **Link da publicação:**
* **Branch ou feature relacionada:** `feature/token-jwt`
* **Tecnologias relacionadas:** Java 21, Spring Boot, JWT, JWK, JWKS, RS256, RSA, Nimbus JOSE + JWT

---

## Objetivo do post

Explicar como o endpoint JWKS publica chaves públicas para que aplicações e Resource Servers consigam validar JWTs assinados pela IAM Platform.

---

## Mensagem principal

O endpoint JWKS permite distribuir somente as chaves públicas necessárias para validar assinaturas JWT, mantendo a chave privada protegida no servidor emissor.

---

## Pontos que devem aparecer na imagem

* Fluxo entre Auth Server, cliente, Resource Server e JWKS.
* Endpoint `/.well-known/jwks.json`.
* Estrutura de uma JWK RSA.
* Campos `kty`, `use`, `alg`, `kid`, `n` e `e`.
* Uso do `kid` para escolher a chave correta.
* Validação da assinatura RS256.
* Diferença entre chave pública e chave privada.
* Cache e headers HTTP.
* Rotação de chaves.
* Boas práticas de segurança.
* Exemplos conceituais de implementação com Spring Boot.

---

## Rascunho da descrição

Adicionar posteriormente.

---

## Referências de estudo

* RFC 7517 — JSON Web Key
* RFC 7515 — JSON Web Signature
* RFC 7518 — JSON Web Algorithms
* RFC 7519 — JSON Web Token
* Spring Security Reference Documentation
* Nimbus JOSE + JWT Documentation

---

## Observações

* Somente a chave pública deve ser publicada.
* A chave privada nunca deve aparecer no JWKS.
* O `kid` do JWT deve corresponder ao `kid` da chave publicada.
* O endpoint deve ser público, somente leitura e cacheável.
* Este post aprofunda a visão geral apresentada no Post 19.