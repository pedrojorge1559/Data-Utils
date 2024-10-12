# Descrição dos Módulos

## `utils.py`
Este módulo fornece funções utilitárias para manipulação de objetos em Python, com foco em serialização e deserialização usando o `pickle`. As principais funções incluem:

- **`save_object(file_path, object_to_save)`**: Salva um objeto Python em um arquivo binário, criando o diretório se necessário. Utiliza a serialização do `pickle` para armazenar o objeto de forma persistente.
  
- **`load_object(file_path)`**: Carrega um objeto Python de um arquivo binário, utilizando a deserialização do `pickle`. Retorna o objeto carregado.

**Nota**: O uso do `pickle` deve ser feito com cautela, especialmente ao carregar dados de fontes não confiáveis, devido a potenciais riscos de segurança.

---

## `eda_utils.py`
Este módulo contém funções para realizar Análise Exploratória de Dados (EDA) e visualização. As principais funções incluem:

- **`eda_utils(data)`**: Exibe informações básicas sobre o DataFrame, incluindo as primeiras e últimas linhas, informações gerais, estatísticas descritivas, forma, colunas e tipos de dados.

- **`plot_missing_values(data)`**: Plota um gráfico de barras mostrando a quantidade de valores ausentes em cada coluna do DataFrame.

- **`analysis_plots(data, features, ...)`**: Gera gráficos para análise univariada e bivariada, incluindo histogramas, gráficos de barras e boxplots, com várias opções de personalização.

- **`check_outliers(data, features, visualize=False)`**: Identifica e calcula outliers nas características especificadas usando o método do Intervalo Interquartil (IQR). Oferece a opção de visualizar os outliers em um boxplot.

---

# Module Description

## `utils.py`
This module provides utility functions for handling Python objects, focusing on serialization and deserialization using `pickle`. The main functions include:

- **`save_object(file_path, object_to_save)`**: Saves a Python object to a binary file, creating the directory if necessary. It uses `pickle` serialization to persistently store the object.
  
- **`load_object(file_path)`**: Loads a Python object from a binary file using `pickle` deserialization. It returns the loaded object.

**Note**: The use of `pickle` should be done with caution, especially when loading data from untrusted sources, due to potential security risks.

---

## `eda_utils.py`
This module contains functions for performing Exploratory Data Analysis (EDA) and visualization. The main functions include:

- **`eda_utils(data)`**: Displays basic information about the DataFrame, including the first and last rows, general information, descriptive statistics, shape, columns, and data types.

- **`plot_missing_values(data)`**: Plots a bar chart showing the number of missing values in each column of the DataFrame.

- **`analysis_plots(data, features, ...)`**: Generates plots for univariate and bivariate analysis, including histograms, bar charts, and boxplots, with various customization options.

- **`check_outliers(data, features, visualize=False)`**: Identifies and calculates outliers in the specified features using the Interquartile Range (IQR) method. It offers the option to visualize the outliers in a boxplot.
