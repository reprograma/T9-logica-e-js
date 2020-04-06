## Operadores de atribuição

```
let x = 1;
const y = 3;

x += y; // x = x + y; 4
x -= y; // x = x - y; -2
x *= y; // x = x * y; 3
x /= y; // x = x / y; 0.33
x %= y; // x = x % y; 1
x **= y; // x = x**y; 1
```

## Operadores de comparação

```
const numero1 = 4;
const numero2 = 7; //numero
const numero3 = '7'; //string

// (numero1 == numero2)// == false // O valor é igual?
// (numero1 != numero2)// != true // O valor é diferente?
// (numero2 === numero3)// === false // O valor e o tipo é igual?
// (numero1 !== numero2) // !== true // O valor ou o tipo é diferente?
// (numero1 > numero2) // > false
// (numero1 >= numero2) // >= false
// (numero1 < numero2) // < true
// (numero1 <= numero2) // <= true
```

## Operadores lógicos

Eu vou à praia se fizer sol e eu tiver dinheiro. [AND]
Eu vou à praia se fizer sol ou eu tiver dinheiro. [OR]

P1 = se fizer sol
P2 = eu tiver dinheiro


|-----|  P1 |  P2 |  D  |
| AND |  F  |  V  |  F  |
| AND |  V  |  F  |  F  |
| AND |  V  |  V  |  V  |
| AND |  F  |  F  |  F  |
| OR  |  F  |  V  |  V  |
| OR  |  V  |  F  |  V  |
| OR  |  V  |  V  |  V  |
| OR  |  F  |  F  |  F  |