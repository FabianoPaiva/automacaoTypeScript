# 🚀 API Automation Framework: Playwright + TypeScript

[![TypeScript](https://img.shields.io/badge/TypeScript-007ACC?style=for-the-badge&logo=typescript&logoColor=white)](https://www.typescriptlang.org/)
[![Playwright](https://img.shields.io/badge/Playwright-2EAD33?style=for-the-badge&logo=playwright&logoColor=white)](https://playwright.dev/)
[![Postman](https://img.shields.io/badge/Postman-FF6C37?style=for-the-badge&logo=postman&logoColor=white)](https://www.postman.com/)
[![CI/CD Pipeline](https://img.shields.io/badge/CI%2FCD-GitHub%20Actions-2088FF?style=for-the-badge&logo=github-actions&logoColor=white)](https://github.com/)

Framework robusto e escalável de automação de testes de API REST desenvolvido em **TypeScript**, utilizando o motor de requisições nativo do **Playwright** (`APIRequestContext`). Este repositório foi estruturado para atender aos padrões de mercado, integrando contratos de coleções do **Postman** e validadores tipados inspirados em boas práticas de mercado (estilo BDD/Fluent Assertions).

---

## 🛠️ Tecnologias e Ferramentas

*   **[TypeScript](https://www.typescriptlang.org/)**: Superset JavaScript que traz tipagem estática e segurança em tempo de desenvolvimento.
*   **[Playwright Test](https://playwright.dev/)**: Gerenciador de testes e cliente HTTP de alta performance (`request`).
*   **[Postman / Newman](https://www.postman.com/)**: Utilizado para exploração manual de endpoints, design inicial das requisições e execução de collections em pipeline via CLI.
*   **[Dotenv](https://github.com/motdotla/dotenv)**: Gerenciamento seguro de variáveis de ambiente.

---

## 📁 Estrutura do Projeto

A organização dos diretórios segue o padrão Page/Service Object Model aplicado a APIs, separando dados, requisições e asserções:

```text
├── .github/
│   └── workflows/
│       └── pipeline.yml       # Configuração de CI/CD (GitHub Actions)
├── src/
│   ├── config/
│   │   └── environment.ts     # Configurações globais e base URLs
│   ├── data/
│   │   └── payloads/          # Payloads estáticos e geradores de massa
│   ├── models/                # Tipos e Interfaces TypeScript (Contracts)
│   ├── services/              # Camada de requisições (Endpoints encapsulados)
│   └── utils/                 # Funções auxiliares (Geração de tokens, massas)
├── tests/
│   ├── contract/              # Testes de contrato e schema JSON
│   ├── functional/            # Testes funcionais (GET, POST, PUT, DELETE)
│   └── e2e-api/               # Fluxos end-to-end integrados via API
├── postman/
│   ├── collection.json        # Coleção oficial exportada do Postman
│   └── environment.json       # Variáveis de ambiente do Postman
├── playwright.config.ts       # Configurações globais do Playwright
├── package.json
└── README.md