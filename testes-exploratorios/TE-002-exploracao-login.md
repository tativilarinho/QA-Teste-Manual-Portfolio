## Cenários explorados

| # | Cenário | Resultado |
|---|---|---|
| 1 | E-mail com espaço antes ou depois | O sistema não permitiu a autenticação e apresentou mensagem de credenciais inválidas |
| 2 | E-mail utilizando letras maiúsculas | O sistema não permitiu a autenticação e apresentou mensagem de credenciais inválidas |
| 3 | E-mail extremamente longo | O campo aceitou o conteúdo, sem apresentar limite ou mensagem de validação |
| 4 | Senha extremamente longa | O campo aceitou o conteúdo, sem apresentar limite ou mensagem de validação |
| 5 | Copiar e colar senha | O comportamento foi igual ao da digitação manual |
| 6 | Mostrar/ocultar senha | O comportamento ocorreu conforme esperado |
| 7 | Navegação utilizando teclado | O foco passou pelo controle de visualização da senha antes de prosseguir para os demais elementos |
| 8 | Clique repetido no botão Entrar | A aplicação navegou rapidamente para a tela inicial, não sendo possível realizar múltiplos cliques |

## Observações

Durante a sessão exploratória foram observados comportamentos relacionados ao tratamento de entradas extensas e à autenticação utilizando diferentes formatos de e-mail.

Também foi avaliada a navegação utilizando o teclado, sendo observado que o controle de visualização da senha recebe foco antes dos demais elementos interativos.

Esses comportamentos foram registrados como observações e não foram classificados automaticamente como defeitos sem uma definição clara do comportamento esperado.

## Defeitos identificados

Nenhum novo defeito foi confirmado durante a sessão exploratória.

## Conclusão

A sessão exploratória avaliou diferentes comportamentos da funcionalidade de login, incluindo validação de entradas, tratamento de dados extensos, interação com o campo de senha e navegação utilizando teclado.

Nenhum novo defeito foi confirmado durante a sessão.
