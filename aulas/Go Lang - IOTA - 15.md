### Iota

- golang.org/ref/spec
- Numa declaração de constantes, o identificador iota representa números sequenciais.
- Na prática.
    - iota, iota + 1, a = iota b c, reinicia em cada const, _
- Go Playground: https://play.golang.org/p/eSrwoQjuYR

EXEMPLOS:

```go
package main

import "fmt"

const (
	a = iota
	b = iota
	c = iota
	d = iota
	e = iota
	f = iota
	g = iota
	h = iota
	i = iota
	j = iota
	k = iota
)

func main() {

	fmt.Println(a, b, c, d, e, f, g, h, i, j, k)

}

	// OUTPUT: 0 1 2 3 4 5 6 7 8 9 10

```

```go
package main

import "fmt"

const (
	a = iota
	b = iota * 2
	c = iota
	d = iota
	e = iota
	f = iota
	g = iota
	h = iota
	i = iota
	j = iota
	k = iota
)

func main() {

	fmt.Println(a, b, c, d, e, f, g, h, i, j, k)

}

```