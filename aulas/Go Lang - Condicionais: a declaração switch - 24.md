# Condicionais: a declaração switch

- Switch:
    - pode avaliar uma expressão 
        - switch statement == case (value)
        - default switch statement == true (bool)
    - não há fall-through por padrão
    - criando fall-through
    - default
    - cases compostos

# `switch`
O switch é uma instrução condicional alternativa útil para comunicar as ações tomadas pelos seus programas em Go quando diante de diferentes opções. Tudo o que podemos escrever com a instrução switch também pode ser escrito com as instruções if .


```go
switch optstatement; optexpression{
case expression1: Statement..
case expression2: Statement..
...
default: Statement..
}
```

```go
package main
  
import "fmt"
  
func main() {
      
    // Switch statement with both 
    // optional statement, i.e, day:=4
    // and expression, i.e, day
    switch day:=4; day{
       case 1:
       		fmt.Println("Monday")
       case 2:
       		fmt.Println("Tuesday")
       case 3:
      		fmt.Println("Wednesday")
       case 4:
    		fmt.Println("Thursday")
       case 5:
       	 	fmt.Println("Friday")
       case 6:
       	 	fmt.Println("Saturday")
       case 7:
       	 	fmt.Println("Sunday")
       default: 
       	 	fmt.Println("Invalid")
   }
}     
```

```go
package main
  
import "fmt"
  
func main() {
    var value string = "five"
      
    // Switch statement without default statement
    // Multiple values in case statement
   switch value {
       case "one":
       fmt.Println("C#")
       case "two", "three":
       fmt.Println("Go")
       case "four", "five", "six":
       fmt.Println("Java")
   }  
}
```

<a href="https://go.dev/play/p/uN-xQPowcUW">My code example</a> 


<a href="https://go.dev/play/p/DRi6_Y94KIv">My code example</a>