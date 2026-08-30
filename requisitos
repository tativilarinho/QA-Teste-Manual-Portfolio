# 📋 Matriz de Requisitos — BugBank

## 1. Objetivo

Esta matriz apresenta as principais funcionalidades identificadas na aplicação BugBank que serão consideradas no escopo dos testes manuais.

Os requisitos foram levantados a partir da análise da aplicação e serão validados durante a execução dos testes.

> **Observação:** quando o comportamento esperado não estiver explicitamente definido pela aplicação, ele será tratado como um cenário a ser validado durante os testes, evitando assumir regras de negócio sem evidência.

---

## 2. Requisitos Funcionais

| ID     | Funcionalidade | Requisito                                                                                                               | Prioridade | Caso de Teste        | Status    |
| ------ | -------------- | ----------------------------------------------------------------------------------------------------------------------- | ---------- | -------------------- | --------- |
| RF-001 | Cadastro       | O sistema deve permitir o cadastro de um novo usuário.                                                                  | Alta       | CT-001               | A validar |
| RF-002 | Cadastro       | O sistema deve solicitar um e-mail para realização do cadastro.                                                         | Alta       | CT-001, CT-004       | A validar |
| RF-003 | Cadastro       | O sistema deve solicitar o nome do usuário.                                                                             | Alta       | CT-001               | A validar |
| RF-004 | Cadastro       | O sistema deve solicitar uma senha.                                                                                     | Alta       | CT-001               | A validar |
| RF-005 | Cadastro       | O sistema deve solicitar a confirmação da senha.                                                                        | Alta       | CT-003               | A validar |
| RF-006 | Cadastro       | O sistema deve disponibilizar a opção de criação de conta com saldo.                                                    | Média      | CT-008               | A validar |
| RF-007 | Login          | O sistema deve permitir a autenticação utilizando e-mail e senha.                                                       | Alta       | CT-005, CT-006       | A validar |
| RF-008 | Conta          | O usuário autenticado deve conseguir acessar sua conta.                                                                 | Alta       | CT-005               | A validar |
| RF-009 | Saldo          | O sistema deve apresentar as informações relacionadas ao saldo da conta.                                                | Alta       | CT-008, CT-009       | A validar |
| RF-010 | Transferência  | O sistema deve permitir a realização de transferências.                                                                 | Alta       | CT-009               | A validar |
| RF-011 | Pagamento      | O sistema deve disponibilizar funcionalidade relacionada a pagamentos.                                                  | Alta       | A definir            | A validar |
| RF-012 | Validação      | O sistema deve validar o preenchimento dos campos obrigatórios.                                                         | Alta       | CT-002, CT-007       | A validar |
| RF-013 | Validação      | O sistema deve tratar entradas inválidas fornecidas pelo usuário.                                                       | Alta       | CT-004, CT-010       | A validar |
| RF-014 | Usabilidade    | Os campos e controles da aplicação devem apresentar comportamento compreensível ao usuário.                             | Média      | Testes exploratórios | A validar |
| RF-015 | Persistência   | O comportamento dos dados deve ser avaliado considerando as características de armazenamento informadas pela aplicação. | Média      | Testes exploratórios | A validar |

---

## 3. Classificação de prioridade

### 🔴 Alta

Funcionalidades que impactam diretamente o funcionamento principal da aplicação ou operações financeiras.

Exemplos:

* Cadastro;
* Login;
* Saldo;
* Transferência;
* Validação de dados.

### 🟡 Média

Funcionalidades importantes, mas cujo impacto sobre o fluxo principal é menor.

Exemplos:

* Usabilidade;
* Comportamentos complementares;
* Persistência.

### 🟢 Baixa

Itens cujo impacto é pequeno e que podem ser avaliados posteriormente.

---

## 4. Rastreabilidade

A rastreabilidade será utilizada para relacionar os requisitos aos respectivos casos de teste.

O fluxo utilizado será:

```text
Requisito
    ↓
Caso de Teste
    ↓
Execução
    ↓
Resultado
    ↓
Bug Report
```

### Exemplo

```text
RF-010
  ↓
CT-009
  ↓
Resultado da execução
  ↓
PASS ou FAIL
  ↓
BUG-XXX, caso seja identificado um defeito
```

---

## 5. Critérios de status

| Status        | Significado                                         |
| ------------- | --------------------------------------------------- |
| A validar     | Requisito ainda não foi validado durante a execução |
| Validado      | Comportamento esperado foi confirmado               |
| Não atendido  | Comportamento observado não atende ao esperado      |
| Bloqueado     | Não foi possível realizar a validação               |
| Não aplicável | Item não se aplica ao cenário avaliado              |

---

## 6. Observações

Esta matriz será atualizada conforme os casos de teste forem executados.

Os resultados apresentados no projeto devem representar o comportamento efetivamente observado durante os testes, sem assumir previamente a existência de defeitos.

A identificação de um possível defeito deverá ser acompanhada de evidências e documentada em um Bug Report específico.
