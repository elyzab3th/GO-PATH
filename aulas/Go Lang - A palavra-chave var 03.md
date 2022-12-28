# A palavra-chave var

## Subtópicos
- Variável declarada em um code block é undefined em outro
- Para variáveis com uma abrangência maior, package level scope, utilizamos `var`	
- Funciona em qualquer lugar
- Prestar atenção: chaves, colchetes, parênteses

# Variável declarada em um code block é undefined em outro

```go
package main

import ("fmt")

func main () {
	// A var y está declarada dentro do codeblock
	// Fora do code block ninguém enxerga ela (a var y).

	y := 10
	anything(y)

}

func anything (x int) {

	fmt.Println(x)

}

```

```go
package main

import ("fmt")

var y int = 10

func main () {
	// A var y está declarada dentro do codeblock
	// Fora do code block ninguém enxerga ela (a var y).
	anything(y)

}

func anything (x int) {

	fmt.Println(x)

}
```

#