# Servidor RESTFUL com Nedb

Implementação de uma REST API com Node.js para o curso completo de Javascript da [Hcode](https://hcode.com.br/ "Hcode"). Permite receber dados de usuários por meio dos métodos HTTP, valida-los e realizar a persistência em um banco de dados Nedb, baseado no padrão JSON.

Todos os módulos estão comentados, garantindo facilidade na compreensão da implementação. Ao iniciar o projeto será carregado o servidor express na porta 3000, utilize ferramentas como [Postman](https://www.postman.com/ "Postman") para realizar o teste das rotas especificadas no diretório routes. 

### Módulos utilizados

- Express
- Express validator
- Consign
- Body-parser
- NeDb

### Instalação
```
npm install
```

### Excutando servidor
```
npm start
```
## Rotas
Obter todos os usuários:
```
GET /users
```
Exemplo de resultado:
```json
{
    "users":[]
}
```

Cadastrar um novo usuário:
```
POST /users
```
Exemplo de resultado:
```json
{
    "_id":"hjkhfui324",
    "name":"João Rangel"
}
```

Obter dados de um usuário:
```
GET /users/:id
```
Exemplo de resultado:
```json
{
    "_id":"hjkhfui324",
    "name":"João Rangel"
}
```

Editar um usuário:
```
PUT /users/:id
```
Exemplo de resultado:
```json
{
    "_id":"hjkhfui324"
}
```

Excluir um usuário:
```
DELETE /users/:id
```
Exemplo de resultado:
```json
{
    "_id":"hjkhfui324"
}
```