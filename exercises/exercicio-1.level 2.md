	### Na prática: exercício #1

- Escreva um programa que mostre um número em decimal, binário, e hexadecimal.
- Solução: https://play.golang.org/p/X7qm3aWSa6


Solução (Não consegui resolver e acompanhei):
```go
package main

import (
	"fmt"
)

func main() {

	var number = 122

	// %d decimal
	// %#x hexadecimal
	// %b binary

	fmt.Printf("%d %#x %b", number, number, number)

}

```