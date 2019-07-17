### OQUE SÃO MODULOS?

.1 - Módulos são uma forma de dividir 
toda a lógica do seu software em arquivos
diferentes.

.2 - Para criar um módulo em JavaScript você precisará de criar um
arquivo com a extensão "***.js***".

Abrindo o arquivo criado vamos criar uma função que calcule porcentagem

let porcentagem = function(x, y) {
            return (x * y) / 100
}

Após isso iremos usar o códico modules.exports para exportar a variável
porcentagem.

module.exports = porcentagem

.4 - Salvando e fechando o arquivo, vamos criar o arquivo app.js e 
importar o módulo porcentagem.js

let porcentagem = require('./porcentagem.js')
console.log(porcentagem (100, 10))

.5 - Chegou a hora 🎉 de executar nosso script :)

$ node app.js
10

Se você chegou até aqui parabéns :)
.
