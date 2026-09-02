# 🧪 QA / Teste Manual — BugBank

## 📌 Sobre o projeto

Este projeto apresenta a execução de testes manuais na aplicação web **BugBank**, com o objetivo de aplicar na prática conceitos de Quality Assurance (QA), testes funcionais, testes positivos e negativos, testes exploratórios e documentação de defeitos.

O projeto faz parte do meu portfólio profissional de **QA Manual**.

---

## 🎯 Objetivo

Validar as principais funcionalidades da aplicação, buscando identificar possíveis:

- Defeitos funcionais;
- Problemas de validação;
- Inconsistências de regras de negócio;
- Problemas de usabilidade;
- Comportamentos inesperados.

Além da execução dos testes, o projeto demonstra a aplicação prática de:

- Análise de requisitos;
- Elaboração de cenários e casos de teste;
- Definição de pré-condições e dados de teste;
- Execução de testes manuais;
- Registro de resultados;
- Identificação e documentação de defeitos;
- Classificação de severidade e prioridade;
- Organização de evidências;
- Rastreabilidade dos testes.

---

## 🌐 Aplicação testada

**BugBank**

https://bugbank.netlify.app/

A aplicação simula funcionalidades de um sistema bancário, incluindo cadastro, autenticação, conta, saldo e transferência.

---

## 🔎 Escopo dos testes

### Cadastro

- Cadastro de usuário;
- Validação de campos obrigatórios;
- Validação de e-mail;
- Confirmação de senha;
- Cadastro com dados válidos;
- Cadastro com dados inválidos;
- Comportamento com dados duplicados;
- Testes exploratórios de entrada de dados.

### Login

- Login com credenciais válidas;
- Login com senha inválida;
- Login com usuário inexistente;
- Campos obrigatórios;
- Mensagens de validação;
- Logout;
- Navegação utilizando teclado;
- Testes exploratórios de entrada de dados.

### Conta e saldo

- Criação de conta;
- Visualização de saldo;
- Persistência do saldo;
- Atualização da página;
- Navegação entre telas;
- Logout e nova autenticação;
- Validação das informações apresentadas.

### Transferências

- Transferência válida;
- Transferência para conta válida;
- Valores inválidos;
- Valor zero;
- Valor negativo;
- Valor superior ao saldo disponível;
- Campos obrigatórios;
- Validação das regras de negócio.

> Os cenários de transferência foram planejados, porém alguns permaneceram **BLOCKED** devido às limitações encontradas no ambiente de teste.

### Testes exploratórios

Foram realizadas sessões de testes exploratórios nas funcionalidades de:

- Cadastro;
- Login;
- Conta e saldo.

Os testes exploratórios tiveram como objetivo ampliar a cobertura além dos casos de teste previamente definidos e investigar comportamentos não contemplados inicialmente.

---

## 🧪 Tipos de testes

| Tipo | Aplicação |
|---|---|
| Teste funcional | ✅ |
| Teste positivo | ✅ |
| Teste negativo | ✅ |
| Teste exploratório | ✅ |
| Teste de validação | ✅ |
| Teste de regras de negócio | ✅ |
| Teste de usabilidade | ✅ |
| Teste de regressão | 🔄 |

---

## 🛠️ Ferramentas

- Firefox
- Git
- GitHub
- Markdown
- Ferramenta de captura de tela

---

## 📋 Documentação

| Documento | Descrição |
|---|---|
| [Matriz de Requisitos](requisitos.md) | Requisitos e funcionalidades avaliadas |
| [Casos de Teste](casos-de-teste.md) | Casos de teste manuais e resultados da execução |
| [Checklist](checklist.md) | Checklist de validação |
| [Bug Reports](bug-reports/) | Defeitos encontrados durante os testes |
| [Evidências](evidencias/) | Screenshots utilizados como evidência |
| [Testes Exploratórios](testes-exploratorios/) | Sessões de exploração realizadas |

---

## 📊 Resultado da Execução

Foram planejados **10 casos de teste**, dos quais **8 foram executados**.

| Métrica | Resultado |
|---|---:|
| Casos planejados | 10 |
| Casos executados | 8 |
| PASS | 8 |
| FAIL | 0 |
| BLOCKED | 2 |
| Bugs identificados | 2 |

### Distribuição dos resultados

- ✅ **80%** dos casos planejados foram executados;
- ✅ **100%** dos casos executados apresentaram resultado PASS;
- 🚫 **20%** permaneceram BLOCKED;
- 🐞 **2 defeitos** foram identificados durante o projeto.

---

## 🐞 Defeitos encontrados

Foram identificados dois defeitos durante a execução dos testes.

| ID | Origem | Descrição | Severidade | Status |
|---|---|---|---|---|
| [BUG-001](bug-reports/BUG-001.md) | CT-001 | Elementos da interface apresentados de forma visualmente invertida | Baixa | Aberto |
| [BUG-002](bug-reports/BUG-002.md) | TE-001 | Campo de nome permite texto excessivamente longo e ultrapassa os limites visuais | Baixa | Aberto |

Cada Bug Report contém informações como:

- ID;
- Título;
- Severidade;
- Prioridade;
- Ambiente;
- Pré-condições;
- Passos para reprodução;
- Resultado esperado;
- Resultado atual;
- Evidência;
- Status.

---

## 📸 Evidências

As evidências dos testes estão armazenadas na pasta [`evidencias`](evidencias/).

Elas permitem relacionar os resultados observados aos respectivos casos de teste e defeitos identificados.

---

## 🔗 Rastreabilidade

O projeto utiliza o seguinte fluxo de rastreabilidade:

**Requisito → Caso de Teste → Execução → Resultado → Bug Report**

Exemplo:

**RF-001 → CT-001 → PASS → BUG-001**

Um caso de teste pode apresentar resultado **PASS** e ainda assim gerar um Bug Report referente a um problema adicional identificado durante sua execução.

Isso ocorre porque o resultado do caso de teste está relacionado ao objetivo principal do cenário, enquanto um defeito adicional identificado durante a execução pode ser registrado separadamente.

---

## 🕵️ Testes Exploratórios

Além dos casos de teste estruturados, foram realizadas sessões de testes exploratórios.

| ID | Funcionalidade | Resultado |
|---|---|---|
| [TE-001](testes-exploratorios/TE-001-exploracao-cadastro.md) | Cadastro | 🐞 BUG-002 identificado |
| [TE-002](testes-exploratorios/TE-002-exploracao-login.md) | Login | Nenhum novo defeito confirmado |
| [TE-003](testes-exploratorios/TE-003-exploracao-conta-saldo.md) | Conta e saldo | Nenhum novo defeito confirmado |

Os testes exploratórios complementaram os casos estruturados e permitiram investigar diferentes entradas, comportamentos de navegação, persistência de dados e aspectos de usabilidade.

---

## ⚠️ Limitações do Ambiente de Teste

Durante a execução dos casos relacionados à transferência, foram identificadas limitações no ambiente disponível para validação completa dos cenários.

A aplicação utiliza armazenamento local no navegador, o que dificultou a manutenção e validação simultânea de diferentes contas durante os testes.

Por esse motivo, não foi possível confirmar de forma confiável todos os comportamentos necessários para concluir os cenários **CT-009** e **CT-010**.

Os dois casos foram classificados como **BLOCKED**, evitando classificar como defeito um comportamento que não pôde ser validado adequadamente.

---

## 📚 Aprendizados

Durante o desenvolvimento deste projeto foram praticados conceitos relacionados a:

- Quality Assurance;
- Testes manuais;
- Análise de requisitos;
- Técnicas de teste;
- Casos de teste;
- Testes positivos e negativos;
- Testes exploratórios;
- Regras de negócio;
- Bug Reporting;
- Severidade e prioridade;
- Evidências de teste;
- Rastreabilidade;
- Git e GitHub.

---

## 👩‍💻 Sobre mim

Sou uma profissional em desenvolvimento na área de **Quality Assurance**, construindo experiência prática em testes manuais, análise de requisitos, execução de testes e documentação de qualidade de software.

Este projeto demonstra minha capacidade de estruturar um ciclo de testes, desde a análise e planejamento até a execução, identificação de defeitos e documentação dos resultados.

---

## 📌 Status do projeto

**Concluído — QA Manual**

O projeto contempla planejamento, execução e documentação de testes manuais, incluindo casos de teste, testes exploratórios, evidências e Bug Reports.

Novas funcionalidades ou rodadas de teste poderão ser adicionadas futuramente conforme a evolução do projeto.
