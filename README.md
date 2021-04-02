:spiral_calendar: Atualizado em 5 de março de 2021 :heart:

<img align="right" alt="GIF" height="160px" src="https://github.com/rdeconti/rdeconti-resources/blob/main/Digital%20Innovation%20One%20-%20Logotipo.png" />

# Projeto Digital Innovation One MRV .Net Developer
# API Mongo DB
- Este projeto foi proposto pela Digital Innovation One - Link do código original: https://github.com/gabrielfbarros/dotnet-mongo
- Professor: Gabriel Faraday
- Aula: https://web.digitalinnovation.one/project/construindo-um-projeto-de-uma-apinet-integrada-ao-mongodb/learning/b3d35e6f-b202-4c88-a256-2c17e0836061?back=/track/mrv-net-developer&bootcamp_id=2aa1519c-08ce-4f37-873f-368794f735d2

# Descrição
Construiremos um projeto de uma API em .NET Core integrada a um cluster MongoDB, que também criaremos em tempo real no service cloud Mongo Atlas. Vamos repassar brevemente os conceitos básicos de front-end, back-end, bases de dados, NoSQL e MongoDB para fixar o entendimento e sua aplicabilidade.

# Detalhes
Exemplo de aplicação .net core com mongodb.

Para teste:
https://localhost:5001/infectado

```json
{
	"dataNascimento": "1990-03-01",
	"sexo": "M",
	"latitude": -23.5630994,
	"longitude": -46.6565712
}
```
OBS: é preciso ter configurar o acesso ao banco no appsettings.

Links Uteis:

- .net core - https://dotnet.microsoft.com/download
- visual code - https://code.visualstudio.com/download
- postman - https://www.postman.com/downloads/
- mongo atlas - https://www.mongodb.com/cloud/atlas/register

-----------------------------------------------
Referências:

- https://docs.mongodb.com/
- https://docs.mongodb.com/manual/
- https://docs.mongodb.com/ecosystem/drivers/csharp/
- https://docs.atlas.mongodb.com/

# Detalhes obtidos nas aulas

- Cadastramento realizado no Mongo Atlas DB
- Escolhido o Cluster FREE
- Escolhido o Google Cloud Plataform
- Criado o Database com Senha
- Criado o Network IP address
- Criado a conection string
- A aplicação vai tratar dados referentes a pandemia ocasionada pelo coronavirus
- Foram criados o modelo de dados (collections: infectados)
- Adicionou package com: dotnet add package MongoDB.Driver
- ICOnfiguration é uma interface .NET
- Trabalhou com Mapping Classes (fica mais claro para quem lê o código)
- Para cada ENDPOINTS tem uma view model (DTO)
- Tem o banco, tem as classes: tem que fazer o meio de campo que é a controller (classe controller deve ter "controller" no nome)
- Anotações [ApiController]
- Criou o ENDPOINT POST
- Criou o ENDPOINT GET
- A questão da injeção de dependência realizado com o "Data.MongoDB mongoDB" = desacoplamento de código e facilidade de codificação - controlado pelo startup.cs
- Utilizou POSTMAN para verificar a API 
- Pode executar a aplicação com linha de comando: dotnet run ou com F5 para debugar
- No Postman indica no create: http://localhost:5000/infectado
- No Postman executa um POST com estes dados (no Body, Tipo Json)
{
	"dataNascimento": "1990-03-01",
	"sexo": "M",
	"latitude": -23.5630994,
	"longitude": -46.6565712
}

- Executei vários adds no Postman executa um POST com estes dados (no Body, Tipo Json)
- Utilizou o Visual Code Studio com as extensões: C# e C# Extensions

# Testes executados (utilizando IDE Visual Studio 2019)

## Teste: Criação do cluster no MongoDB Atlas

<img src="https://github.com/rdeconti/Projeto-DIO-.Net-API-MongoDB/blob/main/Tests-screens/MongoDB%20-%20Cria%C3%A7%C3%A3o%20do%20cluster.jpg" />

## Teste: Criação do network ip address

<img src="https://github.com/rdeconti/Projeto-DIO-.Net-API-MongoDB/blob/main/Tests-screens/MongoDB%20-%20Cria%C3%A7%C3%A3o%20do%20network%20IP%20address.jpg" />

## Teste: Criação usuário read only

<img src="https://github.com/rdeconti/Projeto-DIO-.Net-API-MongoDB/blob/main/Tests-screens/MongoDB%20-%20Cria%C3%A7%C3%A3o%20do%20usu%C3%A1rio%20read-olny.jpg" />

## Teste: Utilizando Postman - retorno 500

<img src="https://github.com/rdeconti/Projeto-DIO-.Net-API-MongoDB/blob/main/Tests-screens/Postman%20-%20retorno%20500.jpg" />

## Teste: Utilizando Postman - retorno 201

<img src="https://github.com/rdeconti/Projeto-DIO-.Net-API-MongoDB/blob/main/Tests-screens/Postman%20-%20retorno%20201.jpg" />

## Teste: Registros incluidos visualizados no Chrome

<img src="https://github.com/rdeconti/Projeto-DIO-.Net-API-MongoDB/blob/main/Tests-screens/Registros%20incluidos%20visualizados%20no%20Chrome.jpg" />

## Teste: Registros incluidos visualizados no MongoDB Atlas

<img src="https://github.com/rdeconti/Projeto-DIO-.Net-API-MongoDB/blob/main/Tests-screens/Registros%20incluidos%20visualizados%20no%20MongoDB%20Atlas.jpg" />
