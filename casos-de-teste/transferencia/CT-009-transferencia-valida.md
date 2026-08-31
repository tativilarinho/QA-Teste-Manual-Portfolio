## CT-009 — Transferência com dados válidos

**Requisitos:** RF-010 / RF-009
**Funcionalidade:** Transferência
**Prioridade:** Alta
**Tipo:** Teste positivo

### Objetivo

Verificar se uma transferência pode ser realizada utilizando dados válidos.

### Pré-condições

* Usuário remetente cadastrado;
* Usuário destinatário cadastrado;
* Usuário remetente autenticado;
* Saldo suficiente para realizar a operação.

### Dados de teste

```text
Remetente: QA Teste 01
Destinatário: QA Teste 02
Valor: R$ 100,00
```

### Passos

1. Realizar login com o usuário remetente.
2. Acessar a funcionalidade de transferência.
3. Informar os dados do destinatário.
4. Informar o valor de R$ 100,00.
5. Confirmar a operação.
6. Verificar o saldo do remetente.
7. Acessar a conta do destinatário.
8. Verificar o saldo do destinatário.

### Resultado esperado

A transferência deve ser processada conforme as regras da aplicação e os saldos envolvidos devem ser atualizados corretamente.

### Resultado obtido

A preencher após a execução.

### Status

⏳ A executar

### Evidência

A adicionar após a execução.
