# Loops: nested loop (repetição hierárquica)

- For
    - Repetição hierárquica
    - Exemplos: relógio, calendário


# Repetição hierárquica

```go
package main

import "fmt"

func main() {

	for hours := 0; hours <= 24; hours++ {

		fmt.Println("Hour(s):", hours, "\n")

		for minutes := 0; minutes <= 60; minutes++ {

			fmt.Print("Seconds", minutes)

			fmt.Println("")

		}

	}

}
```

<a href="https://go.dev/play/p/E4LeiygjVIR">LINK to CODE</a>