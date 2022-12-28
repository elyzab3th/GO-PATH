#  Valor zero

- Declaração vs. inicialização vs. atribuição de valor. Variáveis: caixas postais.

- O que é valor zero?

- Os zeros:
	- ints: 0
	- floats: 0.0
	- booleans: false
	- strings: ""
	- pointers, functions, interfaces, slices, channels, maps: nil

- Use := sempre que possível.
- Use var para package-level scope.

#

Antes de falarmos sobre o valor 0 especificamente temos que definir 3 termos: `Declaração` , `inicialização`, `atribuição`. Para enterdemos esses termos utilisaremos um exemplo de caixa postal.

### `Declaração`
Você vai ao correio e pede por uma caixa postal. A pessoa que trabalha no local vai te dar documentos, assinutaruas e uma taxa para pagar. Dado tudo isso você terá uma caixa postal.

### `Inicialização` (primeiro valor colocado dentro de uma variável)
Você comprou uma caixa postal e a primeira coisa que você receber será chamado

### `Atribuição`

- Declaração é quando você compra um endereço de caixa postal.
- Inicialização é quando se recebe a primeira correspondência da caixa postal
- Atribuição é o valor colocado depois


## Na prática

```go
package main

import (
		"fmt"
		)

var x int // Declaração

func main () {

			x = 10 // Inicialização | Ou seja, nossa primeira primeira atribuição de 
				// valor à uma váriavel.


			x = 11 // Atribuição | Atribuindo valor à uma variável

			fmt.Print(x)
}
```


# Valor Zero

O `valor zero` é o valor que se encontra presente em uma variável antes dela ser inicializada pelo usuário.

Quando você compra uma caixa postal ela vem vazia e esse vazio é um 0, e esse 0 é o que queremos ver.

Se sua variável for uma `string` o valor Zero será outro, se for `Integer` o seu valor Zero será outro, se for `float` será outro valor, caso seja `bool` será um outro valor.

#### ! - Cada tipo terá um valor `0` diferente - !

- Os Zeros
	- ints: 0
	- floats: 0.0
	- booleans: false
	- strings: ""
	- pointers, functions, interfaces, slices, channels, maps: nil


```go
package main

import (
			"fmt"
		)

var a int			// Declaration
var b float64		// Declaration
var c string		// Declaration
var d bool			// Declaration

func main () {

		fmt.Printf("%v %T\n", a, a)
		fmt.Printf("%v %T\n", b, b)
		fmt.Printf("%v %T\n", c, c)
		fmt.Printf("%v %T\n", d, d)
}

// OUTPUT:

	//0 = int
	//0 = float64
	// = string
	//false = bool

	// Sempre que você declarar uma variável e não inicializar ela, automaticamente
	// conterá por padrão o valor 0
```