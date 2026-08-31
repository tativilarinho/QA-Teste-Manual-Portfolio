## CT-001 — Cadastro com dados válidos

**Requisito:** RF-001
**Funcionalidade:** Cadastro
**Prioridade:** Alta
**Tipo:** Teste positivo

### Objetivo

Validar se um novo usuário consegue realizar o cadastro utilizando dados válidos.

### Pré-condições

* Aplicação disponível;
* Usuário ainda não cadastrado;
* E-mail disponível para utilização no teste.

### Dados de teste

| Campo       | Valor                                     |
| ----------- | ----------------------------------------- |
| Nome        | QA Teste 01                               |
| E-mail      | testebugbank@gmail.com                    |
| Senha       | 123bug                                    |
| Confirmação | 123bug                                    |

### Passos

1. Acessar a aplicação BugBank.
2. Acessar a opção de registrar.
3. Informar o nome.
4. Informar um e-mail válido.
5. Informar uma senha.
6. Confirmar a senha.
7. Concluir o cadastro.

### Resultado esperado

O sistema deve aceitar os dados informados e concluir o processo de cadastro, apresentando ao usuário a resposta correspondente.

### Resultado obtido

O cadastro foi realizado com sucesso. Mas, foi identificado que alguns textos e elementos da interface estavam apresentados de forma invertida/espelhada visualmente.

### Status

✅ PASS

### Observação

Embora o fluxo funcional de cadastro tenha sido concluído com sucesso, foi identificado um defeito visual durante a execução. O problema foi registrado separadamente como BUG-001.

### Evidência

![Evidência do teste](../evidencias/CT-001.png)
