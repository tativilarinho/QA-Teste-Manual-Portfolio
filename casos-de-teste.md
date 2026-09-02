# 🧪 Casos de Teste — BugBank

## 1. Objetivo

Este documento apresenta a visão geral dos casos de teste elaborados para validar as principais funcionalidades da aplicação BugBank.

Os testes contemplam cenários positivos, negativos e de validação, buscando verificar o comportamento esperado da aplicação e identificar possíveis comportamentos inesperados.

Os detalhes de cada caso de teste estão organizados em arquivos individuais dentro da pasta [`casos-de-teste`](casos-de-teste/).

---

## 2. Resumo dos Casos de Teste

| ID | Requisito | Funcionalidade | Cenário | Prioridade | Status |
|---|---|---|---|---|---|
| [CT-001](casos-de-teste/cadastro/CT-001-cadastro-dados-validos.md) | RF-001 | Cadastro | Cadastro com dados válidos | Alta | ✅ PASS + 🐞 BUG-001 |
| [CT-002](casos-de-teste/cadastro/CT-002-cadastro-campos-vazios.md) | RF-012 | Cadastro | Cadastro com campos obrigatórios vazios | Alta | ✅ PASS |
| [CT-003](casos-de-teste/cadastro/CT-003-senhas-diferentes.md) | RF-005 | Cadastro | Cadastro com senhas diferentes | Alta | ✅ PASS |
| [CT-004](casos-de-teste/cadastro/CT-004-email-invalido.md) | RF-002/RF-013 | Cadastro | Cadastro com e-mail inválido | Alta | ✅ PASS |
| [CT-005](casos-de-teste/login/CT-005-login-valido.md) | RF-007 | Login | Login com credenciais válidas | Alta | ✅ PASS |
| [CT-006](casos-de-teste/login/CT-006-login-senha-incorreta.md) | RF-007 | Login | Login com senha incorreta | Alta | ✅ PASS |
| [CT-007](casos-de-teste/login/CT-007-login-campos-vazios.md) | RF-012 | Login | Login com campos vazios | Alta | ✅ PASS |
| [CT-008](casos-de-teste/conta/CT-008-conta-com-saldo.md) | RF-006/RF-009 | Conta | Criação de conta com saldo | Média | ✅ PASS |
| [CT-009](casos-de-teste/transferencia/CT-009-transferencia-valida.md) | RF-010/RF-009 | Transferência | Transferência com dados válidos | Alta | 🚫 BLOCKED |
| [CT-010](casos-de-teste/transferencia/CT-010-valores-transferencia.md) | RF-013 | Transferência | Validação de valores inválidos | Alta | 🚫 BLOCKED |

### Legenda de Status

| Status | Significado |
|---|---|
| ⏳ A executar | Caso ainda não executado |
| ✅ PASS | Resultado esperado confirmado |
| ❌ FAIL | Resultado diferente do esperado |
| 🚫 BLOCKED | Execução impedida por algum bloqueio |
| ➖ N/A | Caso não aplicável |

---

## 3. Resumo da Execução

Foram executados 8 dos 10 casos de teste planejados.

| Métrica | Resultado |
|---|---:|
| Casos planejados | 10 |
| Casos executados | 8 |
| PASS | 8 |
| FAIL | 0 |
| BLOCKED | 2 |
| Bugs identificados | 1 |

### Observações

- Os casos CT-001 a CT-008 foram executados com sucesso.
- O CT-001 apresentou um problema visual adicional durante sua execução, registrado separadamente como [BUG-001](bug-reports/BUG-001.md).
- O resultado funcional do CT-001 permaneceu como **PASS**, pois o comportamento principal do cadastro ocorreu conforme esperado.
- Os casos CT-009 e CT-010 permaneceram como **BLOCKED** devido às limitações encontradas no ambiente de teste para validação completa dos cenários de transferência.
- Nenhum dos casos executados apresentou falha funcional confirmada.

---

## 4. Critérios de Execução

Os casos de teste foram executados manualmente na aplicação BugBank.

Durante a execução foram registrados:

- Resultado obtido;
- Status do teste;
- Evidências;
- Observações;
- Possíveis defeitos identificados.

Quando um comportamento diferente do esperado foi identificado, foi realizada uma análise para determinar se o comportamento representava um defeito.

Defeitos confirmados foram documentados individualmente na pasta [`bug-reports`](bug-reports/).

---

## 5. Rastreabilidade

A execução seguiu o fluxo:

**Requisito → Caso de Teste → Execução → Resultado → Bug Report**

Exemplo:

**RF-001 → CT-001 → PASS → BUG-001**

Neste projeto, um caso de teste pode apresentar resultado **PASS** e ainda assim gerar um Bug Report referente a um problema adicional identificado durante sua execução.

Isso ocorre porque o resultado do caso de teste está relacionado ao objetivo principal do cenário, enquanto um defeito adicional identificado durante a execução pode ser registrado separadamente.

---

## 6. Testes Exploratórios

Além dos casos de teste estruturados, foram realizadas sessões de testes exploratórios nas funcionalidades de:

- Cadastro;
- Login;
- Conta e saldo.

Os testes exploratórios tiveram como objetivo ampliar a cobertura dos testes e investigar comportamentos que não estavam necessariamente contemplados nos casos de teste previamente definidos.

Documentação disponível em:

- [TE-001 — Exploração do Cadastro](testes-exploratorios/TE-001-exploracao-cadastro.md)
- [TE-002 — Exploração do Login](testes-exploratorios/TE-002-exploracao-login.md)
- [TE-003 — Exploração da Conta e Saldo](testes-exploratorios/TE-003-exploracao-conta-saldo.md)

Durante os testes exploratórios, foi confirmado um defeito relacionado ao tratamento de nomes excessivamente longos, documentado como [BUG-002](bug-reports/BUG-002.md).

---

## 7. Defeitos Identificados

| ID | Origem | Descrição | Severidade | Status |
|---|---|---|---|---|
| [BUG-001](bug-reports/BUG-001.md) | CT-001 | Elementos da interface apresentados de forma visualmente invertida | Baixa | Aberto |
| [BUG-002](bug-reports/BUG-002.md) | TE-001 | Campo de nome permite texto excessivamente longo e ultrapassa os limites visuais | Baixa | Aberto |

### Resumo dos defeitos

Foram identificados **2 defeitos** durante o projeto:

- **BUG-001:** identificado durante a execução do CT-001;
- **BUG-002:** identificado e confirmado durante o teste exploratório TE-001.

Os defeitos foram documentados separadamente para facilitar sua análise e rastreabilidade.

---

## 8. Limitações do Ambiente de Teste

Durante a execução dos casos relacionados à transferência, foram identificadas limitações no ambiente disponível para validação completa dos cenários.

A aplicação utiliza armazenamento local no navegador, o que dificultou a manutenção e validação simultânea de diferentes contas durante os testes.

Por esse motivo, não foi possível confirmar de forma confiável todos os comportamentos necessários para concluir os cenários CT-009 e CT-010.

Os casos foram classificados como **BLOCKED**, evitando classificar como defeito um comportamento que não pôde ser validado adequadamente.

Os cenários permanecem documentados e podem ser executados posteriormente em um ambiente que permita a validação completa das condições necessárias.

---

## 9. Conclusão

O projeto contemplou a elaboração e execução de casos de teste manuais para as principais funcionalidades do BugBank, incluindo:

- Cadastro;
- Login;
- Conta;
- Saldo;
- Validações;
- Transferência.

Foram executados **8 dos 10 casos de teste planejados**, com **8 resultados PASS**, nenhum FAIL e **2 casos BLOCKED** devido às limitações encontradas no ambiente de teste.

Também foram realizadas sessões de testes exploratórios, ampliando a cobertura das funcionalidades avaliadas e permitindo a identificação de comportamentos não contemplados inicialmente.

Ao final da execução, foram documentados **2 defeitos**, cada um com seu respectivo Bug Report e evidências.

O projeto demonstra a aplicação prática de conceitos de **QA Manual**, incluindo elaboração de requisitos, planejamento de testes, execução, registro de evidências, identificação e documentação de defeitos, testes exploratórios e rastreabilidade.
