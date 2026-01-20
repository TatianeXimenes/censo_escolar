# 🧠 Sistema de Inferência Fuzzy para Cálculo de Gorjeta

## Descrição
Este projeto implementa um sistema de inferência fuzzy para determinar o valor da gorjeta com base na qualidade da comida e no atendimento. Utiliza a biblioteca scikit-fuzzy para modelar variáveis linguísticas e simular a tomada de decisão humana ao calcular gorjetas.

## Objetivo
Simular o processo de decisão humana para calcular gorjetas considerando:
Qualidade da comida (ruim, boa, saborosa)
Serviço (ruim, aceitável, ótimo)
Gorjeta (baixa, média, alta)

## Tecnologias Utilizadas
Python 3
NumPy
scikit-fuzzy
Google Colab (ambiente de desenvolvimento original)

## Estrutura do Sistema
### Variáveis Linguísticas
Antecedentes (Entradas):
Qualidade da Comida (0-10)
ruim: Função de pertinência automática
boa: Função de pertinência automática
saborosa: Função de pertinência automática

Serviço (0-10)
ruim: Função de pertinência automática
aceitável: Função de pertinência automática
ótimo: Função de pertinência automática

Consequente (Saída):
Gorjeta (0-25%)
baixa: Função sigmoidal (sigmf)
média: Função Gaussiana (gaussmf)
alta: Função PI (pimf)

## Lógica de Inferência
Processo de Decisão:
Fuzzificação: Converter entradas numéricas em valores linguísticos
Avaliação de Regras: Aplicar regras fuzzy baseadas na qualidade e serviço
Agregação: Combinar resultados das regras
Defuzzificação: Converter resultado fuzzy em valor numérico (gorjeta)


##  Características do Projeto
- Implementadas:
Definição de variáveis linguísticas
Funções de pertinência personalizadas para gorjeta
Visualização dos conjuntos fuzzy
Modelagem do sistema de inferência

- Ajustes Realizados:
Alteração da taxa da qualidade para 0.5
Alteração da taxa do serviço para 0.5
Reconfiguração dos antecedentes

## Conceitos de IA Aplicados
1. Lógica Fuzzy
Conjuntos difusos vs. conjuntos crisp
Graus de pertinência (0 a 1)
Operadores fuzzy (AND, OR, NOT)

2. Sistemas de Inferência
Fuzzificação → Inferência → Defuzzificação
Base de regras linguísticas
Métodos de defuzzificação (centroide, máximo, etc.)

3. Aplicação em Problemas Reais
Modelagem de incerteza
Tomada de decisão com múltiplos fatores
Sistemas especialistas simples
