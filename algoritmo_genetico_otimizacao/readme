# Algoritmo Genético para Otimização de Função Não-Linear
## 📌 Descrição
Implementação de um Algoritmo Genético (AG) em Python para maximização de uma função matemática não-linear. O algoritmo simula o processo de evolução natural com seleção, crossover e mutação para encontrar valores ótimos que maximizam a função objetivo.

## Função Objetivo
Maximizar:
f(x, y) = x² + 3y + 4

Onde:
x ∈ [0.0, 51.0]
y ∈ [10.0, 51.0]

## Componentes do Algoritmo
1. Representação Genética
Cada indivíduo é representado por uma string de bits
8 bits por variável (total 16 bits para x e y)
Conversão de binário para real no intervalo especificado

2. Função de Fitness
Avalia a qualidade de cada solução
Quanto maior o valor da função, melhor o indivíduo

3. Operadores Genéticos
Seleção por Torneio (k=3): Seleciona os melhores indivíduos
Crossover de Um Ponto: Combina características dos pais
Mutação Bit a Bit: Introduz diversidade na população

4. Parâmetros do AG
n_iter = 150      # Número de gerações
n_populacao = 100 # Tamanho da população
r_cross = 0.9     # Taxa de crossover (90%)
r_mut = 0.0078    # Taxa de mutação adaptativa

## Como Funciona
- Inicialização: Gera população aleatória de strings binárias
- Avaliação: Calcula fitness para cada indivíduo
- Seleção: Escolhe pais via torneio
- Reprodução: Aplica crossover e mutação
- Substituição: Nova geração substitui a anterior
- Repetição: Continua por N gerações
- Resultado: Retorna o melhor indivíduo encontrado

## Resultados
O algoritmo busca o máximo global da função:
- Máximo teórico: f(51, 51) = 51² + 3×51 + 4 = 2764
- Algoritmo converge para valores próximos do ótimo
- Visualização: Melhoria progressiva ao longo das gerações

## Personalização

- Para Otimizar Outra Função
Modifique a função funcao_de_fitness:
def nova_funcao(x):
    return x[0]**3 + 2*x[1]**2 - 5*x[0]*x[1]

- Para Alterar os Limites
limites = [[-10, 10], [-5, 5], [0, 100]]  # Para 3 variáveis

- Para Ajustar Parâmetros
n_bits = 16        # Mais precisão
n_populacao = 200  # Maior diversidade
r_mut = 0.01       # Mais exploração

## Aplicações Práticas
Este algoritmo pode ser adaptado para:
- Otimização de parâmetros em modelos ML
- Problemas de roteamento (TSP)
- Projeto de engenharia (minimização de custos)
- Ajuste de hiperparâmetros de redes neurais

## Referências
Baseado no trabalho de Ankur Chattopadhyay
Conceitos de Computação Evolucionária
Otimização Heurística e Metaheurística

## Estrutura do Código
ag.py
├── funcao_de_fitness()    # Função objetivo
├── bit2real()             # Decodificação binária
├── selection()            # Seleção por torneio
├── crossover()            # Recombinação
├── mutacao()             # Operador de mutação
└── algoritmo_genetico()  # Loop principal


## Observações
- O algoritmo maximiza a função (para minimização, inverter o sinal)
- Taxa de mutação é adaptativa (1/(n_bits × n_variáveis))
- Elitismo implícito: Melhor indivíduo é preservado entre gerações

## Possíveis Melhorias
- Elitismo explícito para garantir preservação do melhor
- Diversas estratégias de seleção (roleta, ranking)
- Tipos de crossover (dois pontos, uniforme)
- Visualização gráfica da convergência
- Critérios de parada adaptativos



