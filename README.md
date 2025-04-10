# Azure-Databricks-Exercises

git clone https://github.com/A-jota07/Azure-Databricks-Exercises.git

Azure-Databricks-Exercises/
├── README.md                         # Documentação geral do repositório
├── provisioning/                     # Instruções para provisionar recursos no Azure Databricks
│   ├── provision-databricks.md       # Passo a passo para provisionar o Azure Databricks
│   ├── create-cluster.md             # Instruções para criar um cluster no Databricks
├── spark-exercises/                  # Scripts e dados para análise com Apache Spark
│   ├── data-analysis/
│   │   ├── example-dataset.csv       # Conjunto de dados de exemplo para análise
│   │   ├── spark-analysis.py         # Script Python para análise Spark
│   ├── README.md                     # Explicação dos exercícios Spark
├── notebooks/                        # Notebooks do Databricks para análise de dados
│   ├── data-analysis-notebook.ipynb  # Notebook para análise de dados com Spark
├── resources/                        # Recursos e links úteis
│   ├── azure-databricks-setup-guide.md  # Guia de configuração inicial
│   ├── useful-links.md               # Links úteis para documentação e tutoriais

# Azure Databricks Exercises
Este repositório contém exercícios práticos para trabalhar com o Azure Databricks, incluindo provisionamento, criação de clusters e análise de dados com o Apache Spark.

## Conteúdo
- **Provisionamento**: Instruções para configurar o Azure Databricks.
- **Exercícios Spark**: Scripts e exemplos para análise de dados.
- **Notebooks**: Exemplos em notebooks Databricks.
- **Recursos**: Links úteis e guias.

## Pré-requisitos
- Conta no Azure.
- Conhecimento básico de Python e Apache Spark.

- # Provisionando o Azure Databricks
1. Acesse o portal Azure.
2. Crie um recurso `Azure Databricks`.
3. Configure o workspace e clique em `Criar`.

4. # Criando um Cluster
1. Acesse o workspace do Azure Databricks.
2. Vá até `Clusters` e clique em `Create Cluster`.
3. Escolha a configuração desejada e clique em `Criar`.

4. from pyspark.sql import SparkSession

# Inicializando o Spark
spark = SparkSession.builder.appName("Data Analysis").getOrCreate()

# Carregando o dataset
data = spark.read.csv("example-dataset.csv", header=True, inferSchema=True)

# Exemplo de operação: Mostrar estatísticas
data.describe().show()

# Links Úteis
- [Documentação do Azure Databricks](https://learn.microsoft.com/en-us/azure/databricks/)
- [Tutoriais de Apache Spark](https://spark.apache.org/docs/latest/)
