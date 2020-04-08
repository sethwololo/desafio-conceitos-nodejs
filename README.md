# Desafio 02 : Conceitos do Node.JS 

Essa é uma aplicação para armazenar repositórios, que permite a criação, listagem, atualização e remoção dos repositórios, e além disso permitir que os repositórios possam receber "likes".

## Como baixar e executar o projeto

 - Clone o repositório ou baixe como ZIP e descompacte;
 - Abra seu terminal na pasta raiz do projeto e execute `yarn` para baixar as dependências;
 - Para executar o servidor express execute o comando  `yarn dev`
 - Para executar os testes automatizados execute o comando  `yarn test`
 - O servidor será executado na porta 3333
 
## Rotas da aplicação
 - Criar um repositório
  `POST http://localhost:3333/repositories`
 - Listar repositórios
  `GET http://localhost:3333/repositories`
 - Alterar um repositório
  `PUT http://localhost:3333/repositories/:id`
 - Deletar um repositório
  `DELETE http://localhost:3333/repositories/:id`
 - Adicionar um like ao repositório
  `POST http://localhost:3333/repositories/:id/like`

## Corpo das requisições
Para as requisições de criação e alteração é necessário especificar os dados do repositório no formato JSON
  
  {
		"title": "Título do repositório",
		"url": "https://github.com/sethwololo/desafio-conceitos-nodejs",
		"techs": ["nodejs", "react"]
	}
  
