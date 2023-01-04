# Na prática: exercício #3

- Crie constantes tipadas e não-tipadas.
- Demonstre seus valores.
- Solução: https://play.golang.org/p/eWnKI59ual

## My solution:
```go
import "fmt"

const ( // Não Tipadas
	consOne   = 1
	consTwo   = 2
	consThree = 3
	// Tipadas
	one int = 4
	two int = 5
)

func main() {

	fmt.Println(consOne, consTwo, consThree, one, two)

}
```