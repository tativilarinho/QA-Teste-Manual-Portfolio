## CT-008 — Criação de conta com saldo

**Requisitos:** RF-006 / RF-009
**Funcionalidade:** Conta
**Prioridade:** Média
**Tipo:** Teste funcional

### Objetivo

Verificar o comportamento da aplicação ao criar uma conta utilizando a opção de criação com saldo.

### Pré-condições

* Aplicação disponível;
* E-mail ainda não utilizado.

### Dados de teste

| Campo                 | Valor                                     |
| --------------------- | ----------------------------------------- |
| Nome                  | QA Teste 08                               |
| E-mail                | testebugbank@gmail.com                    |
| Senha                 | 123bug                                    |
| Confirmação           | 123bug                                    |
| Criar conta com saldo | Selecionado                               |

### Passos

1. Acessar a tela de cadastro.
2. Informar os dados válidos.
3. Selecionar a opção de criação de conta com saldo.
4. Concluir o cadastro.
5. Realizar login com o usuário criado.
6. Verificar o saldo apresentado.

### Resultado esperado

A conta deve ser criada e, após o login, o sistema deve apresentar o saldo correspondente ao comportamento definido pela aplicação.

### Resultado obtido

Após a criação da conta com a opção de criação com saldo e realização do login, o sistema apresentou saldo de **R$ 1.000,00**, conforme o comportamento esperado.

### Status

✅ PASS

### Evidência

Não aplicável. Nenhuma evidência foi necessária para o resultado deste teste.
