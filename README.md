
# Assignment 2 - Programa de Classificação de Condições de Saúde

## Introdução
Este programa foi construído com o objetivo de determinar a capacidade de sobrevivência dos doentes 1 ano após o diagnóstico (por exemplo, “Lives” ou “Dies”). Para tal é necessário a utilização real da ciência de dados, realizar a limpeza de dados e avaliação de características até à inspeção visual e comunicação dos resultados, utilizando o conjunto de dados reais de doentes diagnosticados com carcinoma hepatocelular (CHC), recolhido no Centro Hospitalar e Universitário de Coimbra (CHUC) em Portugal. 

Com o desenvolvimento do pipeline foi necessário cumprir com algumas etapas: 
 - **Análise exploratória**
 - **Pré-processamento dos dados**
 - **Aplicação de técnicas de aprendizagem supervisionada (ML)**
 - **Treinamento dos modelos**
 - **Classificação, interpretação, avaliação e comparação do desempenho dos modelos utilizados**


## Procedimento do Pipeline

### Análise Exploratória:
 - **Contagem de Dados e Características:** Foi verificado o número total de colunas (características) e linhas (dados) no conjunto de dados.
 - **Listagem das Características:** Foram listadas todas as colunas presentes no conjunto de dados.
 - **Identificão dos tipos de dados:** (por exemplo, numéricos, categóricos) de cada coluna utilizando ‘data.dtypes’.
 - **Contagem de Valores Ausentes:** Contou-se o número de ‘?’ em cada coluna.
 - **Substituição de Valores Ausentes por NaN:** Garantiu-se que os valores ausentes fossem representados como NaN no conjunto de dados.
 - **Análise estatística para cada característica do conjunto de dados:** realizou-se o cálculo de medidas como média, desvio padrão, máximo, mínimo, contagem de valores ausentes e ainda foi identificada a moda (valor mais frequente).
 - **Criação de uma tabela:** que contém os seguintes elementos para cada característica: o nome da característica, o tipo (numérico ou categórico), a média ou moda (dependendo do tipo de dados), o desvio padrão (expresso como uma percentagem da média), os valores máximo e mínimo para as características numéricas, e a contagem e percentagem de valores ausentes.
 - **Criação de histogramas:** para todas as categorias com o objetivo de compreender melhor a distribuição dos dados .

### Pré-Processamento:
 - **Transformação de dados:** Conversão de valores categóricos (ex: Yes, No) em numéricos(ex: 1,0).
 - **Remoção de variáveis:** Remoção de variavéis com base na análise de uma matriz de correlação. Uma menor correlação de uma variável com a variável alvo: ‘Class’, leva à remoção desta.
 - **Imputação de valores ausentes:** os valores em falta, representados por NaN, são substituídos pela Média da coluna (em colunas numéricas)
ou pela Moda da coluna (em colunas categóricas).


Para este programa foram utilizadas duas técnicas de aprendizagem supervisionada: KNN (K-Neares Neighbors) e DT (Decision Tree/Árvore de Decisão). 




## Dependências de Pacotes
- numpy
- pandas
- seaborn
- csv
- matplotlib
- scikit-learn


## Instruções

**1.** Descarregue o programa para um diretório vazio da máquina de análise. 
**2.** Verificar se os pacotes estão instalados. Se não estão, pode instalá-los usando o pip:
**3.** Mova o arquivo `hcc_dataset.csv` para o mesmo diretório onde o programa se encontra.
**4.** Execute todas as células jupyter de forma a inicializar o programa.


## Estrutura do Programa

- `health_condition_classification.ipynb`: Notebook Jupyter contendo o programa.
- `hcc_dataset.csv`: Arquivo de conjunto de dados contendo os dados de condições de saúde.

## Uso
1. O programa carrega o conjunto de dados de `hcc_dataset.csv`.
2. Ele é capaz de realizar o pré-processamento de dados para valores ausentes e converte-los em variáveis categóricas.
3. Análise exploratória de dados é realizada, incluindo visualização de distribuições de dados e correlações.
4. Dois modelos de classificação, KNN e Árvore de Decisão, são treinados e avaliados.
5. A comparação dos modelos é realizada com base em acurácia, precisão, recall/sensibilidade e F1-score.
6. Curvas de aprendizado e curvas ROC são plotadas para analisar o desempenho do modelo.


## Como Executar
1. Certifique-se de ter o Python e o Jupyter Notebook instalado em seu sistema.
2. Clone o repositório.
3. Navegue até o diretório que contém o script e o conjunto de dados.
4. Abra e execute o notebook health_condition_classification.ipynb no Jupyter Notebook.



## Notas Adicionais
- O programa pressupõe que a última coluna do conjunto de dados é a variável alvo.
- Métricas de avaliação do modelo e visualizações são fornecidas para avaliar o desempenho dos modelos de classificação.
- Sinta-se à vontade para modificar o script de acordo com seu conjunto de dados específico e requisitos.

