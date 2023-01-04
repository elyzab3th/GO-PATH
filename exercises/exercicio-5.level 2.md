# Na prática: exercício #5

- Crie uma variável de tipo string utilizando uma raw string literal.
- Demonstre-a.
- Solução: https://play.golang.org/p/RkpqPpRWuo

```go
package main

import (
	"fmt"
)

func main() {

	TEXT := `
	
	
		IF 
			NOTHING
				HAS
					COLLECTED,
						NOTHING
							WILL
								ANALYZE.
	`

	fmt.Println(TEXT)

}

```

<a href="https://go.dev/play/p/mrHK69uulCI">Code</a>