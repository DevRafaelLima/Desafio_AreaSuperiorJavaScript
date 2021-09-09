/*
Leia um caractere maiúsculo, que indica uma operação que deve ser realizada e uma 
matriz M[12][12]. Em seguida, calcule e mostre a soma ou a média considerando somente 
aqueles elementos que estão na área superior da matriz, conforme ilustrado abaixo 
(área verde).


Entrada
A primeira linha de entrada contem um único caractere Maiúsculo O ('S' ou 'M'), 
indicando a operação (Soma ou Média) que deverá ser realizada com os elementos da 
matriz. Seguem 144 valores com ponto flutuante de dupla precisão que compõem a matriz.

Saída
Imprima o resultado solicitado (a soma ou média), com 1 casa após o ponto decimal.
*/

// a função gets é implementada dentro do sistema para ler as entradas(inputs) dos dados
// Abaixo segue um exemplo de código que você pode ou não utilizar

const isSum = gets();

const xL = 12,
  yL = 12;
  
const matriz = new Array(12)
let sum = 0.0,
  av = 0.0;

for (l/ let x = 0; x < 12; x++   ) {
  matriz[x] = new Array(12)
  for (let y = 0; y < 12; y++   ) {
   // const i = Number(gets());
    matriz[x][y] = Number(gets());
    
  }
}
  
for ( let x = 0; x <= 4; x++   ) {
  for (let y = 0; y<= 10-x; y++  ) {
   
    if(y > x && y< 12-x-1){
      sum+=matriz[x][y]
    } 
    
  }
}

av = sum/30
if(isSum === "S"){
  console.log( sum.toFixed(1));  
} else if(isSum === "M"){
  console.log(av.toFixed(1))
}
