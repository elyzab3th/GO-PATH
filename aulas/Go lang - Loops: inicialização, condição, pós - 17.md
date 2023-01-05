# 06 – Fluxo de Controle

- For
    - Inicialização, condição, pós
    - Ponto e vírgula?
    - gobyexample.com
    - Não existe while!

# Inicialização, condição, pós

```go
package main
import "fmt"
func main() {
The most basic type, with a single condition.

    i := 1
    for i <= 3 {
        fmt.Println(i)
        i = i + 1
    }
A classic initial/condition/after for loop.

    for j := 7; j <= 9; j++ {
        fmt.Println(j)
    }
for without a condition will loop repeatedly until you break out of the loop or return from the enclosing function.

    for {
        fmt.Println("loop")
        break
    }
You can also continue to the next iteration of the loop.

    for n := 0; n <= 5; n++ {
        if n%2 == 0 {
            continue
        }
        fmt.Println(n)
    }
}
```

# Ponto e vírgula `;`
Em `GO` o ponto e vírgula serve para por exemplo, definir o fim de cada instrução. Em vez de você digitar algo legível (`O que é recomendável`), podemos por exemplo usar `;` para juntar todo códugo em um linha só:

```go
package main; import "fmt"; func main() {for x := 13; x != 0; x++ {fmt.Println(x)}}
```

Quando você compila seu código o programa coloca/define automaticamente o `;` de cada instrução.

# Não existe while!
Em `GO` não existe `While`. Mais adiante veremos como substitui-lo