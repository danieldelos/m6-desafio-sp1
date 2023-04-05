<h1>Desafio FullStack</h1>

<h2>[201] O sistema deve permitir o cadastro de usuários. </h2>
<h3>POST - /users</h3>

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
<h3>GET - /users</h3>

<strong>Essa rota necessita de autenticação bearer token. Não há Campos de envio para request</strong>

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

<h2>[200] O sistema deve permitir Login de usuários. </h2>
<h3>POST - /login</h3>

<strong>Essa rota não necessita autenticação bearer token.</strong>

<p>Retorno esperado com status code <strong style="color:LimeGreen;font-size:18px">201</strong> para criação realizada com sucesso:</p>
<pre>
{
	"token": "eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJwaG9uZSI6Ijk5OTkiLCJpYXQiOjE2ODA0NTAxODYsImV4cCI6MTY4MDUzNjU4Niwic3ViIjoiMTIifQ.77vTUXOR7p7KexiyjVSYPqzQO16lu48iOn91DsDo17s"
}
</pre>
<hr noshade />

<h2>[200] O sistema deve permitir atualização de usuários. </h2>
<h3>PATCH - /users/id</h3>

<strong>Essa rota necessita autenticação bearer token.</strong>

<p>Retorno esperado com status code <strong style="color:LimeGreen;font-size:18px">201</strong> para atualização realizada com sucesso:</p>
<pre>
{
	"name": "daniel",
	"email": "daniel@Kenzie.com.br",
	"phone": "9999",
	"id": 12,
	"createdAt": "2023-03-25T14:29:31.236Z",
	"updatedAt": "2023-03-27T15:23:59.134Z",
	"deletedAt": null
}
</pre>
<hr noshade />

<h2>[204] O sistema deve permitir deletar um usuários. </h2>
<h3>DELETE - /users/id</h3>

<strong>Essa rota necessita de autenticação bearer token.</strong>

<p>Retorno esperado com status code <strong style="color:LimeGreen;font-size:18px">201</strong> para criação realizada com sucesso:</p>
<pre>
{}
</pre>
<hr noshade />

<h2>Rotas de contatos</h2>

<h2>[201] O sistema deve permitir o contatos. </h2>
<h3>POST - /contacts</h3>

<strong>Essa rota necessita autenticação bearer token.</strong>

<p>Retorno esperado com status code <strong style="color:LimeGreen;font-size:18px">201</strong> para criação realizada com sucesso:</p>
<pre>
{
	"id": 124,
	"contactName": "contato28",
	"contactEmail": "contato14@kenzie.com.br",
	"contactPhone": "8888",
	"createAt": "2023-04-02T15:48:15.722Z",
	"user": {
		"name": "daniel",
		"email": "daniel@Kenzie.com.br",
		"phone": "9999",
		"id": 12,
		"createdAt": "2023-03-25T14:29:31.236Z",
		"updatedAt": "2023-03-27T15:23:59.134Z",
		"deletedAt": null
	}
}
</pre>
<hr noshade />

<h2>[200] O sistema deve permitir atualização de contatos. </h2>
<h3>PATCH - /contacts/id</h3>

<strong>Essa rota necessita de autenticação bearer token.</strong>

<p>Retorno esperado com status code <strong style="color:LimeGreen;font-size:18px">201</strong> para atualização realizada com sucesso:</p>
<pre>
{
	"name": "daniel",
	"email": "daniel@Kenzie.com.br",
	"phone": "9999",
	"id": 12,
	"createdAt": "2023-03-25T14:29:31.236Z",
	"updatedAt": "2023-03-27T15:23:59.134Z",
	"deletedAt": null
}
</pre>
<hr noshade />

<h2>[201] O sistema deve permitir a listagem de contatos. </h2>
<h3>GET - /contacts</h3>

<strong>Essa rota necessita bearer token. Não há Campos de envio para request</strong>

<p>Retorno esperado com status code <strong style="color:LimeGreen;font-size:18px">201</strong> para listagem realizada com sucesso:</p>
<pre>
[
	{
		"id": 125,
		"contactName": "MAIK HENRIQUE SOUSA - MG",
		"contactEmail": "maik.sousa@agrocontar.com.br",
		"contactPhone": "1234567890",
		"createAt": "2023-04-02T15:55:03.714Z",
		"user": {
			"name": "daniel",
			"email": "daniel@Kenzie.com.br",
			"phone": "9999",
			"id": 12,
			"createdAt": "2023-03-25T14:29:31.236Z",
			"updatedAt": "2023-03-27T15:23:59.134Z",
			"deletedAt": null
		}
	},
	{
		"id": 123,
		"contactName": "daniel barbosa da silva",
		"contactEmail": "apeiron52@gmail.com",
		"contactPhone": "0123456789",
		"createAt": "2023-04-02T15:45:47.296Z",
		"user": {
			"name": "daniel",
			"email": "daniel@Kenzie.com.br",
			"phone": "9999",
			"id": 12,
			"createdAt": "2023-03-25T14:29:31.236Z",
			"updatedAt": "2023-03-27T15:23:59.134Z",
			"deletedAt": null
		}
	},
	{
		"id": 121,
		"contactName": "MAIK HENRIQUE SOUSA - SP",
		"contactEmail": "apeiron52@gmail.com",
		"contactPhone": "44444",
		"createAt": "2023-04-02T15:30:23.688Z",
		"user": {
			"name": "daniel",
			"email": "daniel@Kenzie.com.br",
			"phone": "9999",
			"id": 12,
			"createdAt": "2023-03-25T14:29:31.236Z",
			"updatedAt": "2023-03-27T15:23:59.134Z",
			"deletedAt": null
		}
	}
]
</pre>
<hr noshade />

<h2>[201] O sistema deve permitir a listagem de contatos por id. </h2>
<h3>GET - /contacts/users/id</h3>

<strong>Essa rota necessita de autenticação bearer token. Não há Campos de envio para request</strong>

<p>Retorno esperado com status code <strong style="color:LimeGreen;font-size:18px">201</strong> para listagem realizada com sucesso:</p>
<pre>
{
	"name": "daniel",
	"email": "daniel@Kenzie.com.br",
	"phone": "9999",
	"id": 12,
	"createdAt": "2023-03-25T14:29:31.236Z",
	"updatedAt": "2023-03-27T15:23:59.134Z",
	"deletedAt": null,
	"contacts": [
		{
			"id": 121,
			"contactName": "MAIK HENRIQUE SOUSA - SP",
			"contactEmail": "apeiron52@gmail.com",
			"contactPhone": "44444",
			"createAt": "2023-04-02T15:30:23.688Z"
		},
		{
			"id": 123,
			"contactName": "daniel barbosa da silva",
			"contactEmail": "apeiron52@gmail.com",
			"contactPhone": "213141",
			"createAt": "2023-04-02T15:45:47.296Z"
		},
		{
			"id": 124,
			"contactName": "contato28",
			"contactEmail": "contato14@kenzie.com.br",
			"contactPhone": "8888",
			"createAt": "2023-04-02T15:48:15.722Z"
		}
	]
}
</pre>
<hr noshade />

<h2>[204] O sistema deve permitir deletar um contato. </h2>
<h3>DELETE - /contacts/id</h3>

<strong>Essa rota necessita autenticação bearer token.</strong>

<p>Retorno esperado com status code <strong style="color:LimeGreen;font-size:18px">201</strong> para criação realizada com sucesso:</p>
<pre>
{}
</pre>
<hr noshade />
