# Data pipelines with delta live tables on Databricks

Nesse projeto, foi construído um pipeline de dados no Databricks utizando Delta Live Tables, que é uma estrutura para o processamento de dados confiáveis e de fácil manutenção. As transformações são definidas no databricks notebook e podem ser realizadas utilizando Python ou SQL. O próprio Delta Live Tables gerencia totalmente a orquestração das tarefas.

## Medallion Architecture

Foi utilizada a Medallion Architecture para organizar os dados no data lakehouse, que melhora progressivamente a estrutura e qualidade dos dados à medida que avançam através de cada camada da arquitetura. Os três níveis são:

- Bronze: dados brutos, landing dos dados.
- Silver:  dados limpos e conformados.
- Gold: tabelas de nível de negócio, prontos para consumo.

## Pipeline Stream

Processamento dos dados em tempo real.

[![Stream](https://github.com/guimarczewski/data_pipeline_databricks/raw/main/images/complete_pipeline_stream.PNG)]()

## Pipeline Batch

Processamento dos dados em batch.

[![Batch](https://github.com/guimarczewski/data_pipeline_databricks/raw/main/images/complete_pipeline.PNG)]()

## Arquivos

O repositório possui dois diretórios, "dbc_files" e "notebooks", contendo os Databricks notebooks e os notebooks .ipynb, respectivamente. 

## Links
- https://www.youtube.com/watch?v=YuFG--utxaA - Live "Construção de um Pipeline de Dados no Databricks" do canal "Luan Moreno | Engenharia de Dados"
- https://www.databricks.com/product/delta-live-tables
- https://www.databricks.com/blog/2021/09/08/5-steps-to-implementing-intelligent-data-pipelines-with-delta-live-tables.html
- https://docs.databricks.com/workflows/delta-live-tables/delta-live-tables-ui.html
- https://www.databricks.com/glossary/medallion-architecture
