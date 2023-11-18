# Sistema de Frente de Caixa :credit_card:
:white_check_mark: Status: Concluído

Este projeto é um Sistema de Ponto de Venda (PDV) desenvolvido em Node.js que visa facilitar a gestão de vendas e operações de caixa para estabelecimentos comerciais. O PDV é uma ferramenta essencial para lojas, restaurantes, supermercados e outros tipos de negócios que lidam com transações de venda.
## :bangbang: Pré-requisitos :bangbang:
Antes de começar, certifique-se de ter instalado em sua máquina:
- Node.js
- npm (Node Package Manager)
- PostgreSQL
- Visual Studio

## 🎮 Funcionalidades
- Cadastro, Login e Atualização de Usuário
- Detalhar usuário
- Cadastro, Atualização e Exclusão de Produto
- Listagem e Detalhamento de Produtos
- E muito mais 

Explore as rotas disponíveis para aproveitar ao máximo as funcionalidades.
## :bowing_man: Como usar
1. Clone o repositório:
```
git@github.com:PatrickRigaud/desafio-backend-modulo-05-sistema-pdv-dbe-t02-2.git
```
2. Instale as dependências do projeto:
```
npm install
```
3. Inicie o servidor (somente após concluída todas as etapas seguintes):
```
npm run dev
```

> Use o Insomnia, Postman (ou outro cliente HTTP) para criar as rotas para acessar as funcionalidades da API.

> Para autenticação, adicione o token de acesso (Recebido após requisição de login) na propriedade autorizhation do cabeçalho (Header).

> Certifique-se de enviar dados no formato JSON ao fazer requisições que exigem corpo (request body).

## :world_map: Sobre as Rotas
### Cadastrar Usuário
``
(POST) http://localhost:3000/usuario
``

➡️ Descrição: Esta rota permite criar um novo usuário na aplicação. Os dados do usuário devem ser fornecidos no body da requisição no formato JSON

⬇️ Exemplo de body no formato JSON ⬇️

```JSON
{
    "nome": "João",
    "email": "joao@email.com",
    "senha": "123abc"
}
```
### Login
``
(POST) http://localhost:3000/login
``

➡️ Descrição: Está rota é usada para autenticar um usuário existente. Um token de autenticação é gerado se as credenciais forem válidas, permitindo o acesso às funcionalidades protegidas da API.

⬇️ Exemplo de body no formato JSON ⬇️

```JSON
{
    "email": "joao@email.com",
    "senha": "123abc"
}
```
### Detalhar Usuário
``
(GET) http://localhost:3000/usuario
``

➡️ Descrição: Está solicitação é para detalhar os dados do usuário.

### Atualizar Usuário
``
(PUT) http://localhost:3000
``
