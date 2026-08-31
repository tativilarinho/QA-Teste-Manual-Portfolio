## CT-010 — Validação de valores de transferência

**Requisito:** RF-013
**Funcionalidade:** Transferência
**Prioridade:** Alta
**Tipo:** Teste negativo / Validação

### Objetivo

Avaliar o comportamento da aplicação diante de diferentes valores informados para uma transferência.

### Cenários

| Cenário                 |         Valor |
| ----------------------- | ------------: |
| Campo vazio             |             — |
| Valor zero              |       R$ 0,00 |
| Valor negativo          |    -R$ 100,00 |
| Valor superior ao saldo | R$ 999.999,00 |
| Valor decimal           |      R$ 10,50 |
| Texto                   |           ABC |

### Pré-condições

* Usuário autenticado;
* Conta destinatária disponível;
* Saldo conhecido.

### Passos

1. Acessar a funcionalidade de transferência.
2. Informar uma conta destinatária válida.
3. Informar um dos valores definidos nos cenários.
4. Tentar concluir a operação.
5. Registrar o comportamento apresentado.
6. Repetir o teste para cada cenário.

### Resultado esperado

A aplicação deve validar os valores informados e impedir operações que não sejam aceitas pelas regras de negócio.

### Resultado obtido

A preencher após a execução.

### Status

⏳ A executar

### Evidência

A adicionar após a execução.
