#  Api de games
Esta API é utilizada para documentar a rotina games, do curso udemy
## endpoints
### GET / games
este endpoit é responsável por retornar todos os games cadastrados no banco de dados
#### Parametros
nenhum
#### Respostas
##### statuscode 200
Resposta dada ao sucesso da operação, será recebida a listagem de todos os games
##### statuscode 401 - token inválido
Resposta dada quando o token não confere. O que significa falha no processo de autenticação da requisição.
Motivos:
Token inválido
Token expirado
