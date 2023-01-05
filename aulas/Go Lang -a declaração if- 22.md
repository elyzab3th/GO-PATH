# Condicionais: a declaração if

- If: bool
- If: o operador não → "!"
- If: declaração de inicialização
- Go Playground: https://play.golang.org/p/6nq2Tjb07i

#

```go
package main

import "fmt"

func main() {

	var soul bool = true

	if !(soul == false) {
			fmt.Println("Var soul is not equal to False")
	}

}
```