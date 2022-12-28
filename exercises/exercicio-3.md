# Utilizando a solução do exercício anterior:
- Em package-level scope, atribua os seguintes valores às variáveis:
	- para "x" atribua 42
	- para "y" atribua "James Bond"
	- para "z" atribua true

- Na função main:

	- Use fmt.Sprintf para atribuir todos esses valores a uma única variável. Faça essa atribuição de tipo string a uma variável de nome "s" utilizando o operador curto de declaração.
	- Demonstre a variável "s".
	

```go
package main

import (
	"fmt"
	"io"
	"os"
)

var x, y, z = 42, "James Bond", true

func main() {

	s := fmt.Sprintf("%s, %s, %s", x, y, z)

	io.WriteString(os.Stdout, s)

}

```

(Link)[https://go.dev/play/p/Qa5EHGWLP6A]
