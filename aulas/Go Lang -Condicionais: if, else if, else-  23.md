# Condicionais: if, else if, else

- If, else.
- If, else if, else.
- If, else if, else if, ..., else.
- Go Playground: https://play.golang.org/p/18VrRX2pec

# If, else

```go
package main

import "fmt"

func main() {

	if x := 111; x < 20 {
		fmt.Println("x é Menor que 20")
	} else if x < 10 {

		fmt.Println("x é menor que dez")
	} else {

		fmt.Println("x é maior que 20")
	}
}
```