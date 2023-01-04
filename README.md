<img src="https://upload.wikimedia.org/wikipedia/commons/thumb/0/05/Go_Logo_Blue.svg/1200px-Go_Logo_Blue.svg.png">

# GO-PATH
I'm trying to learn this amazing programming languague by Google. Hope you enjoy with me ;) 

### Content: Brazilian - Portuguese

## Subtopics and Contents

 [LINK](https://github.com/vkorbes/aprendago/blob/master/OUTLINE.md)

**Hello World!** | [Go Lang - Hello World 01.md](https://github.com/leone-sh/GO-PATH/blob/main/aulas/Go%20Lang%20-%20Hello%20World%2001.md)

<details><summary>Content</summary>
<p>


- Estrutura básica:
  - package main.
  - func main: é aqui que tudo começa, é aqui que tudo acaba.
  - import
- Packages
  - Pacotes são coleções de funções pré-prontas (ou não) que você pode utilizar.
  - Notação: pacote.Identificador. Exemplo: fmt.Println()
  - Documentação: fmt.Println.


</p>
</details>	
	
	
#

**Operador curto de declaração** | [Operador curto de declaração 02.md](https://github.com/leone-sh/GO-PATH/blob/main/aulas/Operador%20curto%20de%20declara%C3%A7%C3%A3o%2002.md)

<details><summary>Content</summary>
<p>

- `:=` parece uma marmota (gopher) ou o punisher.
- Uso:
  - Tipagem automática
  - Só pode repetir se houverem variáveis novas
  - != do assignment operator (operador de atribuição)
  - Só funciona dentro de codeblocks
- Terminologia:
  - keywords (palavras-chave) são termos reservados
  - operadores, operandos
  - statement (declaração, afirmação) → uma linha de código, uma instrução que forma uma ação, formada de expressões
  - expressão -> qualquer coisa que "produz um resultado"
  - scope (abrangência)
    - package-level scope
- Lição principal:
    - := utilizado pra criar novas variáveis, dentro de code blocks
    - = para atribuir valores a variáveis já existentes

</p>
</details>
	
#

**A palavra-chave var** | [Go Lang - A palavra-chave var 03.md](https://github.com/leone-sh/GO-PATH/blob/main/aulas/Go%20Lang%20-%20A%20palavra-chave%20var%2003.md)

<details><summary>Content</summary>
<p>


- ariável declarada em um code block é undefined em outro
- Para variáveis com uma abrangência maior, package level scope, utilizamos `var`
- Funciona em qualquer lugar
- Prestar atenção: chaves, colchetes, parênteses

</p>
</details>
	
#

**Tipos em GO** | [Go Lang - Tipos em GO 04.md](https://github.com/leone-sh/GO-PATH/blob/main/aulas/Go%20Lang%20-%20Tipos%20em%20GO%2004.md)

<details><summary>Content</summary>
<p>

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

</p>
</details>
	
#

**Valor zero** | [golang Valor Zero 05.md](https://github.com/leone-sh/GO-PATH/blob/main/aulas/golang%20Valor%20Zero%2005.md)
  
<details><summary>Content</summary>
<p>
  
- Declaração vs. inicialização vs. atribuição de valor. Variáveis: caixas postais.
- O que é valor zero?
- Os zeros:
  - ints: 0
  - floats: 0.0
  - booleans: false
  - strings: ""
  - pointers, functions, interfaces, slices, channels, maps: nil
- Use := sempre que possível.
- Use var para package-level scope.
  
</p>
</details>
	
  #
  
  **O pacote fmt** | [Go Lang - O pacote fmt 06.md](https://github.com/leone-sh/GO-PATH/blob/main/aulas/Go%20Lang%20-%20O%20pacote%20fmt%2006.md)
  
  <details><summary>Content</summary>
<p>
  
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
   

</p>
</details>
	
   #
   
   **Criando seu próprio tipo** [Go Lang Criando seu próprio tipo - 07.md](https://github.com/leone-sh/GO-PATH/blob/main/aulas/Go%20Lang%20Criando%20seu%20pr%C3%B3prio%20tipo%20-%2007.md)
   
   
<details><summary>Content</summary>
<p>
   
- Revisando: tipos em Go são extremamente importantes. (Veremos mais quando chegarmos em métodos e interfaces.)
- Tem uma história que Bill Kennedy dizia que se um dia fizesse uma tattoo, ela diria "type is life."
- Grande parte dos aspectos mais avançados de Go dependem quase que exclusivamente de tipos.
- Como fundação para estas ferramentas, vamos aprender a declarar nossos próprios tipos.
- Revisando: tipos são fixos. Uma vez declarada uma variável como de um certo tipo, isso é imutável.
- type hotdog int → var b hotdog (main hotdog)
- Uma variável de tipo hotdog não pode ser atribuida com o valor de uma variável tipo int, mesmo que este seja o tipo subjacente de hotdog.

</p>
</details>
	
#

**Tipo booleano** | [Go Lang Tipo booleano - 08.md](https://github.com/leone-sh/GO-PATH/blob/main/aulas/Go%20Lang%20Tipo%20booleano%20-%2008.md)

<details><summary>Content</summary>
<p>

- Agora vamos explorar os tipos de maneira mais detalhada. golang.org/ref/spec. A começar pelo bool.
- O tipo bool é um tipo binário, que só pode conter um dos dois valores: true e false. (Verdadeiro ou falso, sim ou não, zero ou um, etc.)
- Sempre que você ver operadores relacionais (==, <=, >=, !=, <, >), o resultado da expressão será um valor booleano.
- Booleans são fundamentais nas tomadas de decisões em lógica condicional, declarações switch, declarações if, fluxo de controle, etc.
	- Na prática:
		- Zero value
		- Atribuindo um valor
		- Bool como resultado de operadores relacionais
- Go Playground: https://play.golang.org/p/7joj615nZw

</p>
</details>
	
#

**Como os computadores funcionam** | [Go Lang - Como os computadores funcionam 09.md](https://github.com/leone-sh/GO-PATH/blob/main/aulas/Go%20Lang%20-%20Como%20os%20computadores%20funcionam%2009.md)

<details><summary>Content</summary>
<p>

- Isso é importante pois daqui pra frente vamos falar de ints, bytes, e etc.
- Não é necessário um conhecimento a fundo mas é importante ter uma idéia de como as coisas funcionam por trás dos panos.
- https://docs.google.com/presentation/d/1aVytiGOBVDMISFW-ZARJ5iFY1osU2XJIw0hQpNICXm8/
- ASCII: https://en.wikipedia.org/wiki/ASCII
- Filme: Alan Turing, The Immitation Game.

</p>
</details>
	
#

**Tipos numéricos** | [Go Lang - Tipos Numericos 10.md](https://github.com/leone-sh/GO-PATH/blob/main/aulas/Go%20Lang%20-%20Tipos%20Numericos%2010.md)

<details><summary>Content</summary>
<p>

- int vs. float: Números inteiros vs. números com frações.
- golang.org/ref/spec → numeric types
- Integers:
    - Números inteiros
    - int & uint → “implementation-specific sizes”
    - Todos os tipos numéricos são distintos, exceto:
        - byte = uint8
        - rune = int32 (UTF8)
        (O código fonte da linguagem Go é sempre em UTF-8).
    - Tipos são únicos
        - Go é uma linguagem estática
        - int e int32 não são a mesma coisa
        - Para "misturá-los" é necessário conversão
    - Regra geral: use somente int
- Floating point:
    - Números racionais ou reais
    - Regra geral: use somente float64
- Na prática:
    - Defaults com :=
    - Tipagem com var
    - Dá pra colocar número com vírgula em tipo int?
    - Overflow
    - Go Playground: https://play.golang.org/p/dt2x1ies5b
- “implementation-specific sizes”? Runtime package. Word.
    - GOOS
    - GORUNTIME
    - [Get your architecture with GO](https://play.golang.org/p/1vp5DImIMM)

</p>
</details>

#

**Overflow** | [Go Lang - Overflow 11.md](https://github.com/leone-sh/GO-PATH/blob/main/aulas/Go%20Lang%20-%20Overflow%2011.md)


<details><summary>Content</summary>
<p>


- Um uint16, por exemplo, vai de 0 a 65535.
- Que acontece se a gente tentar usar 65536?
- Ou se a gente estiver em 65535 e tentar adicionar mais 1?
- Playground: https://play.golang.org/p/t7Z4m127F2t

</P>
</details>

#

**Strings** | [Go Lang - Strings 12.md](https://github.com/leone-sh/GO-PATH/blob/main/aulas/Go%20Lang%20-%20Strings%2012.md)

<details><summary>Content</summary>
<p>

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

</P>
</details>

#


**Sistemas Numéricos** | [Go Lang - Sistemas Numericos 13.md](https://github.com/leone-sh/GO-PATH/blob/main/aulas/Go%20Lang%20-%20Sistemas%20Numericos%2013.md)

<details><summary>Content</summary>
<p>

- Base-10: decimal, 0–9
- Base-2: binário, 0–1
- Base-16: hexadecimal, 0–f
- https://docs.google.com/document/d/1GqXpubhMMIr4Sy5xwgiPIDh5PGVmVpF2u0c9vDrvykE/
- Demonstração em Go.

</P>
</details>

#

**Constantes** | [Go Lang - Constantes 14.md](https://github.com/leone-sh/GO-PATH/blob/main/aulas/Go%20Lang%20-%20Constantes%2014.md)

<details><summary>Content</summary>
<p>

- São valores imutáveis.
- Podem ser tipadas ou não:
    - const oi = "Bom dia"
    - const oi string = "Bom dia"
- As não tipadas só terão um tipo atribuido a elas quando forem usadas.
    - Ex. qual o tipo de 42? int? uint? float64?
    - Ou seja, é uma flexibilidade conveniente.
- Na prática: int, float, string.
    - const x = y
    - const ( x = y )

</P>
</details>

#

