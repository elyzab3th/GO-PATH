# Tipo string (cadeias de caracteres)

- Strings são sequencias de bytes.
- Imutáveis.
- Uma string é um "slice of bytes" (ou, em português, uma fatia de bytes).
- Na prática:
    - %v %T
    - Raw string literals
    - Conversão para slice of bytes: []byte(x)
    - %#U, %#x
    - Go Playground: https://play.golang.org/p/dt2x1ies5b & https://play.golang.org/p/PpDnspiyA_7
- https://blog.golang.org/strings

# Strings são sequencias de bytes.
.. E essa cadeia de bytes são uma string

# Imutavel

Seu valor não pode ser mutável.

# Na prática:
## %v %T

```go
package main

import (
        "fmt"
        )

func main () {
        // A var y está declarada dentro do codeblock
        // Fora do code block ninguém enxerga ela (a var y).


        Hello := "Hello World"

        fmt.Printf("Value: %v \n Type: %T \n", Hello, Hello ) // %v = Value | %s

        //fmt.Printf("")
}

```


## Raw string literals
Raw string é a formatação de string em mais de uma linha:

```go
package main

import (
        "fmt"
        )

func main () {

        var content string = ` 
                HELLO FRIEND

                `
        fmt.Printf(content)
}

```


## Conversão para slice of bytes: []byte(x)

```go
package main


import (
        "fmt"
        )


func main () {

        var content string = "HELLO FRIEND"
        content_byte := []byte(content)

        fmt.Printf("%v %T", content_byte, content_byte,)

}

```

## %#U, %#x

Será abordado em breve...

