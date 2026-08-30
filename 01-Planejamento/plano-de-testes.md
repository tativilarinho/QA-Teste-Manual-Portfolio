# Plano de Testes — BugBank

## 1. Objetivo

Este projeto tem como objetivo realizar testes manuais na aplicação BugBank, avaliando suas principais funcionalidades e identificando possíveis defeitos funcionais, problemas de validação, inconsistências de regras de negócio e problemas relacionados à experiência do usuário.

## 2. Aplicação

BugBank — aplicação web desenvolvida para prática de testes de software.

URL: https://bugbank.netlify.app/

## 3. Escopo

Serão avaliadas as seguintes funcionalidades:

* Cadastro de usuário
* Login
* Logout
* Visualização de saldo
* Transferências
* Operações financeiras
* Validação de campos
* Regras de negócio
* Mensagens apresentadas ao usuário
* Usabilidade
* Comportamento da aplicação diante de entradas inválidas

## 4. Tipos de testes

Serão utilizados:

* Testes funcionais
* Testes positivos
* Testes negativos
* Testes exploratórios
* Testes de regressão
* Testes de validação
* Testes de usabilidade
* Testes de regras de negócio

## 5. Critérios de sucesso

Uma funcionalidade será considerada aprovada quando:

* O comportamento observado estiver de acordo com o comportamento esperado;
* Os dados informados forem processados corretamente;
* Mensagens de erro forem apresentadas adequadamente;
* A aplicação impedir operações inválidas;
* Não forem observados comportamentos inesperados que comprometam a funcionalidade.

## 6. Ambiente

Navegador: Firefox
Sistema operacional: Windows
Tipo de aplicação: Web
Ambiente: BugBank

## 7. Riscos e limitações

A aplicação informa que utiliza armazenamento em memória local e não possui banco de dados persistente. Assim, alguns comportamentos relacionados à persistência dos dados podem depender do ambiente utilizado durante os testes.

## 8. Evidências

Os testes serão acompanhados de evidências, como:

* Screenshots
* Mensagens apresentadas pela aplicação
* Dados utilizados nos testes
* Resultado observado

## 9. Resultado esperado

Ao final da execução, será produzido um relatório contendo:

* Quantidade de casos de teste executados;
* Casos aprovados;
* Casos reprovados;
* Bugs encontrados;
* Severidade dos defeitos;
* Evidências;
* Conclusão sobre a qualidade da aplicação.
