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

## Aula 04

## Cliente - Servidor

Toda vez que estamos utilizando algum serviço online somos os clientes e tudo que vemos está alocada em um servidor.

Cliete (Usuario) faz um requisição para o Servidor que retornar com os dados solicitados.

## Formularios

- Label

- Inputs

- Fieldset

- legend

## Diferença de Links e Botoes

Links usados como "botoes" servem para navegar em seções entre nossa pagina, ou algo externo, já os botoes servem para enviar dados.

## Json

Json(Javascript object notation) é usado para armazenar/partilhar dados em aplicações web entre o cliente/servidor, seu formato é parecido com Objetos em Js, a diferença que nas "chaves" é usado aspas duplas " "

```javascript

{
"nome": "Lucas",
"idade": 28,
"ocupação": "Analista de dados"

},

```

## Dom

é a representação em forma de "arvore" dos elemntos HTML que podem ser acessados e modificados por javaScript

# Semana 03

## Aula 01

## Flexbox terminologia

- FlexContainer

Quando utitlizamos a propriedade **display-flex** o elemento vira um flexcontainer

- Flex items

Tudo que tiver dentro de um flex-container se transforma em um "filho" que chamamos de flex itens

- Flex Wrap

Quebra o conteudo quando atingir o limite total da tela

- Flex Direction

Muda a direção dos flex-itens, por padrão é row (horizontal), columuns e suas variantes reversa.

- Justify-content

movimenta os flex-itens no eixo principal (horizontal)

- Align-items

movimenta os flex-itens no eixo secunrario (vertical)

## Aula 02

## Responsividade

- Posicionamento com css

- [x] Static
- [x] Relative
- [x] Absolute
- [x] Fixed
- [x] Sticky

- O que é o design responsivo?

Design responsivo tem relação com aplicações webs que se ajustam/adpatam a diversos layouts (celulares,tablets,notbooks)

- Mobile First

É uma "estratégia" de desenvolvimento onde consiste em primeiro fazer a aplicação para aplicativos moveis e ir subindo a escala, fazendo com que fique mais facil adaptar os elementos para telas maiores.

**Mobile First em aplicações profissionais deve ter o layout desenvolvido para ser mobile first**

- Design Layouts

- Fluid Layouts

São layouts que utilizamos medidas relativas, que vao se adaptando conforme cresce/diminui

- Adaptive Layouts

Utilizamos breakpoints para limitar os tamanhos, se adapta aos diversos tamanhos mas não é algo fuido.

- Centered Layouts

São paginas que podem ser fluidas, adaptativas mas dependendo do tamanho do monitor, todo o conteudo fica ao centro (de acordo com o tamanho determinado) e o que ultrapassa isso, fica preto.

- Media Queries

**Mobile First** : Quando criamos um layout mobile first criamos os componentes para serem mobiles, para telas maiores precisaremos das medias queries onde iremos utilizar (min-width)

## Aula 03

### Estruturas Modernas de um Projeto

## Aula 04

### Frameworks de UI

- O que é uma biblioteca?

Bibliotecas são conjuntos de blocos (codigos) pre-desenvolvido que podem ser reutilizados e que nos facilita em nossas aplicações.

Exemplos de Bibliotecas web.

- React
- Vue
- Angular
- Redux

- O que é um Framework?

frameworks são estruturas pré-definidas que fornecem diretrizes, ferramentas e bibliotecas para facilitar o desenvolvimento de aplicativos e sites da web. Eles ajudam os programadores a serem mais eficientes, fornecendo uma base sólida e reutilizável para seus projetos.

Exemplos de Frameworks web.

- NextJs
- Laravel

- Packages de Biblioteca

- Package.json

npm init -y cria um arquivo pachage.js que define as propriedades de nossos projetos

- Frameworks de ui

- Bootstrap
- Tailwind
- Bulma (menos pupular)

# Semana 03

## Aula 02

### Datas em Javascript
