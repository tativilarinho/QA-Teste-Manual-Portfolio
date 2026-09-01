## CT-007 — Login com campos vazios

**Requisito:** RF-012
**Funcionalidade:** Login
**Prioridade:** Alta
**Tipo:** Teste negativo

### Objetivo

Verificar se a aplicação realiza validação quando o usuário tenta acessar o sistema sem informar as credenciais.

### Dados de teste

```text
E-mail: vazio
Senha: vazio
```

### Passos

1. Acessar a tela de login.
2. Não preencher o e-mail.
3. Não preencher a senha.
4. Tentar realizar o login.

### Resultado esperado

O sistema deve impedir a tentativa de autenticação e apresentar as mensagens de validação correspondentes.

### Resultado obtido

O sistema impediu a tentativa de autenticação e apresentou a mensagem "É campo obrigatório" abaixo dos campos de e-mail e senha.

### Status

✅ PASS

### Evidência

Não aplicável. Nenhuma evidência foi necessária para o resultado deste teste.

