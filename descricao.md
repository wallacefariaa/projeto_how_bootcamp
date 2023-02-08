# How Bootcamp - Engenharia de Dados

## Objetivo
O objetivo deste projeto é criar uma plataforma de análise de dados que permita aos usuários visualizar e analisar os gastos públicos obtidos através do portal da transparência. A plataforma permitirá que os usuários filtrem os dados por diferentes categorias (por exemplo, por departamento, por ano, por tipo de gasto, etc.), visualizem gráficos e tabelas e façam comparações entre diferentes períodos de tempo.

## Motivação
O setor público tem uma responsabilidade enorme em garantir que os recursos públicos sejam utilizados de forma eficiente e efetiva para atender às necessidades da sociedade. No entanto, muitas vezes, é difícil obter informações claras e precisas sobre como os recursos públicos são gastos. O objetivo deste projeto é fornecer insights sobre os gastos públicos de uma forma acessível e fácil de entender para a sociedade.

## Fontde de dados
A API do Portal da Transparência fornece diferentes endpoints para acessar diferentes tipos de dados, como por exemplo, informações sobre despesas, receitas, licitações, etc. O endpoint específico para despesas (/api-de-dados/despesas) será utilizado para coletar os dados para este projeto. Documentação: https://api.portaldatransparencia.gov.br/swagger-ui.html

## Serviços da AWS
- Lambda
- Event Bridge
- S3
- Athena
- Quicksight
