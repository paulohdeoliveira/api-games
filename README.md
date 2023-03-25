# API de Games
Esta API é utilizada para gerenciar cadastro de games
## Endpoints
### GET /games
Endpoint responsável por retornar a listagem de todos os games cadastrados no banco de dados
#### Parâmetros
Nenhum
#### Respostas
##### OK 200
Você irá receber a listagem dos games
##### Falha na autenticação 401
Aconteceu alguma falha no processo de autenticação da requisição. Motivos: Token inválido, Token expirado.

### POST /auth
Endpoint responsável pelo processo de login.
#### Parâmetros
email: email do usuário cadstrado no sistema

password: senha do usuário cadastrado no sistema
#### Respostas
##### OK 200
Você recebeŕa um token JWT para acessar os endpoints protegidos na API.
##### Falha na autenticação 401
Aconteceu alguma falha no processo de autenticação da requisição. Motivos: senha ou email incorretos.
