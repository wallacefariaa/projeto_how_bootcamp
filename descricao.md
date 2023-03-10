# How Bootcamp - Engenharia de Dados

## Objetivo
O objetivo deste projeto é criar uma plataforma de análise de dados que permita aos usuários visualizar e analisar os gastos públicos obtidos através do portal da transparência. A plataforma permitirá que os usuários filtrem os dados por diferentes categorias (por exemplo, por departamento, por ano, por tipo de gasto, etc.), visualizem gráficos e tabelas e façam comparações entre diferentes períodos de tempo.

## Motivação
O setor público tem uma responsabilidade enorme em garantir que os recursos públicos sejam utilizados de forma eficiente e efetiva para atender às necessidades da sociedade. No entanto, muitas vezes, é difícil obter informações claras e precisas sobre como os recursos públicos são gastos. O objetivo deste projeto é fornecer insights sobre os gastos públicos de uma forma acessível e fácil de entender para a sociedade.

## Fonte de dados
A API do Portal da Transparência fornece diferentes endpoints para acessar diferentes tipos de dados, como por exemplo, informações sobre despesas, receitas, licitações, etc. O endpoint específico para despesas (/api-de-dados/despesas) será utilizado para coletar os dados para este projeto. Documentação: https://api.portaldatransparencia.gov.br/swagger-ui.html

## Métodos
- O Event Bridge acionará a Lambda para coletar diariamente os dados da API via script em python
- Os dados serão armazenados em um bucket no S3
- Através do Athena será possível consultar e fazer as análises dos dados salvos
- O Quicksight será usado para visualizar os resultados das análises feitas com o Athena

## Serviços
- Event Bridge
- Lambda
- S3
- Athena
- Quicksight

## Arquitetura

![image](https://user-images.githubusercontent.com/80830498/217415517-95695286-dc1e-4ddc-aae5-99b21cbe70dc.png)
