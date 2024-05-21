# IACD

# Programa de Classificação de Condições de Saúde

## Introdução
Este programa foi construído com o objetivo de determinar a capacidade de sobrevivência dos doentes 1 ano após o diagnóstico (por exemplo, “vive” ou “morre”). Para tal é necessário a utilização real da ciência de dados, realizar a limpeza de dados e avaliação de características até à inspeção visual e comunicação dos resultados, utilizando o conjunto de dados reais de doentes diagnosticados com carcinoma hepatocelular (CHC), recolhido no Centro Hospitalar e Universitário de Coimbra (CHUC) em Portugal. 

Com o desenvolvimento do pipeline foi necessário cumprir com algumas etapas: 
 - a análise exploratória
 - o pré-processamento dos dados
 - aplicação de técnicas de aprendizagem supervisionada (ML)
 - treinamento dos modelos
 - classificação, interpretação, avaliação e comparação do desempenho dos modelos utilizados


##

No que se refere à analise exploratória e ao pré-processamento
Para este programa foram utilizadas duas técnicas de aprendizagem supervisionada: KNN (K-Neares Neighbors) e DT (Decision Tree/Árvore de Decisão). 



A segunda tarefa prática consiste no desenvolvimento de um pipeline completo de ciência de dados, desde a análise exploratória
exploratória e o pré-processamento de dados até à aplicação de técnicas de aprendizagem supervisionada para classificação e
classificação e a respectiva avaliação de desempenho. Opcionalmente, o projeto pode também considerar a exploração de técnicas adicionais
técnicas adicionais, como clustering, tratamento de dados em falta ou desequilibrados, entre outras, para melhorar o
desempenho do sistema.

objetivo é abordar um caso de utilização real da ciência de dados, desde a limpeza de dados e avaliação de características até à
inspeção visual e comunicação dos resultados, utilizando o conjunto de dados do carcinoma hepatocelular (CHC). O conjunto de dados HCC
O conjunto de dados HCC foi recolhido no Centro Hospitalar e Universitário de Coimbra (CHUC) em Portugal e contém dados clínicos reais de
dados clínicos reais de pacientes diagnosticados com CHC. O principal objetivo deste projeto é desenvolver um pipeline de aprendizagem
capaz de determinar a capacidade de sobrevivência dos doentes 1 ano após o diagnóstico (por exemplo, “vive” ou “morre”).


## Dependências de Pacotes
- numpy
- pandas
- seaborn
- matplotlib
- scikit-learn

## Instruções
1. Clone este repositório em sua máquina local.
2. Verifique se você possui todos os pacotes necessários instalados. Você pode instalá-los usando o pip:

    ```
    pip install numpy pandas seaborn matplotlib scikit-learn
    ```
3. Coloque seu arquivo de conjunto de dados chamado `hcc_dataset.csv` no mesmo diretório que o programa.
4. Execute o programa executando o script Python.

## Estrutura do Programa
- `health_condition_classification.py`: Script Python contendo o programa.
- `hcc_dataset.csv`: Arquivo de conjunto de dados contendo os dados de condições de saúde.

## Uso
1. O programa carrega o conjunto de dados de `hcc_dataset.csv`.
2. Ele realiza pré-processamento de dados para lidar com valores ausentes e converter variáveis categóricas.
3. Análise exploratória de dados é realizada, incluindo visualização de distribuições de dados e correlações.
4. Dois modelos de classificação, KNN e Árvore de Decisão, são treinados e avaliados.
5. A comparação dos modelos é realizada com base em acurácia, precisão, recall/sensibilidade e F1-score.
6. Curvas de aprendizado e curvas ROC são plotadas para analisar o desempenho do modelo.

## Como Executar
1. Certifique-se de ter o Python instalado em seu sistema.
2. Clone o repositório.
3. Navegue até o diretório que contém o script e o conjunto de dados.
4. Execute o script usando o seguinte comando:

    ```
    python health_condition_classification.py
    ```

## Notas Adicionais
- O programa pressupõe que a última coluna do conjunto de dados é a variável alvo.
- Métricas de avaliação do modelo e visualizações são fornecidas para avaliar o desempenho dos modelos de classificação.
- Sinta-se à vontade para modificar o script de acordo com seu conjunto de dados específico e requisitos.

