# IAM Platform — 22 — JWT com RS256

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
* **Número:** 22
* **Tema:** JWT com RS256
* **Data de criação:** 16/07/2026
* **Data de publicação:**
* **Link da publicação:**
* **Branch ou feature relacionada:** `feature/token-jwt`
* **Tecnologias relacionadas:** Java 21, Spring Boot, JWT, JWS, RS256, RSA, Nimbus JOSE + JWT, Spring Security

---

## Objetivo do post

Explicar como funciona a assinatura de Access Tokens JWT utilizando RS256, destacando a separação entre chave privada e chave pública.

---

## Mensagem principal

No RS256, a chave privada permanece protegida no servidor responsável pela emissão do token, enquanto a chave pública pode ser distribuída aos serviços consumidores para validar sua assinatura sem compartilhar segredos.

---

## Pontos que devem aparecer na imagem

* Estrutura do JWT: Header, Payload e Signature.
* Significado do algoritmo RS256.
* Papel da chave privada.
* Papel da chave pública.
* Fluxo de assinatura do JWT.
* Fluxo de validação em um Resource Server.
* Uso do campo `kid`.
* Claims utilizadas na IAM Platform.
* Geração conceitual do par de chaves RSA.
* Benefícios de segurança e escalabilidade.
* Boas práticas de armazenamento e rotação de chaves.

---

## Rascunho da descrição

Adicionar posteriormente.

---

## Referências de estudo

* RFC 7519 — JSON Web Token
* RFC 7515 — JSON Web Signature
* RFC 7518 — JSON Web Algorithms
* Spring Security Reference Documentation
* Nimbus JOSE + JWT Documentation

---

## Observações

* O Access Token da IAM Platform é assinado utilizando RS256.
* A chave privada não deve ser publicada ou versionada.
* A chave pública será disponibilizada por meio do endpoint JWKS.
* Este post aprofunda a visão geral apresentada no Post 19.