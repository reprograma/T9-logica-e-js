# JavaScript

## Tipos de Dados

Quando falamos em tipos de variáveis, temos as linguagens chamadas de fortemente tipadas e fracamente tipadas.

Em linguagens fortemente tipadas, definimos o tipo da variável no momento de sua criação. Exemplos de linguagens do tipo: Java; C; C++.

Em linguagens fracamente tipadas, não precisamos definir o tipo da variável, ela é tipada automaticamente quando recebe um valor. Exemplos de linguagens do tipo: Python; Ruby; Javascript.

O mais recente padrão ECMAScript define sete tipos de dados:

- Seis tipos de dados são os chamados primitivos:
    - Booleano. true e false.
    - null. Uma palavra-chave que indica valor nulo. Devido JavaScript ser case-sensitive, null não é o mesmo que Null, NULL, ou ainda outra variação.
    - undefined. Uma propriedade superior cujo valor é indefinido.
    - Number. 42 ou 3.14159.
    - String. "Howdy"
    - Symbol (novo em ECMAScript 6). Um tipo de dado cuja as instâncias são únicas e imutáveis.
- Object

### Booleano

Um booleano é um tipo de dado lógico que pode ter apenas um de dois valores possíveis: verdadeiro ou falso.

### null

Um valor nulo representa uma referência que aponta, geralmente de maneira intencional, para um objeto ou endereço de memória inválido ou inexistente. O significado do valor nulo varia entre as implementações das linguagens.

### undefined

Um valor primitivo automaticamente atribuído para variáveis que foram recentemente declaradas, mas não inicializadas.

### Number

No JavaScript, Number é um tipo de dado numérico.

### String

Em qualquer linguagem de programação, uma string é uma sequência de caracteres usados para representar texto.

### Symbol

O tipo de dados "symbol" é qualificado como um primitivo, onde valores desse tipo podem ser usados para fazer propriedades de objetos anônimos. Ele pode ser usado como chave de uma propriedade de objeto quando este tem a intenção de ser privada, para uso interno da classe ou do tipo do objeto em questão.

### Object

Objeto refere-se a uma estrutura de dados contendo dados e instruções para se trabalhar com estes dados. Objetos algumas vezes se referem a coisas do mundo real, por exemplo um objeto de carro ou um mapa em um jogo de corrida. JavaScript, Java, C++, Python, e Ruby são exemplos de Linguagens orientadas à objeto (object-oriented programming).

## Operadores

Os operadores vão nos permitir fazer operações matemáticas, de comparação e lógicas.

O JavaScript possui tanto operadores binários quanto unários e um operador ternário, o operador condicional. Um operador binário exige dois operandos, um antes do operador e outro depois:

> operando1 operador operando2

Um operador unário exige um único operando, seja antes ou depois do operador:

> operador operando
>
> operando operador

### Operadores de atribuição

Um operador de atribuição atribui um valor ao operando à sua esquerda baseado no valor do operando à direita. 

| Nome | Operador encurtado | Significado |
| ---- | ------------------ | ----------- |
| Atribuição | x = y | x = y |
| Atribuição de adição | x += y | x = x + y |
| Atribuição de subtração | x -= y | x = x - y |
| Atribuição de multiplicação | x *= y | x = x * y |
| Atribuição de divisão | x /= y | x = x / y |
| Atribuição de resto | x %= y | x = x % y |
| Atribuição exponencial | x **= y | x = x ** y |

### Operadores de comparação

Um operador de comparação compara seus operandos e retorna um valor lógico baseado em se a comparação é verdadeira. Os operandos podem ser numéricos, strings, lógicos ou objetos. Na maioria dos casos, se dois operandos não são do mesmo tipo, o JavaScript tenta convertê-los para um tipo apropriado. Isto geralmente resulta na realização de uma comparação numérica.

| Nome | Operador | Descrição |
| ---- | -------- | --------- |
| Igual | == | Retorna verdadeiro caso os operandos sejam iguais | 
| Não igual | != | Retorna verdadeiro caso os operandos não sejam iguais |
| Estritamente igual | === | Retorna verdadeiro caso os operandos sejam iguais e do mesmo tipo |
| Estritamente não igual | !== | Retorna verdadeiro caso os operandos não sejam iguais e/ou não sejam do mesmo tipo |
| Maior que | > | Retorna verdadeiro caso o operando da esquerda seja maior que o da direita |
| Maior que ou igual | >= | Retorna verdadeiro caso o operando da esquerda seja maior ou igual ao da direita |
| Menor que | < | Retorna verdadeiro caso o operando da esquerda seja menor que o da direita |
| Menor que ou igual| <= | Retorna verdadeiro caso o operando da esquerda seja menor ou igual ao da direita |

### Operadores aritméticos

Operadores aritméticos tomam valores numéricos (sejam literais ou variáveis) como seus operandos e retornam um único valor númerico. Os operadores aritméticos padrão são os de **soma (+)**, **subtração (-)**, **multiplicação (*)** e **divisão (/)**.

| Nome | Operador | Descrição |
| ---- | -------- | --------- |
| Módulo | % | Operador binário. Retorna o inteiro restante da divisão dos dois operandos |
| Incremento | ++ | Operador unário. Adiciona um ao seu operando. Se usado como operador prefixado (++x), retorna o valor de seu operando após a adição. Se usado como operador pósfixado (x++), retorna o valor de seu operando antes da adição |
| Decremento | -- | Operador unário. Subtrai um de seu operando. O valor de retorno é análogo àquele do operador de incremento | 
| Negação | - | Operador unário. Retorna a negação de seu operando |
| Adição | + | Operador unário. Tenta converter o operando em um número, sempre que possível |
| Operador de exponenciação | ** | Calcula a base elevada à potência do expoente |

### Operadores lógicos

| Nome | Operador | Utilização | Descrição |
| ---- | -------- | ---------- | --------- |
| AND | && | expr1 && expr2 | Retorna expr1 caso possa ser convertido para falso; senão, retorna expr2. Assim, quando utilizado com valores booleanos, && retorna verdadeiro caso ambos operandos sejam verdadeiros; caso contrário, retorna falso | 
| OU | &#124;&#124; | expr1 &#124;&#124; expr2 | Retorna expr1 caso possa ser convertido para verdadeiro; senão, retorna expr2. Assim, quando utilizado com valores booleanos, &#124;&#124; retorna verdadeiro caso ambos os operandos sejam verdadeiro; se ambos forem falsos, retorna falso |
| NOT | ! | !expr | Retorna falso caso o único operando possa ser convertido para verdadeiro; senão, retorna verdadeiro |

### Operadores de string

Além dos operadores de comparação, que podem ser utilizados em valores string, o operador de concatenação (+) concatena dois valores string, retornando outra string que é a união dos dois operandos. O operador de atribuição encurtado += também pode ser utilizado para concatenar strings.

### Operador condicional (ternário)

O operador condicional é o único operador JavaScript que utiliza três operandos. O operador pode ter um de dois valores baseados em uma condição. A sintaxe é:

> condicao ? valor1 : valor2

    var status = (idade >= 18) ? "adulto" : "menor de idade";
