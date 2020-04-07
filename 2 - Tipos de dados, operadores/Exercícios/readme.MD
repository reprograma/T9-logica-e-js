**1.** Crie um algoritmo que dado um valor, calcule 5% de desconto e retorne o valor do desconto;
```
const preco = prompt('Digite o preço do item');

const desconto = preco * 0.05;

alert(`O valor do desconto é R$ ${desconto}`);
```

**2.** Crie um algoritmo que receba dois valores e exiba o resultado e o resto da divisão entre eles;
```
const num1 = prompt('Digite o primeiro valor');
const num2 = prompt('Digite o segundo valor');

const divisao = num1/num2;
const resto = num1%num2;

alert(`O valor da divisão é ${divisao} e o resto é ${resto}`);
```

**3.** Crie um algoritmo que calcule quantos dias o usuário viveu, baseado na idade (considere que a pessoa tenha a idade exata);

**4.** Faça um algoritmo que leia a idade de uma pessoa em dias e mostre-a em anos, meses e dias (assuma que todos os meses tem 30 dias, e todos os anos 365 dias);
```
const idadeEmDias = prompt('Digite quantos dias você já viveu');
const anos = parseInt(idadeEmDias/365);
const meses = parseInt((idadeEmDias%365)/30);
const dias = (idadeEmDias%365)%30;
alert(`Você viveu ${anos} anos, ${meses} meses e ${dias} dias`);

// Entrada: 900 dias
// Resultado: 2 anos, 5 meses, 20 dias
```
(TODAS AS QUESTÕES ABAIXO SÃO DE UM MUNDO SEM COVID-19. TODO MUNDO TAVA NA RUA. VOCÊS FIQUEM EM CASA)

**5.** Wenceslay gostaria de saber quantos litros por quilômetro, sua moto gastou em média. Ele sabe a distância rodada e a quantidade de litros de combustível que ele utilizou. Crie um algoritmo que mostre a Wenceslay qual a média de combustível gasto por quilômetro.

**6.** O gerente ficou louco! E agora não sabe quanto de desconto deu nos seus produtos para fazer o anúncio. Ele sabe o preço sem o desconto e com o desconto. Faça um algoritmo que calcule o percentual de desconto do produto.

**7.** Zenir é responsável por colocar a duração dos filmes no letreiro do cinema comunitário. A duração deve ser mostrada em minutos, mas alguns dos filmes exibidos vieram com a informação em horas e minutos. Ajude Zenir, ela tem mais o que fazer do que ficar fazendo conta.
```
const duracaoHoras = prompt('Duração em horas');
const duracaoMinutos = prompt('Duração em minutos');

let duracaoTotal = duracaoHoras*60;
duracaoTotal += parseInt(duracaoMinutos);

alert(`O filme possui a duração de ${duracaoTotal} minutos`);
```

**8.** Marisa trabalha como cronometrista numa maratona. 
O resultado da maratona é dado em horas, minutos e segundos.
Marisa precisa converter o resultado para segundos. Ajude Marisa.

```
// Em um minuto tem 60 segundos
// Em uma hora tem 60 minutos
// Em uma hora tem 3600 segundos (60 minutos vezes 60 segundos)

// Resolução 1
/* 
const horas = prompt('Digite a duração em horas');
let minutos = prompt('Digite a duração em minutos');
let segundos = prompt('Digite a duração em segundos');

minutos = (horas*60) + minutos; // ou minutos += horas*60;
segundos = minutos*60 + segundos; // ou segundos += minutos*60

alert(`A duração em segundos é ${segundos}`);
*/

// Resolução 2
/*
const horas = prompt('Digite a duração em horas');
const minutos = prompt('Digite a duração em minutos');
let segundos = prompt('Digite a duração em segundos');

segundos += horas*3600 + minutos*60;
// segundos = segundos + horas*3600 + minutos*60;

alert(`A duração em segundos é ${segundos}`);
*/
```

**9.** Marisa trabalha como cronometrista numa maratona. O resultado da maratona é dado em segundos. Marisa precisa converter o resultado para o formato hh:mm:ss. Ajude Marisa.
```
//Recebendo os dados do usuario
const resultadoSegundos = prompt('Digite o resultado em segundos');

//convertendo segundos para hora
const horas = parseInt(resultadoSegundos/3600);

//convertendo segundos para minuto
//  Divide o resto da conta de seg por 3600 (horas), por 60 para descobrir os minutos
const minutos = parseInt((resultadoSegundos%3600) /60) ;

const segundos = parseInt((resultadoSegundos%3600) %60) ;

alert(`${horas}:${minutos}:${segundos}`)
```