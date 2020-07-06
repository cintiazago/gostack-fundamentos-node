<img alt="GoStack" src="https://storage.googleapis.com/golden-wind/bootcamp-gostack/header-desafios.png" />

<p align="center">

<img alt="License" src="https://img.shields.io/badge/license-MIT-brightgreen?color=blue">

<a target="_blank" href="https://nodejs.org/">
    <img alt="ReactNative" src="https://img.shields.io/static/v1?color=brightgreen&label=Node&message=JS&?style=plastic&logo=Node.js">
  </a>

</p>

<h2 align="center">
  Desafio 05: Primeiro projeto Node.js
</h2>

<h3 align="center">
  “Para quem fica melhor a cada dia, ficar pronto é utopia”!
</h3>

## 🚀 Sobre o desafio

Nesse desafio, foi criada uma aplicação para treinar o que aprendemos até agora com Node.js, juntamente com TypeScript, utilizando o conceito de models, repositories e services!

Esta será uma aplicação para armazenar transações financeiras de entrada e saída, devendo permitir o cadastro e a listagem destas transações.


## 🔨 Tecnologias:

- [NodeJs][nodejs]
- [Express][express]
- [Typescript][typescript]
- [uuidv4][uuidv4]


## 🚀 Como rodar este projeto

Para clonar e executar este aplicativo, você precisará de [Git](https://git-scm.com), [NodeJs][nodejs] Instalado em seu computador.

### 🌀 Clonando o repositório

```bash
# Clone este repositório
$ git clone https://github.com/cintiazago/gostack-fundamentos-node

# Acesse a pasta do projeto no terminal/cmd
$ cd gostack-fundamentos-node
```

### 🎲 Rodando a API

```bash
# Instale as dependências
$ yarn

# Execute a Aplicação
$ yarn dev:server

# Execute o teste da Aplicação
$ yarn test

# O servidor inciará na porta:3333 - acesse http://localhost:3333
```

## 🔑 Rotas da aplicação

- **`POST /transactions`**: A rota deve receber `title`, `value` e `type` dentro do corpo da requisição, sendo `type` o tipo da transação, que deve ser `income` para entradas (depósitos) e `outcome` para saídas (retiradas). Ao cadastrar uma nova transação, ela deve ser armazenada dentro de um objeto com o seguinte formato :

```json
{
  "id": "uuid",
  "title": "Salário",
  "value": 3000,
  "type": "income"
}
```

- **`GET /transactions`**: Essa rota deve retornar uma listagem com todas as transações que você cadastrou até agora, junto com o valor de soma de entradas, retiradas e total de crédito. Essa rota deve retornar um objeto com o formato a seguir:

```json
{
  "transactions": [
    {
      "id": "uuid",
      "title": "Salário",
      "value": 4000,
      "type": "income"
    },
    {
      "id": "uuid",
      "title": "Freela",
      "value": 2000,
      "type": "income"
    },
    {
      "id": "uuid",
      "title": "Pagamento da fatura",
      "value": 4000,
      "type": "outcome"
    },
    {
      "id": "uuid",
      "title": "Cadeira Gamer",
      "value": 1200,
      "type": "outcome"
    }
  ],
  "balance": {
    "income": 6000,
    "outcome": 5200,
    "total": 800
  }
}
```

## 🤔 Como contribuir para o projeto

- Faça um **fork** do projeto;
- Crie uma nova branch com as suas alterações: `git checkout -b my-feature`
- Salve as alterações e crie uma mensagem de commit contando o que você fez:`git commit -m "feature: My new feature"`
- Envie as suas alterações: `git push origin my-feature`

> Caso tenha alguma dúvida confira este [guia de como contribuir no GitHub](https://github.com/firstcontributions/first-contributions)

## 📝 Licença

Este projeto esta sobe a licença MIT. Veja a [LICENÇA][license] para saber mais.

Feito com ❤️ por Cintia Zago 👋🏽 [Entre em contato!](https://www.linkedin.com/in/cintiazago/)

[nodejs]: https://nodejs.org/
[express]: https://expressjs.com/
[uuidv4]: https://www.npmjs.com/package/uuidv4
[typescript]: https://www.typescriptlang.org/
[nodemon]: https://www.npmjs.com/package/nodemon
[rs]: https://rocketseat.com.br
[license]: https://opensource.org/licenses/MIT
