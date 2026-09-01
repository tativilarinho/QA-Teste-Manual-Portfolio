## CT-003 — Cadastro com senhas diferentes

**Requisito:** RF-005
**Funcionalidade:** Cadastro
**Prioridade:** Alta
**Tipo:** Teste negativo

### Objetivo

Verificar se o sistema identifica quando a senha e sua confirmação são diferentes.

### Pré-condições

* Aplicação disponível;
* Tela de cadastro acessível.

### Dados de teste

| Campo       | Valor                                     |
| ----------- | ----------------------------------------- |
| Nome        | QA Teste 01                               |
| E-mail      | testebugbank@gmail.com                    |
| Senha       | 123bug                                    |
| Confirmação | bug123                                    |

### Passos

1. Acessar a tela de cadastro.
2. Preencher o nome.
3. Informar um e-mail válido.
4. Informar a senha.
5. Informar uma senha de confirmação diferente.
6. Tentar concluir o cadastro.

### Resultado esperado

O sistema deve identificar a divergência entre as senhas e impedir a conclusão do cadastro.

### Resultado obtido

Ao tentar realizar o cadastro com senhas diferentes, o sistema identificou a divergência entre os campos de senha e confirmação de senha, impediu a conclusão do cadastro e apresentou o alerta: "As senhas não são iguais."

### Status

✅ PASS

### Evidência

Não aplicável. Nenhuma evidência foi necessária para o resultado deste teste.
