# Na prática: exercício #4

- Crie um programa que:
    - Atribua um valor int a uma variável
    - Demonstre este valor em decimal, binário e hexadecimal
    - Desloque os bits dessa variável 1 para a esquerda, e atribua o resultado a outra variável
    - Demonstre esta outra variável em decimal, binário e hexadecimal
- Solução: https://play.golang.org/p/IiwgT0v3Mp

# My solution:
```go
//# Na prática: exercício #4

//- Crie um programa que:
//    - Atribua um valor int a uma variável
//    - Demonstre este valor em decimal, binário e hexadecimal
//    - Desloque os bits dessa variável 1 para a esquerda, e atribua o resultado a outra variável
//   - Demonstre esta outra variável em decimal, binário e hexadecimal
//- Solução: https://play.golang.org/p/IiwgT0v3Mp

package main

import "fmt"

var x int

func main() {

	fmt.Printf("%d %b %#x", x, x, x)
	deslocamento := x << 1
	fmt.Printf("%d \t %b \t %#x ", deslocamento, deslocamento, deslocamento)

}
```

<a href="https://go.dev/play/p/UElj6uzNXhi">Code</a>