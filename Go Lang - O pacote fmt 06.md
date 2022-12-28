# O pacote fmt

## Subtópicos

 - Setup: strings, ints, bools.
 - Strings: interpreted string literals vs. raw string literals.
	- Rune literals.
	- Em ciência da computação, um literal é uma notação para representar um valor fixo no código fonte.
 - Format printing: documentação.
	- Grupo #1: Print -> standard out
		- func Print(a ...interface{}) (n int, err error)
		- func Println(a ...interface{}) (n int, err error)
		- func Printf(format string, a ...interface{}) (n int, err error)
			- Format verbs. (%v %T)
	- Grupo #2: Print -> string, pode ser usado como variável
		- func Sprint(a ...interface{}) string
		- func Sprintf(format string, a ...interface{}) string
		- func Sprintln(a ...interface{}) string
	- Grupo #3: Print -> file, writer interface, e.g. arquivo ou resposta de servidor
		- func Fprint(w io.Writer, a ...interface{}) (n int, err error)
		- func Fprintf(w io.Writer, format string, a ...interface{}) (n int, err error)
		- func Fprintln(w io.Writer, a ...interface{}) (n int, err error)

# Strings: interpreted string literals vs. raw string literals.

Em ciência da computação, um literal é uma notação para representar um valor fixo no código fonte.

Um `interpreted string literals` é uma string que interpreta caractere especiais.

```go
package main

import "fmt"

func main() {

	ip := "IP \n 192.168.1.12" //  interpreted string

	ip_raw := `"IP: \n 192.168.1.12"`

	fmt.Println(ip)

	fmt.Println(ip_raw)

}
```

# Format printing: documentação.

## Grupo #1: Print -> standard out
### func Print(a …interface{}) (n int, err error)