# JavaScript

## Controle de fluxo ou Estruturas condicionais

São comandos da linguagem que permitem desviar o fluxo do programa, dependendo de um teste.

### if
Use a declaração if para executar alguma declaração caso a condição lógica for verdadeira. Use a cláusula opcional else para executar alguma declaração caso a condição lógica for falsa.

Estrutura:

    if (<teste>) {
      <código a ser executado caso o teste seja verdadeiro>
    }

Exemplo:

    var x = 9;
    if (x > 10) {
      console.log("x é maior do que dez, corram para as colinas!");
    }
    console.log("Serei executado independente do if ser true ou false");

#### Usando if...else

    if (x <= 10) {
      console.log("Tudo certo, x é menor ou igual a 10.")
    } else {
      console.log("x é maior do que dez, corram para as colinas!");
    }

#### Usando else if

    if (x < 10) {
      console.log("Tudo certo, x é menor que 10.")
    } else if (x == 10) {
      console.log("x é igual a 10!")
    } else {
      console.log("x é maior do que dez, corram para as colinas!");
    }

### switch
O switch é uma estrutura para testes simples, muito usado quando temos que testar uma mesma condição diversas vezes, pois é mais legível do que uma cadeia de else if.

Uma declaração switch permite que um programa avalie uma expressão e tente associar o valor da expressão ao rótulo de um case. Se uma correspondência é encontrada, o programa executa a declaração associada.

A instrução break associada a cada cláusula case, garante que o programa sairá do switch assim que a declaração correspondente for executada e que continuará a execução a partir da declaração seguinte ao switch. Se a declaração break for omitida, o programa continua a execução a partir da próxima declaração dentro do switch.

Estrutura:

    switch (<expressao>) {
      case <valor>:
        <código a ser executado>
        [break;]
      case <valor2>:
        <código a ser executado>
        [break;]
      ...
      default:
        <código a ser executado>
        [break;]
    }

Exemplo:

    switch (tipofruta) {
      case "Laranja":
        console.log("O quilo da laranja está R$0,59.<br>");
        break;
      case "Maçã":
        console.log("O quilo da maçã está R$0,32.<br>");
        break;
      case "Banana":
        console.log("O quilo da banana está R$0,48.<br>");
        break;
      case "Cereja":
        console.log("O quilo da cereja está R$3,00.<br>");
        break;
      case "Manga":
        console.log("O quilo da manga está R$0,56.<br>");
        break;
      case "Mamão":
        console.log("O quilo do mamão está R$2,23.<br>");
        break;
      default:
        console.log("Desculpe, não temos " + tipofruta + ".<br>");
    }
    console.log("Gostaria de mais alguma coisa?<br>");