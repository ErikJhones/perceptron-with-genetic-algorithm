# Perceptron com algortimo genético (AG)
Implementação do perceptron simples com AG.

A base de dados utilizado foi a flor de Iris. 
O código está em jupyter notebook.

## Base de dados
Flor de iris contendo 3 classes e 150 amostrar, 50 amostras por classe:
Classe: Virginica; Setosa; versicolor.
Características: Tamanho sépala, tamanho pétala, largura sépala, largura pétala.

## parâmetros do AG

CHANCE_MUT = .20     # Chance de mutação de um peso qualquer
CHANCE_CO = .25      # Chance de crossing over de um peso qualquer
NUM_INDIVIDUOS = 50  # Tamanho da população
NUM_MELHORES = 3     # Número de indivíduos que são mantidos de uma geração para a próxima
num_geracoes = 1000  # Quantidade de gerações feitas.

## Algumas informações:
As amostras de treino e teste foram normalizadas. Os pesos (que correspondem aos indivíduos)
são inicializados com valores entre -1 e 1. Em cada geração, os pesos podem ser mutados, onde
um determinado elemento dele pode mudar de valor num intervalo de -10 e 10. O valor desse intervalo
influencia diretamente a taxa de acerto do modelo. Valores muito altos, ou muito baixos, fazemo o modelo
não convergir tão rápido, ou mesmo não convergir.

## resultados: 
Utilizando 3 classes para classificação.
Para 20% das amostras separadas para teste, houve uma taxa de acerto de 80% nas predições.

# Caixeiro viajante com algortimo genético (AG)
Problema modelado com 7 cidade. Onde uma matriz 7x7 
com cada elemento correspondendo a distância da cidade i até j.

## parâmetros do AG

CHANCE_MUT = .20     # Chance de mutação de um peso qualquer
CHANCE_CO = .25      # Chance de crossing over de um peso qualquer
NUM_INDIVIDUOS = 50  # Tamanho da população
NUM_MELHORES = 3     # Número de indivíduos que são mantidos de uma geração para a próxima
num_geracoes = 1000  # Quantidade de gerações feitas.

## Algumas informações:
Cada individuo é um vetor com a sequência das cidade visitadas. A operação de mutação troca dois elementos
de um indivíduo de lugar com probabilidade de 20%. 

## resultados: 
Para o modelo utilizado, foi encontrado que a menor distância percorrida é de 125 e a melhor sequencia é: [2 1 5 4 3 0 6]
