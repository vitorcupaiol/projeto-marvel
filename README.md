# Projeto de Pipeline dos filmes da Marvel com Delta Lake (Databricks e PySpark)

Este projeto demonstra a construção de um pipeline de dados no Databricks utilizando a arquitetura Lakehouse com Delta Lake. Ele simula a ingestão, transformação e análise de dados dos filmes da Marvel a partir de arquivos CSV.

## Tecnologias Utilizadas

- Databricks (Community Edition)
- PySpark
- Delta Lake
- Lakehouse Architecture (Bronze, Silver, Gold)
- CSV como fonte de dados

## Estrutura do Projeto
projeto-marvel/
├── notebooks/
│ ├── 01_ingestion_bronze_BoxOffice_Performance.ipynb
│ ├── 01_ingestion_bronze_ListAllCharacters.ipynb
│ ├── 01_ingestion_bronze_Marvel_Movies.ipynb
│ ├── 01_ingestion_bronze_Phases.ipynb
│ ├── 01_ingestion_bronze_Public_Response.ipynb
│ ├── 02_transformation_silver_BoxOffice.ipynb
│ ├── 02_transformation_silver_Characters.ipynb
│ ├── 02_transformation_silver_Marvel_Movies.ipynb
│ ├── 02_transformation_silver_Phases.ipynb
│ ├── 02_transformation_silver_Public_Response.ipynb
│ ├── 03_analysis_gold_Marvel_Movies.ipynb
├── dados-exemplo/
│ └── Marvel_Movies.csv
│ └── phases.csv
│ └── list_all_characters.csv
│ └── public_response.csv
│ └── BoxOffice_Performance.csv
├── images/
│ └── arquitetura.png
└── README.md


## Visualização
Use o comando display(df_gold) no Databricks para visualizar dashboards interativos com gráficos de barras, pizza e tabelas.

## Autor
Desenvolvido por Vitor Oliveira Cupaiol, como parte de um portfólio de engenharia de dados com foco em Databricks, Delta Lake e PySpark.

## Observações
O projeto pode ser executado no Databricks Community Edition gratuitamente.
A estrutura pode ser expandida com uso de ferramentas como Apache Airflow, DBT, ou ingestão via streaming (Kafka, Auto Loader, etc).
