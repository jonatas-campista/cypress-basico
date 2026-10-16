# Cypress Básico — testes E2E com integração contínua

![Cypress](https://img.shields.io/badge/Cypress-17202C?logo=cypress&logoColor=white) ![GitHub Actions](https://img.shields.io/badge/GitHub%20Actions-2088FF?logo=githubactions&logoColor=white)

Testes end-to-end da aplicação **CAC TAT** (Central de Atendimento ao Cliente), um formulário de
contato, feitos durante o curso básico de Cypress da Escola TAT.

## O que é testado

- Preenchimento e envio do formulário, com mensagem de sucesso e de erro.
- Validação de campos obrigatórios e de e-mail inválido.
- Campos de seleção: `select`, `radio` e `checkbox`.
- Upload de arquivo (seleção e arrastar e soltar).
- Links que abrem em nova aba, sem sair da aplicação.
- Comandos customizados, `cy.clock` / `cy.tick`, `.invoke()`, requisições HTTP com `cy.request` e execução em viewport mobile.

## Integração contínua

Os testes rodam automaticamente a cada push com **GitHub Actions** (`.github/workflows/ci.yml`).

## Como rodar

```bash
npm install
npm test              # headless, desktop
npm run test:mobile   # headless, viewport mobile
npm run cy:open       # modo interativo
```

## Créditos

Fork do projeto [cypress-basico-v2](https://github.com/wlsf82/cypress-basico-v2), de Walmyr Filho
(Escola TAT). Os testes em `cypress/e2e/` foram escritos por mim durante o curso.
