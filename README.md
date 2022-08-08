# Prepare-se
Repositório dedicado à preparação para entrevista de emprego!

Aqui estão algumas das perguntas feitas em entrevistas técnicas para vaga FrontEnd Javascript:

<details>
<summary><strong>👨‍💻 1. O que é o JavaScript?</strong></summary><br />
O JavaScript é uma linguagem de script, criada em 1995 por Brendan Eich na Netscape. Inicialmente criada para o popular navegador Netscape Navigator, com o passar dos anos, passou a ser a linguagem padrão dos navegadores e hoje é uma das mais populares do mundo. É possível usar JavaScript para o desenvolvimento web, desenvolvimento de aplicativos mobile, de aplicações de backend e até aplicações de IOT.
</details>
<details>
<summary><strong>👨‍💻 2. Qual é a diferença entre JavaScript e ECMA Script?</strong></summary><br /> 
O ECMA Script é uma especificação, contendo diretrizes e regras para padronizar o JavaScript, mantida pela comunidade e gerida pela Mozila Foundation. O JavaScript é uma linguagem de script que segue os padrões sugeridos pelo ECMA Script.
</details>
<details>
<summary><strong>👨‍💻 3. Qual a diferença entre valor indefinido e nulo?</strong></summary><br /> 
Um valor indefinido significa que uma variável foi declarada, mas ainda não foi atribuído um valor, já um valor nulo é um valor atribuído ou resultado de um erro que foi gerado.

As variáveis no JavaScript quando inicializadas e não atribuídas tem em seu valor por padrão indefinido. O JavaScript não define um valor como nulo, você precisa definir manualmente.
</details>
<details>
<summary><strong>👨‍💻 4. Que tipos de dados são suportados pelo JavaScript?</strong></summary><br /> 
O JavaScript possui 7 tipos de dados primitivos: String, Number, Boolean, BigInt, Null, Undefined e Symbol. O tipo de dado Object entra na lista como oitavo, embora seja listado como um tipo, um Object é uma estrutura de dados.
</details>
<details>
<summary><strong>👨‍💻 5. O que o operador typeof do JavaScript faz?</strong></summary><br /> 
O tipo do dado de um operando em formato de string, podendo por exemplo retornar se o valor verificado é uma String, Number, Boolean, Null, Undefined, entre outros.

Exemplo de uso do typeof
```
const mensagem = "Algum texto aqui";
console.log(typeof mensagem); // output: string

const ano = 2022;
console.log(typeof ano); // output: number
```
</details>
<details>
<summary><strong>👨‍💻 6. O que é uma closure no JavaScript?</strong></summary><br />
Closures são variáveis ou funções que fazem parte do escopo de uma função, possuem acesso limitado ao escopo da função a que pertencem.
</details>
<details>
<summary><strong>👨‍💻 7. O que é a diretiva use strict do JavaScript?</strong></summary><br />
O modo strict é uma forma de manter a escrita do JavaScript mais rigoroso, proibindo o uso de algumas sintaxes ainda não suportadas ou que provavelmente serão definidas em versões futuras do ECMAScript, além de práticas não recomendas pela linguagem, como atribuição de valores a variáveis não definidas, uso global de variáveis, entre outros pontos.

Ao usar o modo strict, estes erros silenciosos do JavaScript são lançados como exceções.
</details>
<details>
<summary><strong>👨‍💻 8. Qual a diferença entre == e ===?</strong></summary><br />
A igualdade ampla (==) compara dois valores após converter ambos os valores para um tipo comum, independente do seu tipo. Após as conversões o == verifica a igualdade do valor.

A igualdade estrita (===) compara dois valores para a igualdade antes de realizar qualquer conversão. Este comparador verifica se o tipo e o valor estão iguais. Geralmente é o comparador mais indicado a se utilizar.
</details>
<details>
<summary><strong>👨‍💻 9. O que são e quando usar template strings?</strong></summary><br />
Uma Template String é uma string que permite criar expressões embutidas, usando acentos graves para envolver a string no lugar de aspas. É possível usar uma expressão com strings multi-linhas ou realizar a interpolação de string usando uma expressão.

É utilizando quando precisamos adicionar em uma string uma ou mais variáveis.

Exemplo de Template String
```
const outraVariavel = 'texto'
const mensagem = `meu ${outraVariavel} com mais texto`; 
```
</details>
<details>
<summary><strong>👨‍💻 10. Como você pode lançar exceções manualmente no JavaScript?</strong></summary><br />
Usando a declaração throw com uma expressão, geralmente uma instância do construtor Error do JavaScript. Ao lançar esta exceção a função será interrompida e o retorno será passado para o primeiro bloco da função catch em um try.

Se nenhum bloco catch estiver definido, a função será interrompida.
</details>
<details>
<summary><strong>👨‍💻 11. O que faz a declaração debugger no JavaScript?</strong></summary><br />
Quando um depurador de código está ativado, por exemplo, o debugger no Chrome, faz a execução do script pausar no ponto que a declaração está definida, como um breakpoint, para que o código possa ser inspecionado.

Exemplo de uso do debugger
```
function minhaFuncao() {
  const mensagem = 'Alguma coisa aqui';
  const resultado = 2 * 8;
  
  debugger;
  // pausa aqui para depurar o código.
}
```
</details>
<details>
<summary><strong>👨‍💻 12. Quais os tipos de erros padrões gerados em exceptions no JavaScript?</strong></summary><br />
Além do construtor genérico para o objeto Error existem os tipos EvalError, ReferenceError, RangeError, SyntaxError, TypeError, URIError e InternalError (não é mais recomendado).
</details>
<details>
<summary><strong>👨‍💻 13. O que é um callback no JavaScript?</strong></summary><br />
É uma função que é executada só após a execução de outra função. A função de callback é passada como argumento de uma função inicial e será executada na sequência.

Exemplo de um callback
```
function segundaMensagem() {
  console.log('Mensagem 2.');
}

function primeiraMensagem(nome, callback) {
  console.log('Mensagem 1: ', nome);
  callback();
}

primeiraMensagem('Daniel', segundaMensagem);
```
</details>
<details>
<summary><strong>👨‍💻 14. O que são laços e iterações em JavaScript?</strong></summary><br />
São formas de realizar operações múltiplas vezes. Os tipos de laços e iterações do JavaScript mais comuns são: while, do while, for, for in e for off.
</details>
<details>
<summary><strong>👨‍💻 15. O que faz a função map em uma coleção?</strong></summary><br />
A função map permite percorrer uma coleção de itens de um array para fazer alguma operação de transformação ou alteração nos itens, ao final o map retorna uma nova lista com a mesma quantidade de itens da lista inicial.

Exemplo de uso do map
```
const cores = ['branco', 'azul', 'vermelho'];

const resultado = cores.map((corAtual) => {
    console.log(corAtual);
    return corAtual.toUpperCase();
})

console.log(resultado) // ['BRANCO', 'AZUL', 'CINZA']
```
</details>
<details>
<summary><strong>👨‍💻 16. O que é uma Promise em JavaScript? Quais são seus estados?</strong></summary><br />
Uma Promise em JavaScript é um objeto usado para realizar operações assíncronas, ela contém um valor que poderá estar ou não disponível no futuro. É ideal para controlar um fluxo do sistema, quando várias operações precisam ser realizadas de forma paralela.

Uma promise contém três estados:

Pending: Quando a promessa é iniciada mas ainda não foi realizada nem rejeitada.
Fulfilled: Quando a promessa é finalizada com sucesso.
Reject: Quando ocorre algum erro e a promessa é encerrada.
Settled: Quando a promessa é encerrada e sabe se foi finalizada com sucesso ou falha.

Exemplo de uma Promise
```
// Criando uma promise
const minhaPromessa = new Promise((resolve, reject) => {
  try {
    // Faz alguma coisa aqui.
    const valorInicial = 5;
    const multiplicador = 7
    const resultado = multiplicador * valorInicial;

    resolve(resultado)
  } catch (erro) {
    reject(erro)
  }
})
                      
// Executando uma promise
minhaPromessa
  .then((parametrosRetornados) => { 
    /* sucesso */
    console.log('Promessa realizada com sucesso');
    console.log(`Resultado: ${parametrosRetornados}`);
  })
  .catch((erro) => {
    console.log('Promessa teve algum erro');
    console.log(erro.message);
  })
  ```
  </details>
