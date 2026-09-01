## CT-002 — Cadastro com campos obrigatórios vazios

**Requisito:** RF-012
**Funcionalidade:** Cadastro
**Prioridade:** Alta
**Tipo:** Teste negativo

### Objetivo

Verificar o comportamento da aplicação quando o usuário tenta realizar o cadastro sem preencher os campos necessários.

### Pré-condições

* Aplicação disponível;
* Tela de cadastro acessível.

### Dados de teste

Todos os campos permanecem vazios.

### Passos

1. Acessar a aplicação.
2. Acessar a tela de cadastro.
3. Não preencher os campos.
4. Tentar concluir o cadastro.

### Resultado esperado

O sistema deve impedir o cadastro e apresentar mensagens de validação adequadas para os campos obrigatórios.

### Resultado obtido

Ao tentar realizar o cadastro com os campos obrigatórios vazios, o sistema impediu a conclusão do cadastro e apresentou as validações esperadas para os campos obrigatórios.

### Status

✅ PASS

### Evidência

Não aplicável. Nenhuma evidência foi necessária para o resultado deste teste.

