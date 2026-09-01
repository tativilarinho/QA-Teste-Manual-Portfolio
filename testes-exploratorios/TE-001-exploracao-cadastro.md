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

## Defeitos identificados

### BUG-002 — Campo de nome permite texto excessivamente longo

Durante a exploração do campo de nome, foi identificado que a aplicação permite a inserção de aproximadamente 100–200 caracteres.

O conteúdo ultrapassou visualmente os limites disponíveis da interface, sem apresentação de uma barra de rolagem horizontal.

O comportamento também foi observado após a conclusão do cadastro.

O defeito foi documentado separadamente em [BUG-002](../bug-reports/BUG-002-nome-excede-limite-visual.md).

## Conclusão

A sessão exploratória permitiu identificar um defeito relacionado ao tratamento de entradas excessivamente longas no campo de nome.

Além do defeito identificado, foram avaliados diferentes comportamentos relacionados à validação, navegação e preenchimento do formulário de cadastro.
