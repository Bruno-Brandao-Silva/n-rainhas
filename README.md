# Solução do Problema das N-Rainhas utilizando Algoritmos Inteligentes

Este repositório contém a implementação de soluções para o problema das N-Rainhas utilizando algoritmos inteligentes, desenvolvido como parte da disciplina de Inteligência Artificial do Curso de Engenharia de Computação na UTFPR.

## Algoritmos Implementados

### 1. Hill Climbing com Seleção do Melhor Vizinho

O algoritmo de *Hill Climbing* busca a solução movendo-se sempre na direção que maximiza o valor da função de avaliação, neste caso, minimizando o número de ataques entre as rainhas.

- **`HillClimbing_BestNeighborSelection.ipynb`**: Implementação do Hill Climbing com seleção do melhor vizinho.
  
  **Funções Principais:**
  - `State`: Representa o estado do tabuleiro com as posições das rainhas.
  - `evaluation`: Calcula o número de ataques entre as rainhas no estado atual.
  - `neighbor`: Gera o melhor vizinho ao mover cada rainha para uma posição que minimize o número de ataques.
  - `hill_climbing`: Implementa o algoritmo Hill Climbing.
  - `random_restart`: Implementa o Hill Climbing com reinicialização aleatória.
  - `simple_hill_climbing`: Versão simplificada do Hill Climbing.

### 2. Simulated Annealing (Recozimento Simulado)

O algoritmo de *Simulated Annealing* é uma técnica de otimização probabilística que permite escapar de ótimos locais e explorar mais do espaço de soluções.

- **`SimulatedAnnealing.ipynb`**: Implementação do Simulated Annealing para resolver o problema das N-Rainhas.

  **Funções Principais:**
  - `State`: Mesmo que na implementação do Hill Climbing.
  - `evaluation`: Função para calcular o número de ataques entre as rainhas no estado atual.
  - `neighbor`: Gera um vizinho aleatório e decide se deve aceitar ou não com base na função de temperatura.
  - `SimulatedAnnealing`: Implementação principal do Simulated Annealing com parâmetros configuráveis.

## Visualização

Ambos os notebooks fornecem funções para visualizar o tabuleiro de xadrez com as rainhas posicionadas após encontrar a solução. A visualização é feita utilizando `matplotlib` e `seaborn`.

## Uso

Para resolver o problema das N-Rainhas:

1. Execute as células nos notebooks `HillClimbing_BestNeighborSelection.ipynb` ou `SimulatedAnnealing.ipynb` após definir o estado inicial (posições das rainhas).
2. Os algoritmos encontrarão uma solução ou um ótimo local, dependendo da estratégia utilizada.
3. A solução será exibida graficamente mostrando o posicionamento das rainhas no tabuleiro.

Sinta-se à vontade para explorar e adaptar os algoritmos para diferentes tamanhos de tabuleiro ou experimentar com diferentes parâmetros de busca.
