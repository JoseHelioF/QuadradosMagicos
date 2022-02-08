## Quadrados Mágicos

### Algoritmo de busca por quadrados mágicos
#### Consiste em gerar um array com o tamanho equivalente ao quadrado do tamanho da ordem da matriz
#### Preencher com a sequência 1,2,...,n^2
#### Um método vai fazer a troca de uma posição do array por outra de forma aleatória
### Exemplo: posição 2 e 5
### [1,2,3,4,5,6,7,8,9]
### [1,5,3,4,2,6,7,8,9]
#### Um outro método logo em seguida vai escoler uma outra posição aleatória e inverter a parte final para o inicio do array
### Exemplo: posição 7
### [1,5,3,4,2,6,7,8,9]
### [8,9,1,5,3,4,2,6,7]

#### Aqui é feito uma soma de cada coluna, cada linha e cada uma das diagonais, cada soma é comparada com um valor chave, que depende da ordem do quadrado pela seguinte função: chave = n*(n^2+1)/2 onde n é a ordem do quadrado.
#### O módulo do valor de cada linha, coluna e diagonal é somada sendo esse o valor do array.
#### O processo é repetido em um loop e ao final é escolhido o array que representa a menor soma. Esse array passa pelo mesmo processo com objetivo encontrar o valor 0, que representa que um quadrado magico foi encontrado.