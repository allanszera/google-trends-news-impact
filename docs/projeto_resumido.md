Documentação do Projeto: Google Trends x Notícias

1. Levantamento de Requisitos

Objetivo

Analisar se e como notícias do dia influenciam as tendências de busca no Google Brasil.

Requisitos Funcionais

Extrair tópicos em alta no Google Trends diariamente

Extrair manchetes e resumos de notícias nos mesmos períodos

Consolidar, cruzar e armazenar os dados em um data warehouse relacional

Disponibilizar dashboards e análises de correlação

Requisitos Não-Funcionais

O processo deve ser automatizável (ETL agendável)

Código versionado e documentado (GitHub)

Dados sensíveis protegidos e uso apenas educacional

Visualização acessível (dashboard web ou arquivo)

Premissas

As fontes (Google Trends, portais de notícia) estejam acessíveis

O volume diário de dados é pequeno (baixo custo de storage)

Não há necessidade de dados históricos prévios (mas pode ser estendido)

2. Fluxograma do Processo
![alt text](image.png)
+-----------+      +---------+      +---------------+      +--------------------+      +-------------+
|  Coleta   | ---> |  Raw    | ---> | Transformação | ---> | Data Warehouse     | ---> | Dashboard   |
| (Trends & |      |  Data   |      | (ETL)         |      | (PostgreSQL/SQLite)|      | Visualização|
|  News)    |      |         |      |               |      |                    |      |             |
+-----------+      +---------+      +---------------+      +--------------------+      +-------------+

Legenda:

Coleta: Scripts de extração (Google Trends e notícias)

Raw Data: Dados brutos salvos em arquivos (CSV/JSON) ou banco

Transformação: Scripts ETL

Data Warehouse: Banco relacional/modelo estrela

Dashboard: Visualização e análise

3. Etapas e Checklist do Projeto

1. Levantamento de Requisitos



2. Arquitetura e Design



3. Extração de Dados



4. Armazenamento Inicial



5. Transformação e Carga



6. Análise e Dashboard



7. Documentação



8. Publicação



Resumo Visual das Etapas

- Levantamento de Requisitos
- Arquitetura e Design
- Extração de Dados
- Armazenamento Inicial
- Transformação e Carga
- Análise e Dashboard
- Documentação
- Publicação

Observações

O fluxograma pode ser convertido para imagem visual, caso deseje para apresentações ou publicação.

Esta documentação pode ser estendida a cada etapa finalizada, mantendo o histórico do projeto.

