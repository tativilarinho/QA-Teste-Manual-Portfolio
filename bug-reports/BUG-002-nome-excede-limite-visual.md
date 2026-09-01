# 🐞 BUG-002 — Campo de nome permite texto excessivamente longo e ultrapassa os limites visuais

## Resumo

O campo de nome permite a inserção de uma quantidade excessiva de caracteres. Ao utilizar um nome muito longo, o conteúdo ultrapassa visualmente os limites disponíveis da interface, comprometendo a apresentação das informações.

O comportamento também permanece após a conclusão do cadastro.

## Severidade

**Baixa**

## Prioridade

**Média**

## Tipo

**Interface / Usabilidade**

## Ambiente

- Aplicação: BugBank
- Plataforma: Desktop
- Navegador: Firefox
- Funcionalidade: Cadastro

## Pré-condições

- Acesso à tela de cadastro do BugBank.

## Passos para reprodução

1. Acessar a tela de cadastro.
2. Informar um nome contendo aproximadamente 100–200 caracteres.
3. Preencher os demais campos com dados válidos.
4. Observar o campo de nome durante o preenchimento.
5. Concluir o cadastro.
6. Acessar a conta criada.
7. Observar novamente a apresentação do nome.

## Resultado esperado

O sistema deve limitar a quantidade de caracteres permitida no campo de nome ou tratar adequadamente textos extensos, mantendo o conteúdo dentro dos limites visuais da interface.

## Resultado atual

O sistema permite a inserção de uma quantidade excessiva de caracteres. O nome ultrapassa visualmente os limites disponíveis da interface.

O comportamento também é mantido após a conclusão do cadastro.

Não é apresentada uma barra de rolagem horizontal para acomodar o conteúdo excedente.

## Impacto

O comportamento compromete a apresentação visual das informações e pode prejudicar a usabilidade e a leitura do nome do usuário.

## Evidência

A ser adicionada.

## Status

**Aberto**

## Origem

Teste exploratório — TE-001

## Caso de teste relacionado

Não identificado nos casos de teste estruturados.

## Observação

O defeito foi identificado durante uma sessão de teste exploratório, utilizando uma entrada com quantidade elevada de caracteres no campo de nome.
