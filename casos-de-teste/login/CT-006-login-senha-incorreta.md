## CT-006 — Login com senha incorreta

**Requisito:** RF-007
**Funcionalidade:** Login
**Prioridade:** Alta
**Tipo:** Teste negativo

### Objetivo

Verificar se o sistema impede o acesso quando a senha informada está incorreta.

### Pré-condições

* Usuário previamente cadastrado.

### Dados de teste

```text
E-mail: testebugbank@gmail.com
Senha: 123bank
```

### Passos

1. Acessar a página de login.
2. Informar um e-mail cadastrado.
3. Informar uma senha incorreta.
4. Tentar realizar o login.

### Resultado esperado

O sistema não deve autenticar o usuário e deve apresentar uma mensagem adequada informando que as credenciais não são válidas.

### Resultado obtido

O sistema não autenticou o usuário e apresentou o alerta: "Usuário ou senha inválido. Tente novamente ou verifique suas informações!"

### Status

✅ PASS

### Evidência

Não aplicável. Nenhuma evidência foi necessária para o resultado deste teste.
