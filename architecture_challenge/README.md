### Intro

Este repositório contém a proposta de uma arquitetura para a criação de um Data Lake. O desenho contempla um cenário hipótetico onde os dados teriam  origens diversas e deveriam ser disponibilizados no ambiente analítico para que os times de analystics e data science possam utilizá-los.

### Estrutura do repositório
- ````architecture.drawio````
- ````architecture.drawio.png````

### Arquitetura
![Label](/architecture_challenge/architecture.drawio.png)

- aquisição dos dados
    - de SGBD`s via CDC com Kafka
    - de SaaS como Hubspot, Salesforce e Zendesk via Kafka connectors específicos
    - de API`s diversas através de aplicações em Python
- armazenamento dos dados
    - Cloud Storage para armazenamento de dados estruturados e não estruturado
- tratamento dos dados
    - tratamento de dados via dbt sendo orquestrados pelo Airflow
- disponibilização dos dados
    - dados disponibilizados no BigQuery em arquitetura medallion: camadas bronce, silver e gold para análise
    - dados quentes do Cloud Storage disponíveis para modelos de Data Science

### Pontos fortes
- Desacoplamento dos sistemas origens
- Nessa arquitetura o Airflow não necessariamente precisaria ser gerenciado pela Google

### Pontos fracos
- A necessidade de Cloud Storage pode ser questionada: dados poderiam ser ingeridos diretamente na camada raw do BigQuery
