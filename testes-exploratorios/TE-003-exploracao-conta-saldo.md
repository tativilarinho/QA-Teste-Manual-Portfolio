## Cenários explorados

| # | Cenário | Resultado |
|---|---|---|
| 1 | Logout e novo login | O saldo permaneceu igual após realizar um novo login |
| 2 | Atualização da página | O saldo permaneceu igual após atualizar a página |
| 3 | Navegação entre telas | O saldo permaneceu consistente ao retornar à tela da conta |
| 4 | Exibição do saldo | O saldo apresentou `R$`, duas casas decimais, alinhamento adequado e não apresentou cortes ou sobreposição. O valor exibido no extrato também foi consistente |
| 5 | Conta com saldo zero | Não foi possível realizar o teste devido à ausência de funcionalidades suficientes para levar a conta a saldo zero |
| 6 | Dados da conta | Foram exibidos número da conta, nome do usuário e saldo. O e-mail não foi apresentado |
| 7 | Logout e botão voltar do navegador | Após o logout, o sistema não permitiu retornar à área autenticada pelo botão voltar e exigiu nova autenticação |

## Observações

Durante a exploração da funcionalidade de conta e saldo, não foram identificadas inconsistências na manutenção ou apresentação do saldo.

O saldo permaneceu consistente após logout e novo login, atualização da página e navegação entre funcionalidades.

Também foi verificado que, após o logout, a aplicação não permitiu o acesso à área autenticada utilizando o botão voltar do navegador, exigindo nova autenticação.

Não foi possível testar o comportamento de uma conta com saldo zero devido às funcionalidades disponíveis no ambiente.

## Defeitos identificados

Nenhum novo defeito foi confirmado durante a sessão exploratória.

## Conclusão

A sessão exploratória avaliou a persistência do saldo, atualização da página, navegação entre funcionalidades, apresentação das informações da conta e comportamento da sessão após o logout.

Os comportamentos observados foram consistentes com o funcionamento esperado da aplicação nos cenários avaliados.

Nenhum novo defeito foi confirmado durante a sessão exploratória.
