# Na prática: exercício #6

- Utilizando iota, crie 4 constantes cujos valores sejam os próximos 4 anos.
- Demonstre estes valores.
- Solução: https://play.golang.org/p/zRBEooRvo4

# Dei uma olhada no link acima pra resolver melhor:
```go
//# Na prática: exercício #6

//- Utilizando iota, crie 4 constantes cujos valores sejam os próximos 4 anos.
//- Demonstre estes valores.
//- Solução: https://play.golang.org/p/zRBEooRvo4

package main

import "fmt"

const (
	_ = 2023 + iota
	yearNow
	year2
	year3
	year4
)

func main() {

	fmt.Println(yearNow, year2, year3, year4)

}
```

<a href="https://go.dev/play/p/Vp41iWbLwuv">Link to Code</a>