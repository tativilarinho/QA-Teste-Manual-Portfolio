## CT-004 — Cadastro com e-mail inválido

**Requisitos:** RF-002 / RF-013
**Funcionalidade:** Cadastro
**Prioridade:** Alta
**Tipo:** Teste negativo

### Objetivo

Verificar se a aplicação valida corretamente o formato do endereço de e-mail.

### Dados de teste

Serão utilizados formatos inválidos, como:

```text
teste@
teste.com
testebugbank@@gmail.com
```

### Passos

1. Acessar a tela de cadastro.
2. Informar um nome válido.
3. Informar um e-mail inválido.
4. Preencher os demais campos corretamente.
5. Tentar concluir o cadastro.
6. Repetir o teste utilizando os diferentes formatos de e-mail.

### Resultado esperado

O sistema deve validar o formato do e-mail e impedir o cadastro quando o endereço informado for considerado inválido.

### Resultado obtido

A preencher após a execução.

### Status

⏳ A executar

### Evidência

A adicionar após a execução.
