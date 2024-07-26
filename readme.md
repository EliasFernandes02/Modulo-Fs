fs.readFile()
fs.writeFile() ->
fs.mkdir() -> recursive
fs.appendFile() -> adiciona conteúdo a um arquivo existente
fs.unlink() -> remove arquivos
fs.remdir -> remove pastas




ex1: Escrever em um arquivo 
ex2: Ler esse arquivo
ex3:Criar pastas
ex3: Criar pastas dentro de pastas
ex4:Deletar arquivos
ex5:Deletar pastas
ex6:Deletar arquivos dentro de pastas
ex7: Crie a estrutura de pastas
projeto/
  └── src/
      └── controllers/
      └── models/
      └── views/
ex8: Escreva um script que cria um arquivo chamado dados.txt e grava a string "Hello, Node.js!" nele. Depois, leia o conteúdo do arquivo e exiba-o no console.
ex9: Escreva um script que adicione a string "Mais conteúdo!" ao final do arquivo dados.txt (criado no Exercício 2).
ex10:Escreva um script que delete o arquivo dados.txt.
ex11:Escreva um script que delete o diretório projeto criado no Exercício 1, incluindo todos os seus subdiretórios.
ex12: Escreva um script que leia o conteúdo de um arquivo texto.txt e conte o número de linhas presentes no arquivo. Exiba o resultado no console.
Nome,Idade,Email;
Alice,30,alice@example.com;
Bob,25,bob@example.com;
Carol,28,carol@example.com;
David,22,david@example.com;
Eva,35,eva@example.com;
Frank,40,frank@example.com;
Grace,27,grace@example.com;
Hank,32,hank@example.com;
Ivy,24,ivy@example.com;
Jack,29,jack@example.com;


ex13: Preciso mover dados de um arquivo para o outro adicionando todos os dados desse arquivo e adicionando novos dados, por exemplo, em texto.txt existem dados de usuarios e eu gostaria de mover todos esses dados de texto.txt para texto2.txt e adicionar novos dados 

FrankAguiar,40,frank@example.com;
GraceJones,27,grace@example.com;
HankXaves,32,hank@example.com;
IvyJune,24,ivy@example.com;
HughJackman,29,jack@example.com;

e no final o resultado será os dados de texto.txt com esses novos dados.

fs.readFile()
fs.writeFile() ->
fs.mkdir() -> recursive
fs.appendFile() -> adiciona conteúdo a um arquivo existente
fs.unlink() -> remove arquivos
fs.rmdir -> remove pastas


fs.readFile('texto.txt', "utf8", function(err, data){
    if(err){
        console.log("Erro")
    } 
    
    let linha = data.split(';')

    let numeroLinhas = linha.length

    console.log(numeroLinhas)
})
