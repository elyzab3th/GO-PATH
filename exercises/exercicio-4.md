# Na prática: exercício #4

	- Crie um tipo. O tipo subjacente deve ser int.
	- Crie uma variável para este tipo, com o identificador "x", utilizando a palavra-chave var.
	- Na função main:
		- Demonstre o valor da variável "x"
		- Demonstre o tipo da variável "x"
		- Atribua 42 à variável "x" utilizando o operador "="
		- Demonstre o valor da variável "x"

```go
package main

import (
	"fmt"
)

type sub_int int

var x sub_int

func main() {

	fmt.Printf("\n Value: %v \n Type: %T", x, x)

	x = 42 // Atribuindo

	fmt.Print("\n================================================================================")

	fmt.Printf("\n Value: %v \n Type: %T", x, x)
}

```

(LINK)[https://go.dev/play/p/p-c8Dl4K_E8]

