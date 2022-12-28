# Operador curto de declaração


## Subtópicos
- `:=` parece uma marmota (gopher) ou o punisher.
- Uso:
	- Tipagem automática
	- Só pode repetir se houverem variáveis novas
	- != do assignment operator (operador de atribuição)
	- Só funciona dentro de codeblocks
- Terminologia:
	- keywords (palavras-chave) são termos reservados
	- operadores, operandos
	- statement (declaração, afirmação) → uma linha de código, uma instrução que forma uma ação, formada de expressões
	- expressão -> qualquer coisa que "produz um resultado"
	- scope (abrangência)
		- package-level scope
- Lição principal:
	- := utilizado pra criar novas variáveis, dentro de code blocks
	- = para atribuir valores a variáveis já existentes

# := parece uma marmota (gopher) ou o punisher.
O
operador curto de declaração é um caracter semelhante a marmota.
***MARMOTA***
<img src="https://upload.wikimedia.org/wikipedia/commons/thumb/3/3b/Marmot-edit1.jpg/800px-Marmot-edit1.jpg">

E a **`marmota`** é o mascote da linguagem `GO`.

<img src="https://go.dev/blog/gopher/header.jpg">

# Uso

Vimos que o mascote é igual ao operador `:=`. Usamos esse operador para declarar variaével no golang.

#### Declarando Variáveis
```go
// SYNTAX
var := Content

// Example

Myage := 19

```

```go
package main

import "fmt"

func main() {

	Myage := 19

	fmt.Println(Myage)

}

```

## Tipagem automática

 O operador `:=` automaticamente define o tipo da variável.

## Só pode repetir se houverem variáveis novas

Em `Go` só se repete a `var` se atribuirmos se atribuirmos um valor.

## Só funciona dentro de codeblocks

Sabe quando você tenta declarar uma variável fora do função `main`? então, para isso se deve evitar o uso do `operador curto de declaração` ==> `:=` fora do `codeblock`.

E para declarar uma variável fora do codeblock usa-se `var`.


### Syntax
```go
var name type = expression
```


### Maneira Incorreta
```go
package main

import ("fmt")

name := "Elon Musk" // Evite usar operador := fora da func main

func main () {

		fmt.Println(name)

}

```

### Maneira Correta

```go
package main

import ("fmt")

var name string = "Elon Musk" // Caso queira declarar um variável fora, use var

func main () {

	fmt.Println(name)

}
```


# Terminologia

## keywords (palavras-chave) são termos reservados
As seguintes palavras-chave são reservadas e não podem ser usadas como identificadores.

```go
break        default      func         interface    select
case         defer        go           map          struct
chan         else         goto         package      switch
const        fallthrough  if           range        type
continue     for          import       return       var
```

## operadores, operandos

Um termo e distinção básica:

```go
package main

import "fmt"
func main() {

	x := 10 + 10

	fmt.Println(x)
}

```

## expressão -> qualquer coisa que “produz um resultado”
