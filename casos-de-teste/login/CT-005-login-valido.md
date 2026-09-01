## CT-005 — Login com credenciais válidas

**Requisito:** RF-007
**Funcionalidade:** Login
**Prioridade:** Alta
**Tipo:** Teste positivo

### Objetivo

Verificar se um usuário cadastrado consegue acessar sua conta utilizando credenciais válidas.

### Pré-condições

* Usuário previamente cadastrado;
* E-mail e senha conhecidos.

### Dados de teste

```text
E-mail: testebugbank@gmail.com
Senha: 123bug
```

### Passos

1. Acessar a página inicial.
2. Informar o e-mail cadastrado.
3. Informar a senha correta.
4. Clicar para acessar.

### Resultado esperado

O sistema deve autenticar o usuário e permitir o acesso à área da conta.

### Resultado obtido

O sistema autenticou o usuário com sucesso e permitiu o acesso à área da conta, conforme esperado.

### Status

✅ PASS

### Evidência

Não aplicável. Nenhuma evidência foi necessária para o resultado deste teste.
