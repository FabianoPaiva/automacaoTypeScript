# 🤖 Automação TypeScript

> Repositório estruturado para estudos, nivelamento e desenvolvimento de testes automatizados e integrações utilizando **TypeScript**.

---

### 🛠️ Tecnologias e Ferramentas

| Categoria | Badges |
| :--- | :--- |
| **Linguagens** | ![TypeScript](https://img.shields.io/badge/TypeScript-007ACC?style=for-the-badge&logo=typescript&logoColor=white) |
| **Frameworks Backend** | ![Postman](https://img.shields.io/badge/Postman-FF6C37?style=for-the-badge&logo=postman&logoColor=white) ![Newman](https://img.shields.io/badge/Newman-FF6C37?style=for-the-badge&logo=postman&logoColor=white) |
| **Automação e QA** | ![Playwright](https://img.shields.io/badge/Playwright-2EAD33?style=for-the-badge&logo=playwright&logoColor=white) |
| **Ferramentas e CI/CD** | ![Git](https://img.shields.io/badge/Git-F05032?style=for-the-badge&logo=git&logoColor=white) ![GitHub Actions](https://img.shields.io/badge/GitHub_Actions-2088FF?style=for-the-badge&logo=github-actions&logoColor=white) ![CI/CD Pipeline](https://img.shields.io/badge/CI%2FCD-GitHub%20Actions-2088FF?style=for-the-badge&logo=github-actions&logoColor=white) |

---

## 📋 Índice

- [Sobre o Projeto](#-sobre-o-projeto)
- [Estrutura do Projeto](#-estrutura-do-projeto)
- [Tecnologias Utilizadas](#-tecnologias-utilizadas)
- [Pré-requisitos](#-pré-requisitos)
- [Instalação e Configuração](#-instalação-e-configuração)
- [Como Executar os Testes e Scripts](#-como-executar-os-testes-e-scripts)
- [Autor](#-autor)

---

## 💡 Sobre o Projeto

Este projeto centraliza rotinas de automação, testes e práticas avançadas em TypeScript. Ele está dividido em módulos de nivelamento, lógica assíncrona, testes automatizados (como testes de login) e consumo/validação de APIs.

---

## 📂 Estrutura do Projeto

A organização dos diretórios segue uma separação limpa entre lógica de nivelamento, automações de aulas específicas, utilitários e testes:

```text
automacaoTypeScript/
├── src/
│   ├── aula28/            # Módulo/Aula 28: Integrações e consumo de APIs
│   │   └── apis.ts
│   ├── aula28.ts          # Script principal da aula 28
│   ├── aula29/            # Módulo/Aula 29: Testes automatizados de API
│   │   └── apis2.test.ts
│   ├── nivelamento/       # Módulo de Fundamentos
│   │   ├── funcoes_condicoes.ts # Lógica condicional e funções básicas
│   │   └── pratica-async.ts     # Práticas de programação assíncrona (Async/Await)
│   └── index.ts           # Ponto de entrada da aplicação
├── tests/
│   └── login.test.ts      # Testes automatizados de login
├── utils/
│   └── helpers.ts         # Funções auxiliares e utilitários globais
├── package.json           # Dependências e scripts do projeto
├── tsconfig.json          # Configurações do compilador TypeScript
└── README.md              # Documentação do projeto

---

## 🛠️ Tecnologias Utilizadas

TypeScript — Superset JavaScript com tipagem estática.
Node.js — Ambiente de execução backend.
Frameworks/Bibliotecas de Testes e Automação configurados via package.json.

## ⚙️ Pré-requisitos

Certifique-se de ter instalado em sua máquina:
Node.js (Versão 18+ recomendada)
Gerenciador de pacotes npm

## 📥 Instalação e Configuração

1- Clone o repositório:

Bash
git clone [https://github.com/FabianoPaiva/automacaoTypeScript.git](https://github.com/FabianoPaiva/automacaoTypeScript.git)
Acesse a pasta do projeto:

2 - Acesse a pasta do projeto:

Bash
cd automacaoTypeScript

3 - Instale as dependências:

Bash
npm install

---

## 🚀 Como Executar os Testes e Scripts

Para rodar os scripts, verifique os comandos configurados no seu package.json. Geralmente, você pode executar os testes automatizados ou arquivos específicos utilizando o Node.js em conjunto com o TypeScript (ts-node):

1 - Executar testes:

Bash
npm test

(ou o comando específico configurado para rodar os arquivos em tests/ e src/**/*.test.ts)

2 - Executar módulos de nivelamento ou aulas:

Bash
npx ts-node src/nivelamento/pratica-async.ts

---

## 📄 Licença

Este projeto está sob a licença MIT.
Desenvolvido por Fabiano Paiva.
