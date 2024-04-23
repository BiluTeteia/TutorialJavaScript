# Tutorial para JavaScript

Neste arquivo serão mostrados os princípios básicos de JavaScript, como sintaxe, variáveis, tipos, funções e estruturas de controle.

## O que é JavaScript?

JavaScript (frequentemente abreviado como JS) é uma linguagem de programação interpretada estruturada, de script em alto nível com tipagem dinâmica fraca e multiparadigma (protótipos, orientado a objeto, imperativo e funcional). Juntamente com HTML e CSS, o JavaScript é uma das três principais tecnologias da World Wide Web. JavaScript permite páginas da Web interativas e, portanto, é uma parte essencial dos aplicativos da web. A grande maioria dos sites usa, e todos os principais navegadores têm um mecanismo JavaScript dedicado para executá-lo. É atualmente a principal linguagem para programação client-side em navegadores web. É também bastante utilizada do lado do servidor através de ambientes como o node.js.

## Configuração de Ambiente

1. Primeiro devemos verificar se temos instalado no computador o Node.js. Para essa verificação no windows utilizamos no terminal de comando (CMD) o comando:
```
node --version
```

2. Em seguida devemos verificar se temos instalada a IDE mais conhecida atualmente é o Visual Studio Code. Para essa verificação no windows utilizamos no terminal de comando (CMD) o comando:

```
code --version
```

## Sintaxe Básica

O JavaScript é uma linguagem com tipagem básica, isso significa que não é necessário explicitar o tipo (`number`, `string`, `boolean`...) que a variável possui, como em Java.

### Exemplo:

```
const nomeDeVariavel = 5
```

Como é possível ver, a variável não possui um tipo específico, ela é simplesmente criada com uma palavra-chave que a antecede, neste caso foi usado _const_, que indica que o valor desta variavel (5) não pode ser alterado. Para ser possível alterar o valor de uma variável é neccesário usar a palavra-chave _let_ (é possível também usar a palavra-chave _var_, mas ela já caiu em desuso)

## Variáveis e Tipos de Dados

As variáveis mais comuns no JavaScript são:

* String - Usado para declarar textos
* Number - Usado para declarar números 
* Boolean - Usado para declarar valores ou falsos ou verdadeiros
* Array - Usado para se armazenar múltiplos valores dentro de uma variável
* Object - Usado para declarar uma variável com propriedades 

### Exemplo:

```
const variavelString = "Texto"
const variavelNumber = 5
const variavelBoolean = true
const variavelArray = [1, "dois", 3, false, 5]
const variavelObjeto = {
  chave1 = "Valor da chave 1",
  chave2 = 2,
  chave3 = variavelNumber
}
```

## Funções

Funções são blocos de código com o propósito de fazer uma tarefa específica. Essas funções usam a palavra-chave "return" para entregar o resultado da função.

### Exemplo: 

```
function nomeDaFuncao(nomeDoParametro){
  return "O parametro é: " + nomeDoParametro
}
```

Neste exemplo a função de nome "nomeDaFunção" recebe como parametro um valor qualquer, de nome "nomeDoParametro", e retorna uma frase com o valor que foi atribuído à "nomeDoParametro". Caso o valor de "nomeDoParametro" seja "Brasil", o resultado dessa função, ou seu retorno, será: "O parametro é: Brasil"

## Estruturas de contole

No JavaScript estruturas de controle permitem que desenvolvedores tomem decisões, iterem dados, lidem com erros e criem algoritmos complexos, duas das estruturas de controle mais comuns são o `if` e o loop `for`

A estrutura `if` serve para comparar valores, assim efetuando linhas de código somente **se** algo for verdadeiro ou falso

### Exemplo:

```
const numeroMaior = 2
const numeroMenor = 4

if (numeroMaior > numeroMenor){
  return "Esta linha de codigo será efetuada"
}

if (numeroMaior < numeroMenor){
  return "Esta linha de código nunca será efetuada"
}
```

A estrutura `for` serve para repetir um bloco de código x vezes. Sua estrutura recebe primeiro um valor inicial: `let i = 1`, um verificador para conferir se o loop continuará: `i <= 10`, e um incrementador: `i += 1`

### Exemplo:

```
for(let i = 1; i <= 10; i += 1){
  console.log("Iteração de número: " + i")
}
```

Neste caso o resultado deste loop será:

```
Iteração de número: 1
Iteração de número: 2
Iteração de número: 3
Iteração de número: 4
Iteração de número: 5
Iteração de número: 6
Iteração de número: 7
Iteração de número: 8
Iteração de número: 9
Iteração de número: 10
```
