# JavaScript

## Estruturas de repetição ou laços de repetição

São comandos que mantém um código sendo executado até que uma condição de parada seja satisfeita.

### for

Um laço for é repetido até que a condição especificada seja falsa. Formado por três partes: inicialização, condição e incremento. A sintaxe é:

    for (expressaoInicial; condicao; incremento) {
       código aqui;
    }

### while

Uma declaração while executa suas instruções, desde que uma condição especificada seja avaliada como verdadeira. Funciona basicamente igual ao for, e é possível sempre trocar o for() por um while(). Escolhemos um ou outro pela clareza do que estamos fazendo. Geralmente preferimos utilizar o loop for() para interar com contadores e loops while() até que alguma condição mude (de true para false, por exemplo).

    while (condicao) {
       código aqui;
    }

Exemplos de código que só pode ser feito com while

```
let resposta = prompt('Escolha uma das opções a seguir: \n\r(1) Mensagem de paz \n\r(2) Mensagem de incentivo \n\r(3) Mensagem de guerra \n\r(s) Sair');

while (resposta !== 's') { //Enquanto a condição for satisfeita, ele entra no loop
    if (resposta === '1') {
        alert('#pas');
    } else if (resposta === '2') {
        alert('Gambatê!');
    } else if (resposta === '3') {
        alert('Se plante!');
    } else {
        alert('Opção desconhecida');
    }

    resposta = prompt('Escolha uma das opções a seguir: \n\r(1) Mensagem de paz \n\r(2) Mensagem de incentivo \n\r(3) Mensagem de guerra \n\r(s) Sair');
}
```

```
let enviado = false;
while (!enviado) { //while(enviado === false)
    //Enviando email
    // Meu codigo aqui
    enviado = enviarEmail(); //função de enviar email que retorna verdadeiro ou falso
}
```


### do-while

A instrução do-while repetirá até que a condição especificada seja falsa. O corpo é sempre executado pelo menos uma vez, independente da condição, pois primeiro ele faz do e depois testa a condição.

    do {
      código aqui;
    } while (condicao);


## Declarações complementares

### break

Quando você utiliza break, ele encerrará imediatamente o laço mais interno while, do-while, for, ou switch e transferirá o controle para a próxima instrução.

O exemplo a seguir percorre os elementos de um array até que ele encontre o índice do elemento que possui o valor contido em theValue:

    for (i = 0; i < a.length; i++) {
       if (a[i] == theValue) {
          break;
       }
    }

### continue

A declaração continue pode ser usada para reiniciar uma instrução while, do-while ou for. Quando você utiliza continue, ele encerrará a iteração atual mais interna de uma instrução while, do-while, ou for e continuará a execução do laço a partir da próxima iteração. Ao contrário da instrução break, continue não encerra a execução completa do laço. Em um laço while, ele voltará para a condição. Em um laço for, ele pulará para a expressão de incrementação.

O exemplo a seguir mostra um laço while utlizando continue que executará quando o valor de i for igual a 3.

    i = 0;
    n = 0;
    while (i < 5) {
       i++;
       if (i == 3) {
          continue;
       }
       n += i;
    }