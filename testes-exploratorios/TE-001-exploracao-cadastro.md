## Cenários explorados

| # | Cenário | Resultado |
|---|---|---|
| 1 | Espaços antes e depois do nome | Sistema aceitou os espaços |
| 2 | Nome com aproximadamente 100–200 caracteres | Sistema aceitou o texto e o conteúdo ultrapassou visualmente a área disponível |
| 3 | E-mail utilizando letras maiúsculas | Sistema aceitou normalmente |
| 4 | Nome contendo números | Sistema aceitou |
| 5 | Nome utilizando formato de e-mail | Sistema aceitou |
| 6 | Senha igual ao e-mail utilizado no cadastro | Sistema aceitou |
| 7 | Navegação entre cadastro e login após preenchimento parcial | Dados permaneceram preenchidos |
| 8 | Atualização da página durante o preenchimento | Sistema retornou à página inicial e os dados foram perdidos |

## Observações

Durante a exploração foram identificados alguns comportamentos que merecem análise adicional, principalmente relacionados à validação dos campos de cadastro e ao comportamento visual do campo de nome quando preenchido com uma quantidade elevada de caracteres.

Os comportamentos observados não foram classificados automaticamente como defeitos, sendo necessária a análise dos requisitos e/ou confirmação do comportamento esperado da aplicação.
