# 🧪 Casos de Teste — BugBank

## 1. Objetivo

Este documento apresenta a visão geral dos casos de teste elaborados para validar as principais funcionalidades da aplicação BugBank.

Os testes contemplam cenários positivos, negativos e de validação, buscando verificar tanto o comportamento esperado da aplicação quanto possíveis comportamentos inesperados.

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


| Status | Significado |
|---|---|
| ⏳ A executar | Caso ainda não executado |
| ✅ PASS | Resultado esperado confirmado |
| ❌ FAIL | Resultado diferente do esperado |
| 🚫 BLOCKED | Execução impedida por algum bloqueio |
| ➖ N/A | Caso não aplicável |

---

## 3. Resumo da Execução

Até o momento, foram executados 8 dos 10 casos de teste planejados.

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
- O CT-001 apresentou um problema visual durante a execução, que foi registrado separadamente como [BUG-001](bug-reports/BUG-001.md).
- Os casos CT-009 e CT-010 permaneceram bloqueados devido à limitação identificada durante a execução.
- Nenhum dos casos executados apresentou resultado funcional inesperado.

---

## 4. Critérios de Execução

Os casos de teste serão executados manualmente na aplicação BugBank.

Durante a execução serão registrados:

- Resultado obtido;
- Status do teste;
- Evidências;
- Observações;
- Possíveis defeitos identificados.

Quando um comportamento diferente do esperado for identificado, será realizada uma análise para determinar se o comportamento representa um defeito.

Defeitos confirmados serão documentados individualmente na pasta [`bug-reports`](bug-reports/).

---

## 5. Rastreabilidade

A execução seguirá o fluxo:

**Requisito → Caso de Teste → Execução → Resultado → Bug Report**

Exemplo:

**RF-001 → CT-001 → PASS → BUG-001**

Neste projeto, um caso de teste pode apresentar resultado **PASS** e ainda assim gerar um Bug Report referente a um problema adicional identificado durante sua execução.

---

## 6. Observações

Os resultados dos testes serão atualizados conforme a execução for realizada.

Os resultados apresentados neste documento devem representar o comportamento efetivamente observado na aplicação durante os testes.

---

## 7. Limitações do Ambiente de Teste

Durante a execução dos casos de teste, foram identificadas limitações funcionais da aplicação que impediram a execução de alguns cenários relacionados à transferência.

Os casos CT-009 e CT-010 foram classificados como **BLOCKED**, pois não foi possível estabelecer as condições necessárias para realizar uma transferência entre contas e validar os diferentes valores previstos.

Os casos permanecem documentados para demonstrar a cobertura planejada e poderão ser executados em um ambiente que disponibilize as condições necessárias.
