# Loops: a declaração for

- For: inicialização, condição, pós
- For: condição ("while")
- For: ...ever? (http servers)
- For: break
- golang.org/ref/spec#For_statements, Effective Go
- (Range vem mais pra frente.)

# While no Go
Em `GO` podemos substituir `While` por `for`:
```go
package main

import "fmt"

func main() {

	for {

		fmt.Println("Infinite Loop")

	}


}

```
Outra maneira de refatorar o mesmo código seria:
```go
package main

import "fmt"

func main() {

	for true {
		fmt.Println("Infinite Loop")
	}


}
```