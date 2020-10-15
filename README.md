#  Api de games
Esta API é utilizada para documentar a rotina games, do curso udemy
## Endpoints
### GET / games
este endpoit é responsável por retornar todos os games cadastrados no banco de dados
#### Parametros
nenhum
#### Respostas
##### statuscode 200
Resposta dada ao sucesso da operação, será recebida a listagem de todos os games
```
[
    {
        "id": 1,
        "titulo": "game of tres quatro",
        "year": "4444",
        "preco": 22,
        "createdAt": "2020-10-12T11:50:50.000Z",
        "updatedAt": "2020-10-15T01:15:18.000Z"
    },
    {
        "id": 2,
        "titulo": "game of dois",
        "year": "2020",
        "preco": 33,
        "createdAt": "2020-10-12T11:52:41.000Z",
        "updatedAt": "2020-10-12T11:52:41.000Z"
    },
    {
        "id": 6,
        "titulo": "game seis seis quatro",
        "year": "4364",
        "preco": 364,
        "createdAt": "2020-10-13T01:53:25.000Z",
        "updatedAt": "2020-10-13T19:32:17.000Z"
    },
    {
        "id": 8,
        "titulo": "game of telma window",
        "year": "2100",
        "preco": 324.34,
        "createdAt": "2020-10-13T01:57:17.000Z",
        "updatedAt": "2020-10-13T01:57:17.000Z"
    },
    {
        "id": 13,
        "titulo": "game teste",
        "year": "343",
        "preco": 23,
        "createdAt": "2020-10-15T01:14:03.000Z",
        "updatedAt": "2020-10-15T01:14:03.000Z"
    }
]

```


##### statuscode 401 - token inválido
Resposta dada quando o token não confere. O que significa falha no processo de autenticação da requisição.
Motivos:
Token inválido
Token expirado
Resposta 
```
{
    "err": "token invalido"
}

```
### POST /auth
este endpoit é responsável por AUTORIZAR O ACESSO aos endpoints
#### Parametros
email: email do usuario cadastrado no sistema
senha: senha do email cadastrado no sistema
Exemplo:

```
 
```
#### Respostas
##### statuscode 200
Resposta dada ao sucesso da operação, será recebida a listagem de todos os games
```
  
]

```
##### statuscode 400 - usuario não cadastrado
Resposta dada quando o usuário não está cadastrado no sistema
 
Exemplo:
```
{
    "err": "usuário não cadastrado"
}

```

##### statuscode 401 - credenciais invalida
Resposta dada quando a senha ou e-mail não conferem com os dados do sistema. O que significa falha no processo de autenticação da requisição.
Motivos:
Senha ou e-mail invalidos
Exemplo:
```
{
    "err": "credenciais inválidas"
}

```
