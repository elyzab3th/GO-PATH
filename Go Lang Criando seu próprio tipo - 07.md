# Criando seu próprio tipo



# Subtópicos

- Revisando: tipos em Go são extremamente importantes. (Veremos mais quando chegarmos em métodos e interfaces.)
- Tem uma história que Bill Kennedy dizia que se um dia fizesse uma tattoo, ela diria "type is life."
- Grande parte dos aspectos mais avançados de Go dependem quase que exclusivamente de tipos.
- Como fundação para estas ferramentas, vamos aprender a declarar nossos próprios tipos.
- Revisando: tipos são fixos. Uma vez declarada uma variável como de um certo tipo, isso é imutável.
- type hotdog int → var b hotdog (main hotdog)
- Uma variável de tipo hotdog não pode ser atribuida com o valor de uma variável tipo int, mesmo que este seja o tipo subjacente de hotdog.

```go
package main

import "fmt"

type x int
var x


func main() {

				fmt.Prinf(" %T \n", x)


}
```

# Declarando seus próprios tipos em `GO`
Em `Go` podemos definir nossos próprios tipos customizáveis. Fazemos isso através de um tipo `subjacente` (Algo que vem por trás como base):

```go
package main

import "fmt"

type hotdog float64 // O tipo base do tipo hotdog é int

var b hotdog
var c int

func main() {

	fmt.Printf("%T, \n", b)

}

```

#

```go
package main

import "fmt"

type IsDog bool

var Edgar IsDog

func main() {

	fmt.Printf("%T", Edgar)

}
```