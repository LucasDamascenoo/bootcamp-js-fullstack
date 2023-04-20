# Bootcamp Javascript Full Stack

Conteudo ministrado por Guillhermo Rodas em seu canal do [Youtube](https://www.youtube.com/watch?v=Zh9tl2CQUZs&list=PLKBvDYynKmlW1GrqNnwjdgoGP6PlYkxrh).

# Semana 02

## Aula 01

Introdução ao Javascript.

## Valores Primitivos em Js

- Booleans(True,false)
- Numbers (100,3.10)
- Strings ("Oi")
- Symbols (Symbol())
- BigInts (10n)
- Undefined (valor não definido)
- Null (definido mas atribuido)

**Type of** usado para descobrir o tipo de dados

## Objetos e Funções

- Objetos {idade:27}
- funções ( x=> x \* 2)

**Tudo em Javascript que não seja um dado primitivo, é um objeto**

## Váriaveis

- var
- let
- const

**sempre usar const**

## Atribuição deigualdades

- ==
  Compara apenas o valor
- ===
  Compara valor e tipo

  ## Falsy,Trully

  Valores Falsos em Js.

  - false
  - 0
  - -0
  - ""
  - null
  - undefined
  - NaN

Valores Trully em Js.

- true
- 1
- 'conteudo'
- []
- {}
- function()
- new date ()

## Aula 02

## Objetos e suas propriedades

- Objetos literais

Sintaxe mais comum dos objetos, que são um conjunto de chave: valor

```javascript:

const human = {
  name = 'Lucas',
  lastName = 'Oliveira',
  age = 28
}
```

## Adicionando elementos

```javascript:

const human {
  name: 'Lucas',
  lastName: 'Oliveira',
  age: 28
}
human.corCabelo = "Black"


```

## Acessando os propriedades

- atráves de ponto (.)

```javascript:

human.name //Lucas
human.age // 28

```

- atráves de Colchetes []

```javascript:

human["name"] //Lucas
human["age"] // 28

```

## Funções

Temos 3 maneiras de declarar funções em Js.

- Function Statement

É a forma "padrão" de declaração de função;

```javascript:

function hola () {
console.log("Olá")
}

hola() //chamando função

```

- Função Expression

´Criamos uma váriavel e passamos uma função para essa váriavel

```javascript:

const hola = function (){

  console.log("Olá")

}

hola() //chamando função

```

## Parametros e Argumentos

- Parametros

Parametros são "variaveis" Locais de nossas função (ainda sem valor)

- Argumentos

São Parametros quando atribuimos valores

```javascript:

function sum (x,y){
  return x+ y // Parametros
}

sum(10,5) // Argumentos

```

## Referencia e Valor

- Valor

Dados primitivos sempre vão guardar o valor original atribuido

```javascript:

let nome = "Lucas"
let novoNome = nome

nome = "Jair"

//nome agora tem o valor Jair
// novoNome = ainda possui o valor original do nome, ou seja não alterou globalmente o valor  original

```

- Referencia

Em dados não primitivos, os valores são passados por referencia, e quando reatribuir, muda todo local que tenha aquela referencia.

```javascript:

let human = {
  nome: "Lucas"
}

let alien = human

human.nome = "Teste"

// dentro do objeto human, o nome agora passou a ser "Teste"

// e a variavel tambem foi modificada para teste

```

## Operadores Lógicos

- Or ||

Apenas umas das condições precisam ser verdadeiras para todo o check seja true

- And &&

Todas as condições precisam ser verdadeiras para o check ser true

- Not !

Inverte a condição, se false vira true, se true vira false

## Condicionais

Condicionais são "caminhos" lógicos, se isso, faça isso, se aquilo, faça aquilo.

```javascript:

if(age >= 18){
  console.log("Adulto")
} else if ( age > 30){
   console.log(" Muito Adulto Adulto")
} else {
   console.log("Idoso")
}
```

## Ternarios

É um atalho condicional em uma unica linha.

```javascript:

const podeBeber = agr >= 18 ? "Pode beber" : "Não pode beber"

```

## Loops

- For

```javascript:

for(let i = 0; i < 3; i++){
  //executa tarefas enquanto a condição for true

}

```

## Aula 03

## HTML Semántico

- Articles ou Sections?

Usamos Articles quando nosso conteudo está relacionada a algo na pagina, como a informação de um usuario,

- Sections

Separa conteudos que fazem sentido no contexto da página.

## Nav, Header , Footer e Aside

- Nav

Nav normalmente é usado para navegação em uma pagina, como um menu de navegação.

- Header

Usado é para identificar a área principal da pagina

- Footer

Usado para conteudos no fim da pagina, como contatos, links, sobree e etc.

- Aside

Usado mais para conteudos "Laterais"

## Figure , Figpaction e Img

- Figure
  é um "container" semantico para incluir imagens

- Figcaption
  é uma descrição da imagem

- Img

é a forma que incluimos imagens em nosso HTML.

## Seo

Escrever um bom HTML é importante por diversos fatores

- Melhora a busca do nossos paginas em sites de buscas
- Ajuda os eleitores de telas
- Acessibilidade
- Um bom HTML ajuda a escrever um bom CSS
