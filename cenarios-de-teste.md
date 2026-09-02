# 🧪 Cenários de Teste - BugBank

## 1. Objetivo

Este documento apresenta os cenários de teste definidos para a aplicação **BugBank**, elaborados a partir dos requisitos funcionais identificados durante a análise da aplicação.

Os cenários representam situações de negócio que devem ser validadas por meio dos casos de teste detalhados no documento [`casos-de-teste.md`](casos-de-teste.md).

O objetivo é garantir a rastreabilidade entre:

**Requisito → Cenário de Teste → Caso de Teste → Execução → Resultado**

---

## 2. Escopo

Os cenários contemplam as principais funcionalidades avaliadas no projeto:

- Cadastro;
- Login;
- Conta e saldo;
- Transferência;
- Validações de entrada.

---

## 3. Cenários de Teste

### 📌 Cadastro

| ID | Requisito | Cenário | Caso de Teste | Prioridade |
|---|---|---|---|---|
| CTN-001 | RF-001 | Validar o cadastro de um novo usuário utilizando dados válidos | [CT-001](casos-de-teste/cadastro/CT-001-cadastro-dados-validos.md) | Alta |
| CTN-002 | RF-012 | Validar o comportamento do cadastro quando os campos obrigatórios não são preenchidos | [CT-002](casos-de-teste/cadastro/CT-002-cadastro-campos-vazios.md) | Alta |
| CTN-003 | RF-005 | Validar o cadastro quando a confirmação de senha é diferente da senha informada | [CT-003](casos-de-teste/cadastro/CT-003-senhas-diferentes.md) | Alta |
| CTN-004 | RF-002/RF-013 | Validar o cadastro utilizando um endereço de e-mail em formato inválido | [CT-004](casos-de-teste/cadastro/CT-004-email-invalido.md) | Alta |

---

### 🔐 Login

| ID | Requisito | Cenário | Caso de Teste | Prioridade |
|---|---|---|---|---|
| CTN-005 | RF-007 | Validar a autenticação utilizando credenciais válidas | [CT-005](casos-de-teste/login/CT-005-login-valido.md) | Alta |
| CTN-006 | RF-007 | Validar o comportamento do sistema quando uma senha incorreta é informada | [CT-006](casos-de-teste/login/CT-006-login-senha-incorreta.md) | Alta |
| CTN-007 | RF-012 | Validar o comportamento do login quando os campos obrigatórios estão vazios | [CT-007](casos-de-teste/login/CT-007-login-campos-vazios.md) | Alta |

---

### 💰 Conta e Saldo

| ID | Requisito | Cenário | Caso de Teste | Prioridade |
|---|---|---|---|---|
| CTN-008 | RF-006/RF-009 | Validar a criação de uma conta com saldo inicial | [CT-008](casos-de-teste/conta/CT-008-conta-com-saldo.md) | Média |

---

### 💸 Transferência

| ID | Requisito | Cenário | Caso de Teste | Prioridade |
|---|---|---|---|---|
| CTN-009 | RF-010/RF-009 | Validar a realização de uma transferência utilizando dados válidos | [CT-009](casos-de-teste/transferencia/CT-009-transferencia-valida.md) | Alta |
| CTN-010 | RF-013 | Validar o comportamento do sistema diante de valores inválidos ou condições não permitidas para transferência | [CT-010](casos-de-teste/transferencia/CT-010-valores-transferencia.md) | Alta |

---

## 4. Matriz de Rastreabilidade

A tabela abaixo relaciona cada requisito aos respectivos cenários e casos de teste.

| Requisito | Cenário | Caso de Teste | Status |
|---|---|---|---|
| RF-001 | CTN-001 | CT-001 | ✅ PASS |
| RF-012 | CTN-002 | CT-002 | ✅ PASS |
| RF-005 | CTN-003 | CT-003 | ✅ PASS |
| RF-002/RF-013 | CTN-004 | CT-004 | ✅ PASS |
| RF-007 | CTN-005 | CT-005 | ✅ PASS |
| RF-007 | CTN-006 | CT-006 | ✅ PASS |
| RF-012 | CTN-007 | CT-007 | ✅ PASS |
| RF-006/RF-009 | CTN-008 | CT-008 | ✅ PASS |
| RF-010/RF-009 | CTN-009 | CT-009 | 🚫 BLOCKED |
| RF-013 | CTN-010 | CT-010 | 🚫 BLOCKED |

---

## 5. Resumo

Foram definidos **10 cenários de teste**, correspondentes aos 10 casos de teste planejados para o projeto.

| Categoria | Cenários |
|---|---:|
| Cadastro | 4 |
| Login | 3 |
| Conta e Saldo | 1 |
| Transferência | 2 |
| **Total** | **10** |

Dos 10 cenários definidos:

- **8** foram executados com sucesso;
- **2** permaneceram bloqueados;
- Nenhum cenário executado apresentou falha funcional;
- Os defeitos identificados durante as execuções foram registrados separadamente em [`bug-reports`](bug-reports/).

---

## 6. Observações

Os cenários de transferência permaneceram classificados como **BLOCKED**, pois não foi possível estabelecer de forma confiável as condições necessárias para validar uma transferência entre contas no ambiente utilizado.

Essa limitação está relacionada às condições de execução da aplicação e não foi considerada, isoladamente, um defeito funcional.

Os testes exploratórios realizados no projeto são documentados separadamente na pasta [`testes-exploratorios`](testes-exploratorios/).

---

## 7. Relação com os Casos de Teste

Os cenários apresentados neste documento representam o nível de planejamento funcional.

Os detalhes de execução, incluindo:

- pré-condições;
- dados de teste;
- passos;
- resultado esperado;
- resultado obtido;
- status;
- evidências;

estão documentados individualmente nos respectivos arquivos da pasta [`casos-de-teste`](casos-de-teste/).

---

## 8. Fluxo de Rastreabilidade

```text
REQUISITO
    ↓
CENÁRIO DE TESTE
    ↓
CASO DE TESTE
    ↓
EXECUÇÃO
    ↓
RESULTADO
    ↓
BUG REPORT (quando aplicável)
