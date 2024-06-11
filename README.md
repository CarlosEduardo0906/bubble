# bubble
link video
https://www.youtube.com/watch?v=0z3Dkl9EUEY&ab_channel=%23devPreta
pesquisa por nome
Algoritmo de ordenação Bubble Sort - Javascript #devpreta


codigo 


function bubbleSort() {
    const arrayNumbers = [5, 2, 4, 1]; // os numeros recebidos para o sort
    let isChange; // variavel checa se uma troca foi feita
    do { // do while pois vai ter uma condição de true ou false, pra saber se foi trocada ou não a variavel
        isChange = false; // valor falso para troca já que não houve nenhuma
        
        for (let i = 0; i < arrayNumbers.length - 1; i++) { // começa pela variavel i que tem valor de 0 e o i tem q ser menor q o array.length que é o maior tamanho do array 
            if (arrayNumbers[i] > arrayNumbers[i + 1]) { // o valor contido na posição x é maior do que o valor contido na posição 1? mudar x por i
                const temp = arrayNumbers[i]; // guarda o maior valor (ex 5)
                arrayNumbers[i] = arrayNumbers[i + 1]; // troca o valor de 5 pelo valor de 2
                arrayNumbers[i + 1] = temp; // o valor que esta com 2 agora recebe 5
                
                isChange = true; // variavel verdadeira já que teve a troca
            }
        }
    } while (isChange);
    return arrayNumbers;
}

console.log(bubbleSort());
