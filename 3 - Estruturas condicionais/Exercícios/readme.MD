### Exercícios simples

**1.** Faça um algoritmo que receba uma letra e determine se é uma vogal ou consoante (Faça duas versões deste código, uma utilizando if-else e outra utilizando switch-case);
```
// Solicitando a letra do usuário
const letra = prompt('Digite uma letra do alfabeto.');

// Resolvendo com switch
switch (letra) {
    case 'a': // Colocamos os cases seguidos um do outro para economizar
    case 'e': // código, já que todos eles terão a mesma mensagem
    case 'i':
    case 'o':
    case 'u': 
        alert(`A letra ${letra} é uma vogal`);
        break; // Se não houver o break, o alert dentro de default tbm será mostrado
    default:
        alert(`A letra ${letra} é uma consoante`);
}


// Resolvendo com if
// Verificando o valor da constante letra
// || (pipe) significa ou
// Meu if quer dizer "Se letra igual a 'a' OU letra igual a 'e' ..."
// if (letra === 'a'
//     || letra === 'e'
//     || letra === 'i'
//     || letra === 'o'
//     || letra === 'u') {
//     alert(`A letra ${letra} é uma vogal`);
// } else { // Qualquer outra letra que não passar no teste do if, é uma consoante
//     alert(`A letra ${letra} é uma consoante`);
// }
```

**2.** Escreva um código que receba um número (1-7) e devolva o dia da semana correspondente;
```
const diaSemana = parseInt(prompt('Digite o dia da semana [1-7]'));

switch (diaSemana) {
    case 1:
        alert(`Domingo`);
        break;
    case 2:
        alert(`Segunda-Feira`);
        break;
    case 3:
        alert(`Terça-Feira`);
        break;
    case 4:
        alert(`Quarta-Feira`);
        break;
    case 5:
        alert(`Quinta-Feira`);
        break;
    case 6:
        alert(`Sexta-Feira`);
        break        
    case 7:
        alert(`Sábado`);
        break;
    default:
        alert(`Dia de São Nunca`);
}
```

**3.** Escreva um código que receba um número (1-12), e diga qual mês e quantos dias ele tem;
```
let numeroMes = prompt('Digite o número do mês (1-12)');
numeroMes = parseInt(numeroMes);

switch (numeroMes) {
    case 1:
        alert(`Janeiro é o mês ${numeroMes} e possui 31 dias`);
        break;
    case 2:
        alert(`Fevereiro é o mês ${numeroMes} e possui 28 ou 29 dias`);
        break;
    case 3:
        alert(`Março é o mês ${numeroMes} e possui 31 dias`);
        break;
    case 4:
        alert(`Abril é o mês ${numeroMes} e possui 30 dias`);
        break;
    case 5:
        alert(`Maio é o mês ${numeroMes} e possui 31 dias`);
        break;
    case 6:
        alert(`Junho é o mês ${numeroMes} e possui 30 dias`);
        break;
    case 7:
        alert(`Julho é o mês ${numeroMes} e possui 31 dias`);
        break;
    case 8:
        alert(`Agosto é o mês ${numeroMes} e possui 31 dias`);
        break;
    case 9:
        alert(`Setembro é o mês ${numeroMes} e possui 30 dias`);
        break;
    case 10:
        alert(`Outubro é o mês ${numeroMes} e possui 31 dias`);
        break;
    case 11:
        alert(`Novembro é o mês ${numeroMes} e possui 30 dias`);
        break;
    case 12:
        alert(`Dezembro é o mês ${numeroMes} e possui 31 dias`);
        break;
    default:
        alert('Não é um mês conhecido');
}

// switch (numeroMes) {
//     case 2:
//         alert(`Fevereiro é o mês ${numeroMes} e possui 28 ou 29 dias`);
//         break;
//     case 4:
//     case 6:
//     case 9:
//     case 11: {
//         let nomeMes;
//         if (numeroMes === 4) {
//             nomeMes = 'Abril';
//         } else if (numeroMes === 6) {
//             nomeMes = 'Junho';
//         } else if (numeroMes === 9) {
//             nomeMes = 'Setembro';
//         } else {
//             nomeMes = 'Novembro';
//         }
//         alert(`${nomeMes} é o mês ${numeroMes} e possui 30 dias`);
//     }
//         break;
//     case 1:
//     case 3:
//     case 5:
//     case 7:
//     case 8:
//     case 10:
//     case 12: {
//         let nomeMes;
//         if (numeroMes === 1) {
//             nomeMes = 'Janeiro';
//         } else if (numeroMes === 3) {
//             nomeMes = 'Março';
//         } else if (numeroMes === 5) {
//             nomeMes = 'Maio';
//         } else if (numeroMes === 7) {
//             nomeMes = 'Julho';
//         } else if (numeroMes === 8) {
//             nomeMes = 'Agosto';
//         } else if (numeroMes === 10) {
//             nomeMes = 'Outubro';
//         } else {
//             nomeMes = 'Dezembro';
//         }
//         alert(`${nomeMes} é o mês ${numeroMes} e possui 31  dias`)
//     }
//         break;
//     default:
//         alert('Esse mês não faz parte do calendário gregoriano');
// }
```
**4.** Escreva um código que receba dois número e determine qual o maior entre eles;
```
const num1 = prompt('Digite o primeiro número:');
const num2 = prompt('Digite o segundo número:');

if (num1 > num2) {
    alert(`${num1} é maior que ${num2}`);
} else if (num1 === num2) {
    alert(`${num1} é igual a ${num2}`);
} else {
    alert(`${num2} é maior que ${num1}`);
}
```

**5.** Escreva um código que receba um número e determine se ele é par ou ímpar, e se é negativo ou positivo;

**6.** Escreva um código que receba três ângulos e determine se eles formam um triângulo válido.
Em um triângulo válido, a soma dos três ângulos é igual a 180º.

**7.**. Elaborar um algoritmo que lê 2 valores a e b e informa se são múltiplos ou não.

**8.** Crie um código que retorne a quantidade de pontos que seu time fez de acordo com o resultado do jogo. (Se o seu time venceu, ele recebe 3 pontos. Se o resultado foi empate, ele recebe 1 ponto. Se ele perdeu, não recebe nada.)

**9.** Elabore um programa que dada a idade de um nadador classifica-o em uma das seguintes categorias:
* Infantil A = 5 - 7 anos
* Infantil B = 8-10 anos
* Juvenil A = 11-13 anos
* Juvenil B = 14-17 anos
* Adulto = maiores de 18 anos

**10.** Faça um algoritmo que dado um número, retorne a classificação do ângulo. (Ângulo agudo: ângulo com medida maior que 0° menor que 90°; Ângulo reto: ângulo com medida igual a 90°; Ângulo obtuso: ângulo com medida maior que 90° e menor que 180°; Ângulo raso: ângulo com medida igual a 0° ou 180°; Ângulo Côncavo: ângulo com medida entre 180° e 360°; Ângulo completo: ângulo com medida igual a 360°).

### Exercícios [menos] simples 

**1.** Baseado na tabela abaixo, retorne a classificação de um produto.

| Código | Classificação |
| ------ | ------------- |
| 1 | Alimento não-perecível |
| 2,3 ou 4 | Alimento perecível |
| 5 ou 6 | Vestuário |
| 7 | Higiene Pessoal |
| 8 até 15 | Limpeza e Utensílios Domésticos |
| Qualquer outro código | Código inválido |

**2.** Baseado na tabela abaixo, escreva um algoritmo que leia o código do item adquirido pelo consumidor e a quantidade, calculando e mostrando o valor a pagar. A mensagem de retorno deve conter o produto, a quantidade e o valor total a pagar.

| Código | Produto | Preço Unitário (R$) |
| ----- | ------ | ----- |
| 100 | Cachorro quente | R$ 1,70 |
| 101 | Bauru Simples | R$ 2,30 |
| 102 | Bauru com ovo | R$ 2,60 |
| 103 | Hamburguer | R$ 2,40 |
| 104 | Cheeseburguer | R$ 2,50 |
| 105 | Refrigerante | R$ 1,00 |

**3.** Escrever um algoritmo que lê um valor em reais e calcula qual o menor número possível de notas de 100, 50, 10, 5 e 1 em que o valor lido pode ser decomposto. Escrever o valor lido e a relação de notas necessárias.

**4.** Uma empresa concederá um aumento de salário aos seus funcionários, variável de acordo com o cargo, conforme a tabela abaixo. Faça um algoritmo que leia o salário e o cargo de um funcionário e calcule o novo salário. Se o cargo do funcionário não estiver na tabela, ele deverá, então, receber 40% de aumento. Mostre o salário antigo, o novo salário e a diferença. 

| Código | Cargo | Percentual |
| ----- | ------ | ----- |
| 101 | Gerente | 10% |
| 102 | Engenheiro |	20% |
| 103 | Técnico | 30% |

**5.** Escrever um algoritmo que lê o número de identificação, as 3 notas obtidas por um aluno nas 3 verificações e a média dos exercícios que fazem parte da avaliação. Calcular a média de aproveitamento, usando a fórmula:

MA = (Nota1 + Nota2 x 2 + Nota3 x 3 + ME )/7

A atribuição de conceitos obedece a tabela abaixo:

|Média de Aproveitamento | Conceito |
| ------ | ----- |
|9,0 | A |
|7,5 e < 9,0 | B |
|6,0 e < 7,5 | C |
|4,0 e < 6,0 | D |
|< 4,0 | E |

O algoritmo deve escrever o número do aluno, suas notas, a média dos exercícios, a média de aproveitamento, o conceito correspondente e a mensagem: APROVADO se o conceito for A,B ou C e REPROVADO se o conceito for D ou E.