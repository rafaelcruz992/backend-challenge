Projeto desenvolvido em .NET Core 3.1 C$

Requisitos necessário para execução do projeto:
Visual Studio 2019

1 - Abrir a .sln no visual studio.
2 - Definir o projeto API que está dentro da pasta 1 - Presentation como startup project (caso não esteja).
3 - Executar o projeto.
4 - Será iniciado o browser com a home.
5 - Para acessar os métodos disponíveis:

GET - http://localhost:64555/api/pedido/123456 (Aqui já defini o id 123456 pois ao iniciar a aplicação será carregar o banco InMemory com este pedido.

POST - http://localhost:64555/api/pedido/
Necessário enviar o objeto no seguinte formato:
{
 PedidoID: 0
 Itens: [{ ItemID:0, Descricao: "string", PrecoUnitario:0, Qtd:0 }]
}

PUT- http://localhost:64555/api/pedido/{id}
Necessário enviar o objeto no seguinte formato:
{
 PedidoID: 0
 Itens: [{ ItemID:0, Descricao: "string", PrecoUnitario:0, Qtd:0 }]
}

DELETE - http://localhost:64555/api/pedido/{id}


O Units testes estão no projeto UnitTestChallenge dentro da pasta 6 - Tests
Para executá-los, basta em Test -> Run All Tests no menu superior

