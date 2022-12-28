# Hello World! <img src="https://cdn.worldvectorlogo.com/logos/golang-gopher.svg" width="50" height="50">

<img src="https://user-images.githubusercontent.com/8325672/76652279-7cc88c00-6523-11ea-8cd1-247de96c7c69.png">

## Subtópicos

- Estrutura básica:
	- package main.
	- func main: é aqui que tudo começa, é aqui que tudo acaba.
	- import.
- Packages
	- Pacotes são coleções de funções pré-prontas (ou não) que você pode utilizar.
	- Notação: pacote.Identificador. Exemplo: fmt.Println()
	- Documentação: fmt.Println.
- Variáveis: "uma variável é um objeto (uma posição na memória) capaz de reter e representar um valor ou expressão."
- Variáveis não utilizadas? Não pode: _ nelas.
- ...funções variádicas.
- Lição principal: package main, func main, pacote.Identificador.

# Hello World

Uma tradição que se utiliza em uma nova linguagem de programação.

## Package main

O `package main` **define qual é o package principal do programa**. É nela que definimos e dizemos para ele onde ele deve começar.

## `func main`

Define a principal função do programa.

Essa função é responsável por ser o ponto de entrada do seu programa. Se você está construindo uma API ou um executável de linha de comando, você precisa ter uma função main , senão o compilador não sabe onde é o ponto de entrada do seu código e por isso não consegue gerar o executável.
