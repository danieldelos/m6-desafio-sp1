# Desafio FullStack

<h1>Desafio FullStack</h1>

<h2>[201] O sistema deve permitir o cadastro de usuários. </h2>
<h3>POST - /User</h3>

<strong>Essa rota não necessita autenticação bearer token.</strong>

<p>Retorno esperado com status code <strong style="color:LimeGreen;font-size:18px">201</strong> para criação realizada com sucesso:</p>
<pre>
{
	"name": "daniel23",
	"email": "daniel2@Kenzie.com.br",
	"phone": "9999",
	"id": 43,
	"createdAt": "2023-04-03T12:08:55.606Z",
	"updatedAt": "2023-04-03T12:08:55.606Z",
	"deletedAt": null
}
</pre>
<hr noshade />

<h2>[201] O sistema deve permitir a listagem de usuários. </h2>
<h3>GET - /User</h3>

<strong>Essa rota necessita autenticação bearer token. Não há Campos de envio para request:</strong>

<p>Retorno esperado com status code <strong style="color:LimeGreen;font-size:18px">201</strong> para listagem realizada com sucesso:</p>
<pre>
[
	{
		"name": "MAIK HENRIQUE SOUSA - MG",
		"email": "maik@gmail.com",
		"phone": "(62) 32472-820_",
		"id": 30,
		"createdAt": "2023-03-31T11:42:26.392Z",
		"updatedAt": "2023-03-31T11:42:26.392Z",
		"deletedAt": null
	},
	{
		"name": "danilo barbosa",
		"email": "johndoe@email.com",
		"phone": "(62) 98514-4457",
		"id": 32,
		"createdAt": "2023-03-31T21:45:32.757Z",
		"updatedAt": "2023-03-31T21:45:32.757Z",
		"deletedAt": null
	},
	{
		"name": "daniel",
		"email": "daniel@Kenzie.com.br",
		"phone": "9999",
		"id": 12,
		"createdAt": "2023-03-25T14:29:31.236Z",
		"updatedAt": "2023-03-27T15:23:59.134Z",
		"deletedAt": null
	}
]
</pre>
<hr noshade />