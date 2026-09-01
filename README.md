# 🧪 QA Manual — BugBank

## 📌 Sobre o projeto

Este projeto apresenta a execução de testes manuais na aplicação web **BugBank**, com o objetivo de aplicar na prática conceitos de Quality Assurance (QA), testes funcionais, testes positivos e negativos, testes exploratórios e documentação de defeitos.

O projeto faz parte do meu portfólio profissional de **QA Manual**.

## 🎯 Objetivo

Validar as principais funcionalidades da aplicação, identificando possíveis defeitos funcionais, problemas de validação, inconsistências de regras de negócio e problemas de usabilidade.

Além da execução dos testes, o projeto demonstra a capacidade de:

* Analisar requisitos;
* Elaborar cenários e casos de teste;
* Definir pré-condições e dados de teste;
* Executar testes manuais;
* Registrar resultados;
* Identificar e documentar defeitos;
* Classificar severidade e prioridade;
* Organizar evidências;
* Elaborar relatório de testes.

## 🌐 Aplicação testada

**BugBank**

URL: https://bugbank.netlify.app/

A aplicação simula funcionalidades de um sistema bancário, permitindo a realização de atividades como cadastro, autenticação e operações financeiras.

## 🔎 Escopo dos testes

### Cadastro

* Cadastro de usuário;
* Validação de campos obrigatórios;
* Validação de e-mail;
* Confirmação de senha;
* Cadastro com dados válidos;
* Cadastro com dados inválidos;
* Comportamento com dados duplicados.

### Login

* Login com credenciais válidas;
* Login com senha inválida;
* Login com usuário inexistente;
* Campos obrigatórios;
* Mensagens de validação;
* Logout.

### Conta e saldo

* Criação de conta;
* Visualização de saldo;
* Comportamento do saldo após operações;
* Validação das informações apresentadas.

### Transferências

* Transferência válida;
* Transferência para conta válida;
* Valores inválidos;
* Valor zero;
* Valor negativo;
* Valor superior ao saldo disponível;
* Campos obrigatórios;
* Validação das regras de negócio.

### Testes exploratórios

Também serão realizados testes exploratórios com o objetivo de identificar comportamentos inesperados que possam não estar contemplados nos casos de teste previamente definidos.

## 🧪 Tipos de testes

| Tipo                       | Aplicação |
| -------------------------- | --------- |
| Teste funcional            | ✅         |
| Teste positivo             | ✅         |
| Teste negativo             | ✅         |
| Teste exploratório         | ✅         |
| Teste de validação         | ✅         |
| Teste de regras de negócio | ✅         |
| Teste de usabilidade       | ✅         |
| Teste de regressão         | 🔄        |

## 🛠️ Ferramentas

* Firefox
* Git
* GitHub
* Markdown
* Ferramenta de captura de tela

## 📋 Documentação

| Documento                             | Descrição                              |
| ------------------------------------- | -------------------------------------- |
| [Matriz de Requisitos](requisitos.md) | Requisitos e funcionalidades avaliadas |
| [Casos de Teste](casos-de-teste.md)   | Casos de teste manuais                 |
| [Checklist](checklist.md)             | Checklist de validação                 |
| Bug Reports                           | Defeitos encontrados durante os testes |
| Evidências                            | Screenshots e demais evidências        |

## 📊 Status da execução

> Os resultados serão atualizados conforme os testes forem executados.

| Métrica | Resultado |
|---|---:|
| Casos planejados | 10 |
| Casos executados | 8 |
| PASS | 8 |
| FAIL | 0 |
| BLOCKED | 2 |
| Bugs identificados | 1 |

## 🐞 Defeitos encontrados

Os defeitos identificados durante a execução serão documentados individualmente na pasta [`bug-reports`](bug-reports/).

Cada Bug Report conterá:

* ID;
* Título;
* Severidade;
* Prioridade;
* Ambiente;
* Pré-condições;
* Passos para reprodução;
* Resultado esperado;
* Resultado atual;
* Evidência;
* Status.

## 📸 Evidências

As evidências dos testes serão armazenadas na pasta [`evidencias`](evidencias/), permitindo relacionar os resultados dos testes aos respectivos casos de teste e defeitos encontrados.

## 🔗 Rastreabilidade

Os casos de teste serão relacionados aos requisitos correspondentes, permitindo acompanhar o fluxo:

**Requisito → Caso de Teste → Execução → Resultado → Bug Report**

## 📚 Aprendizados

Durante este projeto serão praticados conceitos relacionados a:

* Quality Assurance;
* Testes manuais;
* Análise de requisitos;
* Técnicas de teste;
* Casos de teste;
* Testes positivos e negativos;
* Testes exploratórios;
* Regras de negócio;
* Bug Reporting;
* Severidade e prioridade;
* Evidências de teste;
* Rastreabilidade;
* Git e GitHub.

## 👩‍💻 Sobre mim

Sou uma profissional em desenvolvimento na área de **Quality Assurance**, construindo experiência prática em testes manuais e documentação de qualidade de software.

Este repositório demonstra minha abordagem prática para planejamento, execução, análise e documentação de testes.

---

### 📌 Projeto em desenvolvimento

Este projeto será atualizado continuamente conforme novas rodadas de testes forem executadas e novos resultados forem identificados.
