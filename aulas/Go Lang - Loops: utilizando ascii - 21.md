# Loops: utilizando ascii

- Desafio surpresa!
- Format printing:
    - Decimal       %d
    - Hexadecimal   %#x
    - Unicode       %#U
    - Tab           \t
    - Linha nova    \n
- Faça um loop dos números 33 a 122, e utilize format printing para demonstrá-los como texto/string.
- Solução: https://play.golang.org/p/REm2WHyzzz

```go
package main

import "fmt"

func main() {

	// Faça um loop dos números 33 a 122, e utilize format printing para demonstrá-los como texto/string.

	for numTo122 := 33; numTo122 <= 122; numTo122++ {

		fmt.Printf("%d %#x %#U", numTo122, numTo122, numTo122)
		fmt.Println()
	}
}

```
