# IACD

# Programa de Classificação de Condições de Saúde

## Introdução
Este programa foi projetado para classificar condições de saúde com base em um conjunto de dados fornecido. Ele fornece funcionalidades para pré-processamento de dados, análise exploratória de dados, treinamento de modelo, avaliação e comparação entre dois modelos: K-Vizinhos Mais Próximos (KNN) e Árvore de Decisão.

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

