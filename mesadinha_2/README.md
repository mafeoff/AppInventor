# Mesadinha — App de Controle Financeiro (MIT App Inventor + Firebase)

Projeto pessoal desenvolvido no **MIT App Inventor**, com persistência de dados em **Firebase Realtime Database**. O app funciona como uma "mesadinha digital": permite cadastro/login de usuário, registro de entradas e saídas de dinheiro, consulta de saldo por data e visualização de gastos em gráficos.

> Este repositório documenta a lógica do projeto através dos blocos (Blockly) do App Inventor, já que o `.aia` original foi criado e testado diretamente no editor online do MIT App Inventor antes de ser versionado aqui.

## Telas e funcionalidades

| # | Tela | O que faz |
|---|------|-----------|
| 1 | [Login e Cadastro](docs/01-tela-login-e-cadastro.png) | Permite criar uma conta (usuário/senha) ou entrar em uma já existente, usando o Firebase como banco de autenticação simples. Valida se os campos estão vazios, se o usuário já existe (no cadastro) ou se a senha confere (no login), e exibe alertas para cada caso. |
| 2 | [Menu principal e saldo](docs/02-menu-principal-e-saldo.png) | Tela inicial após o login. Busca o saldo atual no Firebase e o exibe na tela. A partir daqui o usuário navega para as telas de Entradas, Saídas, Consulta por Data, Gastos e Gráficos. |
| 3 | [Tela de Entradas](docs/03-tela-entradas.png) | Registra valores recebidos (mesada, presente, etc.), soma ao saldo atual e grava tanto o valor da entrada (associado à data) quanto o novo saldo no Firebase. |
| 4 | [Tela de Saídas](docs/04-tela-saidas.png) | Registra gastos por categoria (ex.: Alimentação, Transporte, Lazer). Verifica se há saldo suficiente antes de confirmar a saída; se não houver, avisa o usuário. Atualiza o saldo e grava o gasto por categoria no Firebase. |
| 5 | [Consulta por Data](docs/05-consulta-por-data.png) | Permite escolher uma data no seletor e consultar se houve depósito (entrada) registrado naquele dia, buscando o valor salvo no Firebase para aquela data específica. |
| 6 | [Gráficos de Gastos](docs/06-graficos-de-gastos.png) | Monta gráficos (pizza e colunas) com os gastos por categoria, usando o componente ChartMaker. Os dados vêm das saídas registradas no Firebase, agrupadas por categoria (Alimentação, Transporte, Lazer, Vestuário, Outros). |
| 7 | [Consulta de gasto por categoria](docs/07-consulta-gasto-por-categoria.png) | Ao selecionar uma categoria em uma lista, busca no Firebase o total gasto naquela categoria e exibe na tela (ou avisa que não há gastos registrados). |
| 8 | [Splash / Temporizador](docs/08-splash-temporizador.png) | Tela de abertura do app: um temporizador dispara e leva automaticamente o usuário para a tela de Login (Screen2) após alguns segundos. |

## Tecnologias utilizadas
- **MIT App Inventor** (programação em blocos)
- **Firebase Realtime Database** (armazenamento de usuários, saldo, entradas e saídas)
- **ChartMaker** (extensão para geração de gráficos de pizza e colunas)

## Sobre as datas deste repositório
Este projeto foi desenvolvido originalmente no editor do MIT App Inventor, na conta institucional do COTEMIG. Na pasta [`evidencia-desenvolvimento/`](evidencia-desenvolvimento/) há capturas de tela do editor com o relógio do sistema visível, confirmando que o projeto já estava em desenvolvimento em 03/10/2021 — antes da publicação deste repositório no GitHub.
