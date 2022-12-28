# Utilizando o operador curto de declaração, atribua estes valores às variáveis com os identificadores "x", "y", e "z".

- 42
- "James Bond"
- true

```go
package main

import (
	"fmt"
)

func main() {


	x := 42
	y := "James Bond"
	z := true

	fmt.Println(x,y,z, "\n") // Uma declaração


	// Múltiplas declarações


	fmt.Printf("x = %T \n", x)
	fmt.Printf("y = %T \n", y)
	fmt.Prinf("z = %T \n", z)


}


```
