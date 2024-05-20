# Criação de modelos de Machine Learning para previsão e prevenção de doenças

Etapa de desenvolvimento de codigo para tratamento dos dados e técnicas de `Machine Learning` para diagnóstico da doença câncer e tambem toda a implementação da arquitetura medallion para armazenamento dos datasets na cloud `Azure`

## Linguagens e ferramentas utilizadas para a criação desse projeto
- Azure
- Databricks
- Azure Data Lake Storage Gen2
- Python
- Spark
- PySpark
- Pandas
- Bibliotecas de aprendizado de maquina

## Arquitetura do Projeto
O projeto utiliza a arquitetura medallion trazendo as camadas `bronze`, `silver` e `gold` para armazenamento 

![arquitetura esboço](https://github.com/thiagothr/Machine_Learning_TCC/assets/72639507/bfa75e8e-b384-4f0c-9d0f-d906a03f7cdb)


antes de tudo foi criado recursos no ambiente da `Azure` para conseguirmos presseguir com todo o armazenamento na nuvem. Depois de todos os recuros criados, criamos o armazenamento no storage account utilizando o `Data Lake Storage Gen 2`
e fizemos a criação das camadas `bronze`, `silver` e `gold`.

![Captura de tela 2024-05-19 204724](https://github.com/thiagothr/Machine_Learning_TCC/assets/72639507/98e13085-85fc-43bb-8902-6bec23d8eefb)

Após a criação das camadas fizemos o upload dos datasets `Cancer_Data.csv` e `Dados_dummies.csv` para a cada `Bronze` conhecida como camada `Raw` onde todo os dados brutos vão ser armazenados nessa camada para ser enviada ao `Databricks`
