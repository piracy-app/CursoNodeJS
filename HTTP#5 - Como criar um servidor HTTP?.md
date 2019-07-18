### OQUE É O PROTOCOLO HTTP?

.1 - Http, é um protocolo de Transferência de Hipertexto.

Imagine que você precise acessar o Google, no momento que você acessa o google.com o cliente(você) pedirá o servidor do google.com que mande arquivos para ele.
Essa estrutura de comunicação é chamada de HTTP.

.2 - Para podermos subir um servidor http com (NodeJS) precisamos de criar um arquivo **"app.js"**, após a criação do arquivo iremos escrever algumas instruções.

#!/usr/bin/node

let http = require('http')

/*
(http) Para podemos importar módulos internos do Java Script,
precisamos somente do nome.

(HTML) retorna o documento HTML para o HTTPServer
*/
let HTML = function(req, res) {
     return res.end('hello word!')
}
let porta = 8000
http.createServer(HTML).listen(porta)

console.log(\` Acessar: http://127.0.0.1:${porta}`)

.3 - Executando o servidor
$ node app.js
Acessar: http://127.0.0.1:8000
