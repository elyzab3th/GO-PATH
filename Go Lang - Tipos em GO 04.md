# Explorando tipos

# Subtópicos

- Tipos em Go são extremamente importantes. (Veremos mais quando chegarmos em métodos e interfaces.)
- Tipos em Go são estáticos.
- Ao declarar uma variável para conter valores de um certo tipo, essa variável só poderá conter valores desse tipo.
- O tipo pode ser deduzido pelo compilador:
	- x := 10
	- var y = "a tia do batima"
- Ou pode ser declarado especificamente:
	- var w string = "isso é uma string"
	- var z int = 15
	- na declaração var z int com package scope, atribuição z = 15 no codeblock (somente)
- Tipos de dados primitivos: disponíveis na linguagem nativamente como blocos básicos de construção
	- int, string, bool
- Tipos de dados compostos: são tipos compostos de tipos primitivos, e criados pelo usuário
- slice, array, struct, map
- O ato de definir, criar, estruturar tipos compostos chama-se composição. Veremos muito disso futuramente.


#

- Tipos em Go são extremamente importantes. (Veremos mais quando chegarmos em métodos e interfaces.)

# Tipos em Go são estáticos.

Por exemplo, você delcara uma variável `x` como um `int`, ela sempre será `int`. Ao declarar uma variável para conter valores de um certo tipo, essa variável só poderá conter valores desse tipo.


```go
package main

import ("fmt")

var x int = 10

func main () {

	x := "Text" // A estática do GO não deixará isso acontecer
}
```

- O tipo pode ser deduzido pelo compilador:

```go
x := 10 // Quando se declara uma variável como essa, o compilador é responsável por deduzir seu tipo
var y = "a tia do batima" // Aqui é o mesmo caso
```


- Tipos de dados primitivos: disponíveis na linguagem nativamente como blocos básicos de construção int, string, bool

- Tipos de dados compostos: são tipos compostos de tipos primitivos, e criados pelo usuário (`slice`, `array`, `struct`, `map`)

- O ato de definir, criar, estruturar tipos compostos chama-se composição. Veremos muito disso futuramente.


# Ao declarar uma variável para conter valores de um certo tipo, essa variável só poderá conter valores desse tipo.

Se você declara uma variável do tipo `int` e quer mudar para `string` por exemplo, não será possível pois o `GO` não deixará.