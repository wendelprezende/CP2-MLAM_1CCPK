# Regressão Linear com PIB e Índice ABCR

## Integrantes:
Wendel Pedro - RM:573126
Daniel Alejandro - RM: 573075
Victor Hugo - RM: 573838
Arthur Araújo - RM: 573308

## Sobre o projeto

Este projeto investiga a relação entre a atividade econômica brasileira e o fluxo de veículos nas rodovias, utilizando o índice de volume do **PIB** e o **Índice ABCR de fluxo total de veículos**.

Foram utilizados dados de **2006 a 2025**, totalizando 20 anos completos em comum entre as duas bases.

## Dados utilizados

* **PIB:** dados do IBGE, obtidos na Tabela 1620 do SIDRA.
* **Índice ABCR:** série original de fluxo total de veículos no Brasil.

Os dados do PIB foram transformados de índices trimestrais para médias anuais. Os dados do ABCR foram transformados de índices mensais para médias anuais.

## Análise

Foi calculada a correlação entre os dois indicadores e construído um gráfico de dispersão para observar a relação entre PIB e fluxo de veículos.

Em seguida, foi treinado um modelo de **Regressão Linear** utilizando:

* **Variável de entrada (`X`):** `PIB_indice`
* **Variável estimada (`y`):** `ABCR_indice`
* **Treinamento:** 2006 a 2021
* **Teste:** 2022 a 2025

A divisão foi feita mantendo a ordem cronológica dos dados.

## Avaliação

O modelo foi avaliado utilizando as métricas:

* MAE (Mean Absolute Error)
* MSE (Mean Squared Error)
* R² (Coeficiente de Determinação)

Os resultados e gráficos estão disponíveis no notebook deste repositório.

## Tecnologias utilizadas

* Python
* Google Colab
* Pandas
* NumPy
* Matplotlib
* Scikit-learn

## Fontes

Presentes ao final do Notebook

## Conclusão

A análise busca verificar se existe uma relação linear entre a atividade econômica brasileira e o fluxo de veículos nas rodovias. Os resultados do notebook apresentam a correlação encontrada, o desempenho da regressão linear e uma comparação entre os valores observados e previstos.

Uma correlação elevada não significa, por si só, que o PIB cause diretamente alterações no fluxo de veículos, pois outros fatores também podem influenciar os indicadores.
