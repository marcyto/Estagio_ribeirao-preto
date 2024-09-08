# Estagio_ribeirao-preto

Questões realizadas e resolvidas com Javascript

1 - Fibonnaci 

function Fibonacci(numero) {
    let a = 0, b = 1, next = 0;
    if (numero === 0 || numero === 1) return true;
    while (next < numero) {
        next = a + b;
        a = b;
        b = next;
    }
    return next === numero;
}

let number = 21; //numero teste
if (Fibonacci(number)) {
    console.log(`${number} pertence à sequência de Fibonacci.`);
} else {
    console.log(`${number} não pertence à sequência de Fibonacci.`);
}

2 - existe A na string?

function existeA(str) {
    let count = 0;
    for (let i = 0; i < str.length; i++) {
        if (str[i].toLowerCase() === 'a') {
            count++;
        }
    }
    return count;
}

let inputString = "Abracadabra"; // String de teste
let count = existeA(inputString);

if (count > 0) {
    console.log(`A letra 'a' aparece ${count} vezes na string.`);
} else {
    console.log("A letra 'a' não aparece na string.");
}


3 - Valor da Var Soma

let INDICE = 12, SOMA = 0, K = 1;
while (K < INDICE) {
    K = K + 1;
    SOMA = SOMA + K;
}
console.log(SOMA); 

Resultado de SOMA = 78

4 - 

a) 1, 3, 5, 7, 9
b) 2, 4, 8, 16, 32, 64, 128
c) 0, 1, 4, 9, 16, 25, 36, 49
d) 4, 16, 36, 64, 100
e) 1, 1, 2, 3, 5, 8, 13 
f) 2, 10, 12, 16, 17, 18, 19, 20

5 - 

1 - Ligue o primeiro interruptor e deixe-o ligado por alguns minutos.
2 - Desligue o primeiro interruptor e ligue o segundo.
3 - Vá até a sala das lâmpadas.
A lâmpada que está acesa corresponde ao segundo interruptor.
A lâmpada que está quente, mas apagada, corresponde ao primeiro interruptor.
A lâmpada que está apagada e fria corresponde ao terceiro interruptor.

Dessa forma é possível identificar os três interruptores e suas respectivas lampadas.

