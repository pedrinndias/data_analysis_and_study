# Relatório de Análise da Base de Dados

## Metadados Básicos

- **Total de Entradas**: 5293
- **Total de Colunas**: 399

## Sumário das Colunas

| Coluna                                                                                                                            | Tipo    |   Valores Únicos |   Valores Ausentes |   % Ausentes |
|:----------------------------------------------------------------------------------------------------------------------------------|:--------|-----------------:|-------------------:|-------------:|
| id                                                                                                                                | object  |             5293 |                  0 |         0    |
| Idade                                                                                                                             | int64   |               53 |                  0 |         0    |
| Faixa idade                                                                                                                       | object  |                9 |                  0 |         0    |
| Genero                                                                                                                            | object  |                4 |                  0 |         0    |
| Cor/raca/etnia                                                                                                                    | object  |                7 |                  0 |         0    |
| PCD                                                                                                                               | object  |                3 |                  0 |         0    |
| experiencia_profissional_prejudicada                                                                                              | object  |               17 |               2574 |        48.63 |
| Não acredito que minha experiência profissional seja afetada                                                                      | float64 |                2 |               2574 |        48.63 |
| Experiencia prejudicada devido a minha Cor Raça Etnia                                                                             | float64 |                2 |               2574 |        48.63 |
| Experiencia prejudicada devido a minha identidade de gênero                                                                       | float64 |                2 |               2574 |        48.63 |
| Experiencia prejudicada devido ao fato de ser PCD                                                                                 | float64 |                2 |               2574 |        48.63 |
| aspectos_prejudicados                                                                                                             | object  |              602 |               4049 |        76.5  |
| Quantidade de oportunidades de emprego/vagas recebidas                                                                            | float64 |                2 |               4048 |        76.48 |
| Senioridade das vagas recebidas em relação à sua experiência                                                                      | float64 |                2 |               4048 |        76.48 |
| Aprovação em processos seletivos/entrevistas                                                                                      | float64 |                2 |               4048 |        76.48 |
| Oportunidades de progressão de carreira                                                                                           | float64 |                2 |               4048 |        76.48 |
| Velocidade de progressão de carreira                                                                                              | float64 |                2 |               4048 |        76.48 |
| Nível de cobrança no trabalho/Stress no trabalho                                                                                  | float64 |                2 |               4048 |        76.48 |
| Atenção dada diante das minhas opiniões e ideias                                                                                  | float64 |                2 |               4048 |        76.48 |
| Relação com outros membros da empresa                                                                                             | float64 |                2 |               4048 |        76.48 |
| Relação com outros membros da empresa                                                                                             | float64 |                2 |               4048 |        76.48 |
| vive_no_brasil                                                                                                                    | int64   |                2 |                  0 |         0    |
| Estado onde mora                                                                                                                  | object  |               26 |                121 |         2.29 |
| uf onde mora                                                                                                                      | object  |               25 |                124 |         2.34 |
| Regiao onde mora                                                                                                                  | object  |                5 |                124 |         2.34 |
| Mudou de Estado?                                                                                                                  | float64 |                2 |                121 |         2.29 |
| Regiao de origem                                                                                                                  | object  |               28 |               4229 |        79.9  |
| Nivel de Ensino                                                                                                                   | object  |                7 |                  0 |         0    |
| Área de Formação                                                                                                                  | object  |                9 |                113 |         2.13 |
| Qual sua situação atual de trabalho?                                                                                              | object  |               13 |                  0 |         0    |
| Setor                                                                                                                             | object  |               21 |                540 |        10.2  |
| Numero de Funcionarios                                                                                                            | object  |                9 |                540 |        10.2  |
| Gestor?                                                                                                                           | float64 |                2 |                540 |        10.2  |
| Cargo como Gestor                                                                                                                 | object  |                5 |               4397 |        83.07 |
| Cargo Atual                                                                                                                       | object  |               17 |               1436 |        27.13 |
| Nivel                                                                                                                             | object  |                3 |               1436 |        27.13 |
| Faixa salarial                                                                                                                    | object  |               14 |                540 |        10.2  |
| Quanto tempo de experiência na área de dados você tem?                                                                            | object  |                8 |                540 |        10.2  |
| Quanto tempo de experiência na área de TI/Engenharia de Software você teve antes de começar a trabalhar na área de dados?         | object  |                7 |                540 |        10.2  |
| Você está satisfeito na sua empresa atual?                                                                                        | float64 |                2 |                540 |        10.2  |
| Qual o principal motivo da sua insatisfação com a empresa atual?                                                                  | object  |              259 |               3975 |        75.1  |
| Falta de oportunidade de crescimento no emprego atual                                                                             | float64 |                2 |               3975 |        75.1  |
| Salário atual não corresponde ao mercado                                                                                          | float64 |                2 |               3975 |        75.1  |
| Não tenho uma boa relação com meu líder/gestor                                                                                    | float64 |                2 |               3975 |        75.1  |
| Gostaria de trabalhar em em outra área de atuação                                                                                 | float64 |                2 |               3975 |        75.1  |
| Gostaria de receber mais benefícios                                                                                               | float64 |                2 |               3975 |        75.1  |
| O clima de trabalho/ambiente não é bom                                                                                            | float64 |                2 |               3975 |        75.1  |
| Falta de maturidade analítica na empresa                                                                                          | float64 |                2 |               3975 |        75.1  |
| Você participou de entrevistas de emprego nos últimos 6 meses?                                                                    | object  |                6 |                540 |        10.2  |
| Você pretende mudar de emprego nos próximos 6 meses?                                                                              | object  |                4 |                540 |        10.2  |
| Quais os principais critérios que você leva em consideração no momento de decidir onde trabalhar?                                 | object  |              466 |                566 |        10.69 |
| Remuneração/Salário                                                                                                               | float64 |                2 |                566 |        10.69 |
| Benefícios                                                                                                                        | float64 |                2 |                566 |        10.69 |
| Propósito do trabalho e da empresa                                                                                                | float64 |                2 |                566 |        10.69 |
| Flexibilidade de trabalho remoto                                                                                                  | float64 |                2 |                566 |        10.69 |
| Ambiente e clima de trabalho                                                                                                      | float64 |                2 |                566 |        10.69 |
| Oportunidade de aprendizado e trabalhar com referências na área                                                                   | float64 |                2 |                566 |        10.69 |
| Plano de carreira e oportunidades de crescimento profissional                                                                     | float64 |                2 |                566 |        10.69 |
| Maturidade da empresa em termos de tecnologia e dados                                                                             | float64 |                2 |                566 |        10.69 |
| Qualidade dos gestores e líderes                                                                                                  | float64 |                2 |                566 |        10.69 |
| Reputação que a empresa tem no mercado                                                                                            | float64 |                2 |                566 |        10.69 |
| Empresa que trabaha passou por layoff em 2023                                                                                     | object  |                3 |                540 |        10.2  |
| Atualmente qual a sua forma de trabalho?                                                                                          | object  |                4 |                540 |        10.2  |
| Qual a forma de trabalho ideal para você?                                                                                         | object  |                4 |                540 |        10.2  |
| Caso sua empresa decida pelo modelo 100% presencial qual será sua atitude?                                                        | object  |                3 |                540 |        10.2  |
| Qual o número aproximado de pessoas que atuam com dados na sua empresa hoje?                                                      | object  |                8 |               4397 |        83.07 |
| Quais desses papéis/cargos fazem parte do time (ou chapter) de dados da sua empresa?                                              | object  |              647 |               4434 |        83.77 |
| Analytics Engineer                                                                                                                | float64 |                2 |               4434 |        83.77 |
| Engenharia de Dados/Data Engineer                                                                                                 | float64 |                2 |               4434 |        83.77 |
| Analista de Dados/Data Analyst                                                                                                    | float64 |                2 |               4434 |        83.77 |
| Cientista de Dados/Data Scientist                                                                                                 | float64 |                2 |               4434 |        83.77 |
| Database Administrator/DBA                                                                                                        | float64 |                2 |               4434 |        83.77 |
| Analista de Business Intelligence/BI                                                                                              | float64 |                2 |               4434 |        83.77 |
| Arquiteto de Dados/Data Architect                                                                                                 | float64 |                2 |               4434 |        83.77 |
| Data Product Manager/DPM                                                                                                          | float64 |                2 |               4434 |        83.77 |
| Business Analyst                                                                                                                  | float64 |                2 |               4434 |        83.77 |
| Quais dessas responsabilidades fazem parte da sua rotina atual de trabalho como gestor?                                           | object  |              611 |               4420 |        83.51 |
| Pensar na visão de longo prazo de dados da empresa e fortalecimento da cultura analítica da companhia.                            | float64 |                2 |               4419 |        83.49 |
| Organização de treinamentos e iniciativas com o objetivo de aumentar a maturidade analítica das áreas de negócios.                | float64 |                2 |               4419 |        83.49 |
| Atração                                                                                                                           | float64 |                2 |               4419 |        83.49 |
| Decisão sobre contratação de ferramentas e tecnologias relacionadas a dados.                                                      | float64 |                2 |               4419 |        83.49 |
| Sou gestor da equipe responsável pela engenharia de dados e por manter o Data Lake da empresa como fonte única dos dados          | float64 |                2 |               4419 |        83.49 |
| Sou gestor da equipe responsável pela entrega de dados                                                                            | float64 |                2 |               4419 |        83.49 |
| Sou gestor da equipe responsável por iniciativas e projetos envolvendo Inteligência Artificial e Machine Learning.                | float64 |                2 |               4419 |        83.49 |
| Apesar de ser gestor ainda atuo na parte técnica                                                                                  | float64 |                2 |               4419 |        83.49 |
| Gestão de projetos de dados                                                                                                       | float64 |                2 |               4419 |        83.49 |
| Gestão de produtos de dados                                                                                                       | float64 |                2 |               4419 |        83.49 |
| Gestão de pessoas                                                                                                                 | float64 |                2 |               4419 |        83.49 |
| Quais são os 3 maiores desafios que você tem como gestor no atual momento?                                                        | object  |              601 |               4421 |        83.53 |
| a Contratar novos talentos.                                                                                                       | float64 |                2 |               4419 |        83.49 |
| b Reter talentos.                                                                                                                 | float64 |                2 |               4419 |        83.49 |
| c Convencer a empresa a aumentar os investimentos na área de dados.                                                               | float64 |                2 |               4419 |        83.49 |
| d Gestão de equipes no ambiente remoto.                                                                                           | float64 |                2 |               4419 |        83.49 |
| e Gestão de projetos envolvendo áreas multidisciplinares da empresa.                                                              | float64 |                2 |               4419 |        83.49 |
| f Organizar as informações e garantir a qualidade e confiabilidade.                                                               | float64 |                2 |               4419 |        83.49 |
| g Conseguir processar e armazenar um alto volume de dados.                                                                        | float64 |                2 |               4419 |        83.49 |
| h Conseguir gerar valor para as áreas de negócios através de estudos e experimentos.                                              | float64 |                2 |               4419 |        83.49 |
| i Desenvolver e manter modelos Machine Learning em produção.                                                                      | float64 |                2 |               4419 |        83.49 |
| j Gerenciar a expectativa das áreas de negócio em relação as entregas das equipes de dados.                                       | float64 |                2 |               4419 |        83.49 |
| k Garantir a manutenção dos projetos e modelos em produção                                                                        | float64 |                2 |               4419 |        83.49 |
| Conseguir levar inovação para a empresa através dos dados.                                                                        | float64 |                2 |               4419 |        83.49 |
| Garantir retorno do investimento (ROI) em projetos de dados.                                                                      | float64 |                2 |               4419 |        83.49 |
| Dividir o tempo entre entregas técnicas e gestão.                                                                                 | float64 |                2 |               4419 |        83.49 |
| AI Generativa é uma prioridade em sua empresa?                                                                                    | object  |                5 |               4397 |        83.07 |
| Tipos de uso de AI Generativa e LLMs na empresa                                                                                   | object  |              152 |               4431 |        83.71 |
| Colaboradores usando AI generativa de forma independente e descentralizada                                                        | float64 |                2 |               4431 |        83.71 |
| Direcionamento centralizado do uso de AI generativa                                                                               | float64 |                2 |               4431 |        83.71 |
| Desenvolvedores utilizando Copilots                                                                                               | float64 |                2 |               4431 |        83.71 |
| AI Generativa e LLMs para melhorar produtos externos                                                                              | float64 |                2 |               4431 |        83.71 |
| AI Generativa e LLMs para melhorar produtos internos para os colaboradores                                                        | float64 |                2 |               4431 |        83.71 |
| IA Generativa e LLMs como principal frente do negócio                                                                             | float64 |                2 |               4431 |        83.71 |
| IA Generativa e LLMs não é prioridade                                                                                             | float64 |                2 |               4431 |        83.71 |
| Não sei opinar sobre o uso de IA Generativa e LLMs na empresa                                                                     | float64 |                2 |               4431 |        83.71 |
| Motivos que levam a empresa a não usar AI Genrativa e LLMs                                                                        | object  |              269 |               4471 |        84.47 |
| Falta de compreensão dos casos de uso                                                                                             | float64 |                2 |               4470 |        84.45 |
| Falta de confiabilidade das saídas (alucinação dos modelos                                                                        | float64 |                2 |               4470 |        84.45 |
| Incerteza em relação a regulamentação                                                                                             | float64 |                2 |               4470 |        84.45 |
| Preocupações com segurança e privacidade de dados                                                                                 | float64 |                2 |               4470 |        84.45 |
| Retorno sobre investimento (ROI) não comprovado de IA Generativa                                                                  | float64 |                2 |               4470 |        84.45 |
| Dados da empresa não estão prontos para uso de IA Generativa                                                                      | float64 |                2 |               4470 |        84.45 |
| Falta de expertise ou falta de recursos                                                                                           | float64 |                2 |               4470 |        84.45 |
| Alta direção da empresa não vê valor ou não vê como prioridade                                                                    | float64 |                2 |               4470 |        84.45 |
| Preocupações com propriedade intelectual                                                                                          | float64 |                2 |               4470 |        84.45 |
| Mesmo que esse não seja seu cargo formal                                                                                          | object  |                4 |               1542 |        29.13 |
| Atuacao                                                                                                                           | object  |                6 |                  0 |         0    |
| Quais das fontes de dados listadas você já analisou ou processou no trabalho?                                                     | object  |              544 |               1521 |        28.74 |
| Dados relacionais (estruturados em bancos SQL                                                                                     | float64 |                2 |               1521 |        28.74 |
| Dados armazenados em bancos NoSQL                                                                                                 | float64 |                2 |               1521 |        28.74 |
| Imagens                                                                                                                           | float64 |                2 |               1521 |        28.74 |
| Textos/Documentos                                                                                                                 | float64 |                2 |               1521 |        28.74 |
| Vídeos                                                                                                                            | float64 |                2 |               1521 |        28.74 |
| Áudios                                                                                                                            | float64 |                2 |               1521 |        28.74 |
| Planilhas                                                                                                                         | float64 |                2 |               1521 |        28.74 |
| Dados georeferenciados                                                                                                            | float64 |                2 |               1521 |        28.74 |
| Entre as fontes de dados listadas                                                                                                 | object  |              104 |               1522 |        28.75 |
| Dados relacionais (estruturados em bancos SQL                                                                                     | float64 |                2 |               1521 |        28.74 |
| Dados armazenados em bancos NoSQL                                                                                                 | float64 |                2 |               1521 |        28.74 |
| Imagens                                                                                                                           | float64 |                2 |               1521 |        28.74 |
| Textos/Documentos                                                                                                                 | float64 |                2 |               1521 |        28.74 |
| Vídeos                                                                                                                            | float64 |                2 |               1521 |        28.74 |
| Áudios                                                                                                                            | float64 |                2 |               1521 |        28.74 |
| Planilhas                                                                                                                         | float64 |                2 |               1521 |        28.74 |
| Dados georeferenciados                                                                                                            | float64 |                2 |               1521 |        28.74 |
| Quais das linguagens listadas abaixo você utiliza no trabalho?                                                                    | object  |              271 |               1521 |        28.74 |
| SQL                                                                                                                               | float64 |                2 |               1521 |        28.74 |
| R                                                                                                                                 | float64 |                2 |               1521 |        28.74 |
| Python                                                                                                                            | float64 |                2 |               1521 |        28.74 |
| C/C++/C#                                                                                                                          | float64 |                2 |               1521 |        28.74 |
| .NET                                                                                                                              | float64 |                2 |               1521 |        28.74 |
| Java                                                                                                                              | float64 |                2 |               1521 |        28.74 |
| Julia                                                                                                                             | float64 |                2 |               1521 |        28.74 |
| SAS/Stata                                                                                                                         | float64 |                2 |               1521 |        28.74 |
| Visual Basic/VBA                                                                                                                  | float64 |                2 |               1521 |        28.74 |
| Scala                                                                                                                             | float64 |                2 |               1521 |        28.74 |
| Matlab                                                                                                                            | float64 |                2 |               1521 |        28.74 |
| Rust                                                                                                                              | float64 |                2 |               1521 |        28.74 |
| PHP                                                                                                                               | float64 |                2 |               1521 |        28.74 |
| JavaScript                                                                                                                        | float64 |                2 |               1521 |        28.74 |
| Não utilizo nenhuma linguagem                                                                                                     | float64 |                2 |               1521 |        28.74 |
| Entre as linguagens listadas abaixo                                                                                               | object  |               14 |               1521 |        28.74 |
| Entre as linguagens listadas abaixo                                                                                               | object  |               16 |               1543 |        29.15 |
| Quais dos bancos de dados/fontes de dados listados abaixo você utiliza no trabalho?                                               | object  |             1838 |               1523 |        28.77 |
| MySQL                                                                                                                             | float64 |                2 |               1521 |        28.74 |
| Oracle                                                                                                                            | float64 |                2 |               1521 |        28.74 |
| SQL SERVER                                                                                                                        | float64 |                2 |               1521 |        28.74 |
| Amazon Aurora ou RDS                                                                                                              | float64 |                2 |               1521 |        28.74 |
| DynamoDB                                                                                                                          | float64 |                2 |               1521 |        28.74 |
| CoachDB                                                                                                                           | float64 |                2 |               1521 |        28.74 |
| Cassandra                                                                                                                         | float64 |                2 |               1521 |        28.74 |
| MongoDB                                                                                                                           | float64 |                2 |               1521 |        28.74 |
| MariaDB                                                                                                                           | float64 |                2 |               1521 |        28.74 |
| Datomic                                                                                                                           | float64 |                2 |               1521 |        28.74 |
| S3                                                                                                                                | float64 |                2 |               1521 |        28.74 |
| PostgreSQL                                                                                                                        | float64 |                2 |               1521 |        28.74 |
| ElasticSearch                                                                                                                     | float64 |                2 |               1521 |        28.74 |
| DB2                                                                                                                               | float64 |                2 |               1521 |        28.74 |
| Microsoft Access                                                                                                                  | float64 |                2 |               1521 |        28.74 |
| SQLite                                                                                                                            | float64 |                2 |               1521 |        28.74 |
| Sybase                                                                                                                            | float64 |                2 |               1521 |        28.74 |
| Firebase                                                                                                                          | float64 |                2 |               1521 |        28.74 |
| Vertica                                                                                                                           | float64 |                2 |               1521 |        28.74 |
| Redis                                                                                                                             | float64 |                2 |               1521 |        28.74 |
| Neo4J                                                                                                                             | float64 |                2 |               1521 |        28.74 |
| Google BigQuery                                                                                                                   | float64 |                2 |               1521 |        28.74 |
| Google Firestore                                                                                                                  | float64 |                2 |               1521 |        28.74 |
| Amazon Redshift                                                                                                                   | float64 |                2 |               1521 |        28.74 |
| Amazon Athena                                                                                                                     | float64 |                2 |               1521 |        28.74 |
| Snowflake                                                                                                                         | float64 |                2 |               1521 |        28.74 |
| Databricks                                                                                                                        | float64 |                2 |               1521 |        28.74 |
| HBase                                                                                                                             | float64 |                2 |               1521 |        28.74 |
| Presto                                                                                                                            | float64 |                2 |               1521 |        28.74 |
| Splunk                                                                                                                            | float64 |                2 |               1521 |        28.74 |
| SAP HANA                                                                                                                          | float64 |                2 |               1521 |        28.74 |
| Hive                                                                                                                              | float64 |                2 |               1521 |        28.74 |
| Firebird                                                                                                                          | float64 |                2 |               1521 |        28.74 |
| Dentre as opções listadas                                                                                                         | object  |              175 |               1680 |        31.74 |
| Azure (Microsoft                                                                                                                  | float64 |                2 |               1680 |        31.74 |
| Amazon Web Services (AWS                                                                                                          | float64 |                2 |               1680 |        31.74 |
| Google Cloud (GCP                                                                                                                 | float64 |                2 |               1680 |        31.74 |
| Oracle Cloud                                                                                                                      | float64 |                2 |               1680 |        31.74 |
| IBM                                                                                                                               | float64 |                2 |               1680 |        31.74 |
| Servidores On Premise/Não utilizamos Cloud                                                                                        | float64 |                2 |               1680 |        31.74 |
| Cloud Própria                                                                                                                     | float64 |                2 |               1680 |        31.74 |
| Cloud preferida                                                                                                                   | object  |               44 |               1522 |        28.75 |
| Ferramenta de BI utilizada no dia a dia                                                                                           | object  |              764 |               1521 |        28.74 |
| Microsoft PowerBI                                                                                                                 | float64 |                2 |               1521 |        28.74 |
| Qlik View/Qlik Sense                                                                                                              | float64 |                2 |               1521 |        28.74 |
| Tableau                                                                                                                           | float64 |                2 |               1521 |        28.74 |
| Metabase                                                                                                                          | float64 |                2 |               1521 |        28.74 |
| Superset                                                                                                                          | float64 |                2 |               1521 |        28.74 |
| Redash                                                                                                                            | float64 |                2 |               1521 |        28.74 |
| Looker                                                                                                                            | float64 |                2 |               1521 |        28.74 |
| Looker Studio(Google Data Studio                                                                                                  | float64 |                2 |               1521 |        28.74 |
| Amazon Quicksight                                                                                                                 | float64 |                2 |               1521 |        28.74 |
| Mode                                                                                                                              | float64 |                2 |               1521 |        28.74 |
| Alteryx                                                                                                                           | float64 |                2 |               1521 |        28.74 |
| MicroStrategy                                                                                                                     | float64 |                2 |               1521 |        28.74 |
| IBM Analytics/Cognos                                                                                                              | float64 |                2 |               1521 |        28.74 |
| SAP Business Objects/SAP Analytics                                                                                                | float64 |                2 |               1521 |        28.74 |
| Oracle Business Intelligence                                                                                                      | float64 |                2 |               1521 |        28.74 |
| Salesforce/Einstein Analytics                                                                                                     | float64 |                2 |               1521 |        28.74 |
| Birst                                                                                                                             | float64 |                2 |               1521 |        28.74 |
| SAS Visual Analytics                                                                                                              | float64 |                2 |               1521 |        28.74 |
| Grafana                                                                                                                           | float64 |                2 |               1521 |        28.74 |
| TIBCO Spotfire                                                                                                                    | float64 |                2 |               1521 |        28.74 |
| Pentaho                                                                                                                           | float64 |                2 |               1521 |        28.74 |
| Fazemos todas as análises utilizando apenas Excel ou planilhas do google                                                          | float64 |                2 |               1521 |        28.74 |
| Não utilizo nenhuma ferramenta de BI no trabalho                                                                                  | float64 |                2 |               1521 |        28.74 |
| Qual sua ferramenta de BI preferida?                                                                                              | object  |               91 |               1525 |        28.81 |
| Qual o tipo de uso de AI Generativa e LLMs na empresa                                                                             | object  |              199 |               1521 |        28.74 |
| Colaboradores usando AI generativa de forma independente e descentralizada                                                        | float64 |                2 |               1521 |        28.74 |
| Direcionamento centralizado do uso de AI generativa                                                                               | float64 |                2 |               1521 |        28.74 |
| Desenvolvedores utilizando Copilots                                                                                               | float64 |                2 |               1521 |        28.74 |
| AI Generativa e LLMs para melhorar produtos externos para os clientes finais                                                      | float64 |                2 |               1521 |        28.74 |
| AI Generativa e LLMs para melhorar produtos internos para os colaboradores                                                        | float64 |                2 |               1521 |        28.74 |
| IA Generativa e LLMs como principal frente do negócio                                                                             | float64 |                2 |               1521 |        28.74 |
| IA Generativa e LLMs não é prioridade                                                                                             | float64 |                2 |               1521 |        28.74 |
| Não sei opinar sobre o uso de IA Generativa e LLMs na empresa                                                                     | float64 |                2 |               1521 |        28.74 |
| Utiliza ChatGPT ou LLMs no trabalho?                                                                                              | object  |               22 |               1521 |        28.74 |
| Não uso soluções de AI Generativa com foco em produtividade                                                                       | float64 |                2 |               1521 |        28.74 |
| Uso soluções gratuitas de AI Generativa com foco em produtividade                                                                 | float64 |                2 |               1521 |        28.74 |
| Uso e pago pelas soluções de AI Generativa com foco em produtividade                                                              | float64 |                2 |               1521 |        28.74 |
| A empresa que trabalho paga pelas soluções de AI Generativa com foco em produtividade                                             | float64 |                2 |               1521 |        28.74 |
| Uso soluções do tipo Copilot                                                                                                      | float64 |                2 |               1521 |        28.74 |
| Qual seu objetivo na área de dados?                                                                                               | object  |               52 |               4768 |        90.08 |
| Qual oportunidade você está buscando?                                                                                             | object  |               13 |               5006 |        94.58 |
| Há quanto tempo você busca uma oportunidade na área de dados?                                                                     | object  |                4 |               5006 |        94.58 |
| Como tem sido a busca por um emprego na área de dados?                                                                            | object  |                6 |               5007 |        94.6  |
| Quais das opções abaixo fazem parte da sua rotina no trabalho atual como engenheiro de dados?                                     | object  |              311 |               4381 |        82.77 |
| Desenvolvo pipelines de dados utilizando linguagens de programação como Python                                                    | float64 |                2 |               4381 |        82.77 |
| Realizo construções de ETLs em ferramentas como Pentaho                                                                           | float64 |                2 |               4381 |        82.77 |
| Crio consultas através da linguagem SQL para exportar informações e compartilhar com as áreas de negócio.                         | float64 |                2 |               4381 |        82.77 |
| Atuo na integração de diferentes fontes de dados através de plataformas proprietárias como Stitch Data                            | float64 |                2 |               4381 |        82.77 |
| Modelo soluções de arquitetura de dados                                                                                           | float64 |                2 |               4381 |        82.77 |
| Desenvolvo/cuido da manutenção de repositórios de dados baseados em streaming de eventos como Data Lakes e Data Lakehouses.       | float64 |                2 |               4381 |        82.77 |
| Atuo na modelagem dos dados                                                                                                       | float64 |                2 |               4381 |        82.77 |
| Cuido da qualidade dos dados                                                                                                      | float64 |                2 |               4381 |        82.77 |
| Nenhuma das opções listadas refletem meu dia a dia.                                                                               | float64 |                2 |               4381 |        82.77 |
| Quais as ferramentas/tecnologias de ETL que você utiliza no trabalho como Data Engineer?                                          | object  |              357 |               4381 |        82.77 |
| Scripts Python                                                                                                                    | float64 |                2 |               4381 |        82.77 |
| SQL & Stored Procedures                                                                                                           | float64 |                2 |               4381 |        82.77 |
| Apache Airflow                                                                                                                    | float64 |                2 |               4381 |        82.77 |
| Apache NiFi                                                                                                                       | float64 |                2 |               4381 |        82.77 |
| Luigi                                                                                                                             | float64 |                2 |               4381 |        82.77 |
| AWS Glue                                                                                                                          | float64 |                2 |               4381 |        82.77 |
| Talend                                                                                                                            | float64 |                2 |               4381 |        82.77 |
| Pentaho                                                                                                                           | float64 |                2 |               4381 |        82.77 |
| Alteryx                                                                                                                           | float64 |                2 |               4381 |        82.77 |
| Stitch                                                                                                                            | float64 |                2 |               4381 |        82.77 |
| Fivetran                                                                                                                          | float64 |                2 |               4381 |        82.77 |
| Google Dataflow                                                                                                                   | float64 |                2 |               4381 |        82.77 |
| Oracle Data Integrator                                                                                                            | float64 |                2 |               4381 |        82.77 |
| IBM DataStage                                                                                                                     | float64 |                2 |               4381 |        82.77 |
| SAP BW ETL                                                                                                                        | float64 |                2 |               4381 |        82.77 |
| SQL Server Integration Services (SSIS                                                                                             | float64 |                2 |               4381 |        82.77 |
| SAS Data Integration                                                                                                              | float64 |                2 |               4381 |        82.77 |
| Qlik Sense                                                                                                                        | float64 |                2 |               4381 |        82.77 |
| Knime                                                                                                                             | float64 |                2 |               4381 |        82.77 |
| Databricks                                                                                                                        | float64 |                2 |               4381 |        82.77 |
| Não utilizo ferramentas de ETL                                                                                                    | float64 |                2 |               4381 |        82.77 |
| Sua organização possui um Data Lake?                                                                                              | float64 |                2 |               4382 |        82.79 |
| Qual tecnologia utilizada como plataforma do Data Lake?                                                                           | object  |                7 |               4551 |        85.98 |
| Sua organização possui um Data Warehouse?                                                                                         | float64 |                2 |               4384 |        82.83 |
| Qual tecnologia utilizada como plataforma do Data Warehouse?                                                                      | object  |               10 |               4554 |        86.04 |
| Quais as ferramentas de gestão de Qualidade de dados                                                                              | object  |               13 |               4738 |        89.51 |
| Em qual das opções abaixo você gasta a maior parte do seu tempo?                                                                  | object  |               59 |               4381 |        82.77 |
| Desenvolvendo pipelines de dados utilizando linguagens de programação como Python                                                 | float64 |                2 |               4381 |        82.77 |
| Realizando construções de ETLs em ferramentas como Pentaho                                                                        | float64 |                2 |               4381 |        82.77 |
| Criando consultas através da linguagem SQL para exportar informações e compartilhar com as áreas de negócio.                      | float64 |                2 |               4381 |        82.77 |
| Atuando na integração de diferentes fontes de dados através de plataformas proprietárias como Stitch Data                         | float64 |                2 |               4381 |        82.77 |
| Modelando soluções de arquitetura de dados                                                                                        | float64 |                2 |               4381 |        82.77 |
| Desenvolvendo/cuidando da manutenção de repositórios de dados baseados em streaming de eventos como Data Lakes e Data Lakehouses. | float64 |                2 |               4381 |        82.77 |
| Atuando na modelagem dos dados                                                                                                    | float64 |                2 |               4381 |        82.77 |
| Cuidando da qualidade dos dados                                                                                                   | float64 |                2 |               4381 |        82.77 |
| Nenhuma das opções listadas refletem meu dia a dia.                                                                               | float64 |                2 |               4381 |        82.77 |
| Quais das opções abaixo fazem parte da sua rotina no trabalho atual com análise de dados?                                         | object  |              415 |               3498 |        66.09 |
| Processo e analiso dados utilizando linguagens de programação como Python                                                         | float64 |                2 |               3498 |        66.09 |
| Realizo construções de dashboards em ferramentas de BI como PowerBI                                                               | float64 |                2 |               3498 |        66.09 |
| Crio consultas através da linguagem SQL para exportar informações e compartilhar com as áreas de negócio.                         | float64 |                2 |               3498 |        66.09 |
| Utilizo APIs para extrair dados e complementar minhas análises.                                                                   | float64 |                2 |               3498 |        66.09 |
| Realizo experimentos e estudos utilizando metodologias estatísticas como teste de hipótese                                        | float64 |                2 |               3498 |        66.09 |
| Desenvolvo/cuido da manutenção de ETLs utilizando tecnologias como Talend                                                         | float64 |                2 |               3498 |        66.09 |
| Atuo na modelagem dos dados                                                                                                       | float64 |                2 |               3498 |        66.09 |
| Desenvolvo/cuido da manutenção de planilhas para atender as áreas de negócio.                                                     | float64 |                2 |               3498 |        66.09 |
| Utilizo ferramentas avançadas de estatística como SASS                                                                            | float64 |                2 |               3498 |        66.09 |
| Nenhuma das opções listadas refletem meu dia a dia.                                                                               | float64 |                2 |               3498 |        66.09 |
| Quais as ferramentas/tecnologias de ETL que você utiliza no trabalho como Data Analyst?                                           | object  |              372 |               3498 |        66.09 |
| Scripts Python                                                                                                                    | float64 |                2 |               3498 |        66.09 |
| SQL & Stored Procedures                                                                                                           | float64 |                2 |               3498 |        66.09 |
| Apache Airflow                                                                                                                    | float64 |                2 |               3498 |        66.09 |
| Apache NiFi                                                                                                                       | float64 |                2 |               3498 |        66.09 |
| Luigi                                                                                                                             | float64 |                2 |               3498 |        66.09 |
| AWS Glue                                                                                                                          | float64 |                2 |               3498 |        66.09 |
| Talend                                                                                                                            | float64 |                2 |               3498 |        66.09 |
| Pentaho                                                                                                                           | float64 |                2 |               3498 |        66.09 |
| Alteryx                                                                                                                           | float64 |                2 |               3498 |        66.09 |
| Stitch                                                                                                                            | float64 |                2 |               3498 |        66.09 |
| Fivetran                                                                                                                          | float64 |                2 |               3498 |        66.09 |
| Google Dataflow                                                                                                                   | float64 |                2 |               3498 |        66.09 |
| Oracle Data Integrator                                                                                                            | float64 |                2 |               3498 |        66.09 |
| IBM DataStage                                                                                                                     | float64 |                2 |               3498 |        66.09 |
| SAP BW ETL                                                                                                                        | float64 |                2 |               3498 |        66.09 |
| SQL Server Integration Services (SSIS                                                                                             | float64 |                2 |               3498 |        66.09 |
| SAS Data Integration                                                                                                              | float64 |                2 |               3498 |        66.09 |
| Qlik Sense                                                                                                                        | float64 |                2 |               3498 |        66.09 |
| Knime                                                                                                                             | float64 |                2 |               3498 |        66.09 |
| Databricks                                                                                                                        | float64 |                2 |               3498 |        66.09 |
| Não utilizo ferramentas de ETL                                                                                                    | float64 |                2 |               3498 |        66.09 |
| Sua empresa utiliza alguma das ferramentas listadas para dar mais autonomia em análise de dados para as áreas de negócio?         | object  |               32 |               3498 |        66.09 |
| Ferramentas de AutoML como H2O.ai                                                                                                 | float64 |                2 |               3498 |        66.09 |
| ""Point and Click"" Analytics como Alteryx                                                                                        | float64 |                2 |               3498 |        66.09 |
| Product metricts & Insights como Mixpanel                                                                                         | float64 |                2 |               3498 |        66.09 |
| Ferramentas de análise dentro de ferramentas de CRM como Salesforce Einstein Anaytics ou Zendesk dashboards.                      | float64 |                2 |               3498 |        66.09 |
| Minha empresa não utiliza essas ferramentas.                                                                                      | float64 |                2 |               3498 |        66.09 |
| Não sei informar.                                                                                                                 | float64 |                2 |               3498 |        66.09 |
| Em qual das opções abaixo você gasta a maior parte do seu tempo de trabalho?                                                      | object  |               66 |               3498 |        66.09 |
| Processando e analisando dados utilizando linguagens de programação como Python                                                   | float64 |                2 |               3498 |        66.09 |
| Realizando construções de dashboards em ferramentas de BI como PowerBI                                                            | float64 |                2 |               3498 |        66.09 |
| Criando consultas através da linguagem SQL para exportar informações e compartilhar com as áreas de negócio.                      | float64 |                2 |               3498 |        66.09 |
| Utilizando APIs para extrair dados e complementar minhas análises.                                                                | float64 |                2 |               3498 |        66.09 |
| Realizando experimentos e estudos utilizando metodologias estatísticas como teste de hipótese                                     | float64 |                2 |               3498 |        66.09 |
| Desenvolvendo/cuidando da manutenção de ETLs utilizando tecnologias como Talend                                                   | float64 |                2 |               3498 |        66.09 |
| Atuando na modelagem dos dados                                                                                                    | float64 |                2 |               3498 |        66.09 |
| Desenvolvendo/cuidando da manutenção de planilhas do Excel ou Google Sheets para atender as áreas de negócio.                     | float64 |                2 |               3498 |        66.09 |
| Utilizando ferramentas avançadas de estatística como SAS                                                                          | float64 |                2 |               3498 |        66.09 |
| Nenhuma das opções listadas refletem meu dia a dia.                                                                               | float64 |                2 |               3498 |        66.09 |
| Quais das opções abaixo fazem parte da sua rotina no trabalho atual com ciência de dados?                                         | object  |              438 |               4545 |        85.87 |
| Estudos Ad-hoc com o objetivo de confirmar hipóteses                                                                              | float64 |                2 |               4545 |        85.87 |
| Sou responsável pela coleta e limpeza dos dados que uso para análise e modelagem.                                                 | float64 |                2 |               4545 |        85.87 |
| Sou responsável por entrar em contato com os times de negócio para definição do problema                                          | float64 |                2 |               4545 |        85.87 |
| Desenvolvo modelos de Machine Learning com o objetivo de colocar em produção em sistemas (produtos de dados).                     | float64 |                2 |               4545 |        85.87 |
| Sou responsável por colocar modelos em produção                                                                                   | float64 |                2 |               4545 |        85.87 |
| Cuido da manutenção de modelos de Machine Learning já em produção                                                                 | float64 |                2 |               4545 |        85.87 |
| Realizo construções de dashboards em ferramentas de BI como PowerBI                                                               | float64 |                2 |               4545 |        85.87 |
| Utilizo ferramentas avançadas de estatística como SAS                                                                             | float64 |                2 |               4545 |        85.87 |
| Crio e dou manutenção em ETLs                                                                                                     | float64 |                2 |               4545 |        85.87 |
| Crio e gerencio soluções de Feature Store e cultura de MLOps.                                                                     | float64 |                2 |               4545 |        85.87 |
| Sou responsável por criar e manter a infra que meus modelos e soluções rodam (clusters                                            | float64 |                2 |               4545 |        85.87 |
| Treino e aplico LLMs para solucionar problemas de negócio.                                                                        | float64 |                2 |               4545 |        85.87 |
| Quais as técnicas e métodos listados abaixo você costuma utilizar no trabalho?                                                    | object  |              470 |               4545 |        85.87 |
| Utilizo modelos de regressão (linear                                                                                              | float64 |                2 |               4545 |        85.87 |
| Utilizo redes neurais ou modelos baseados em árvore para criar modelos de classificação                                           | float64 |                2 |               4545 |        85.87 |
| Desenvolvo sistemas de recomendação (RecSys                                                                                       | float64 |                2 |               4545 |        85.87 |
| Utilizo métodos estatísticos Bayesianos para analisar dados                                                                       | float64 |                2 |               4545 |        85.87 |
| Utilizo técnicas de NLP (Natural Language Processing) para análisar dados não-estruturados                                        | float64 |                2 |               4545 |        85.87 |
| Utilizo métodos estatísticos clássicos (Testes de hipótese                                                                        | float64 |                2 |               4545 |        85.87 |
| Utilizo cadeias de Markov ou HMMs para realizar análises de dados                                                                 | float64 |                2 |               4545 |        85.87 |
| Desenvolvo técnicas de Clusterização (K-means                                                                                     | float64 |                2 |               4545 |        85.87 |
| Realizo previsões através de modelos de Séries Temporais (Time Series                                                             | float64 |                2 |               4545 |        85.87 |
| Utilizo modelos de Reinforcement Learning (aprendizado por reforço                                                                | float64 |                2 |               4545 |        85.87 |
| Utilizo modelos de Machine Learning para detecção de fraude                                                                       | float64 |                2 |               4545 |        85.87 |
| Utilizo métodos de Visão Computacional                                                                                            | float64 |                2 |               4545 |        85.87 |
| Utilizo modelos de Detecção de Churn                                                                                              | float64 |                2 |               4545 |        85.87 |
| Utilizo LLMs para solucionar problemas de negócio                                                                                 | float64 |                2 |               4545 |        85.87 |
| Quais dessas tecnologias fazem parte do seu dia a dia como cientista de dados?                                                    | object  |              403 |               4545 |        85.87 |
| Ferramentas de BI (PowerBI                                                                                                        | float64 |                2 |               4545 |        85.87 |
| Planilhas (Excel                                                                                                                  | float64 |                2 |               4545 |        85.87 |
| Ambientes de desenvolvimento local (R-studio                                                                                      | float64 |                2 |               4545 |        85.87 |
| Ambientes de desenvolvimento na nuvem (Google Colab                                                                               | float64 |                2 |               4545 |        85.87 |
| Ferramentas de AutoML (Datarobot                                                                                                  | float64 |                2 |               4545 |        85.87 |
| Ferramentas de ETL (Apache Airflow                                                                                                | float64 |                2 |               4545 |        85.87 |
| Plataformas de Machine Learning (TensorFlow                                                                                       | float64 |                2 |               4545 |        85.87 |
| Feature Store (Feast                                                                                                              | float64 |                2 |               4545 |        85.87 |
| Sistemas de controle de versão (Github                                                                                            | float64 |                2 |               4545 |        85.87 |
| Plataformas de Data Apps (Streamlit                                                                                               | float64 |                2 |               4545 |        85.87 |
| Ferramentas de estatística avançada como SPSS                                                                                     | float64 |                2 |               4545 |        85.87 |
| Em qual das opções abaixo você gasta a maior parte do seu tempo no trabalho?                                                      | object  |               87 |               4545 |        85.87 |
| Estudos Ad-hoc com o objetivo de confirmar hipóteses                                                                              | float64 |                2 |               4545 |        85.87 |
| Coletando e limpando os dados que uso para análise e modelagem.                                                                   | float64 |                2 |               4545 |        85.87 |
| Entrando em contato com os times de negócio para definição do problema                                                            | float64 |                2 |               4545 |        85.87 |
| Desenvolvendo modelos de Machine Learning com o objetivo de colocar em produção em sistemas (produtos de dados).                  | float64 |                2 |               4545 |        85.87 |
| Colocando modelos em produção                                                                                                     | float64 |                2 |               4545 |        85.87 |
| Cuidando da manutenção de modelos de Machine Learning já em produção                                                              | float64 |                2 |               4545 |        85.87 |
| Realizando construções de dashboards em ferramentas de BI como PowerBI                                                            | float64 |                2 |               4545 |        85.87 |
| Utilizando ferramentas avançadas de estatística como SAS                                                                          | float64 |                2 |               4545 |        85.87 |
| Criando e dando manutenção em ETLs                                                                                                | float64 |                2 |               4545 |        85.87 |
| Criando e gerenciando soluções de Feature Store e cultura de MLOps.                                                               | float64 |                2 |               4545 |        85.87 |
| Criando e mantendo a infra que meus modelos e soluções rodam (clusters                                                            | float64 |                2 |               4545 |        85.87 |
| Treinando e aplicando LLMs para solucionar problemas de negócio.                                                                  | float64 |                2 |               4545 |        85.87 |

## Estatísticas Numéricas

|                                                                                                                                   |   count |        mean |       std |   min |   25% |   50% |   75% |   max |
|:----------------------------------------------------------------------------------------------------------------------------------|--------:|------------:|----------:|------:|------:|------:|------:|------:|
| Idade                                                                                                                             |    5293 | 31.9972     | 7.6235    |    18 |    27 |    30 |    36 |    73 |
| Não acredito que minha experiência profissional seja afetada                                                                      |    2719 |  0.542111   | 0.498315  |     0 |     0 |     1 |     1 |     1 |
| Experiencia prejudicada devido a minha Cor Raça Etnia                                                                             |    2719 |  0.202648   | 0.402046  |     0 |     0 |     0 |     0 |     1 |
| Experiencia prejudicada devido a minha identidade de gênero                                                                       |    2719 |  0.291284   | 0.454437  |     0 |     0 |     0 |     1 |     1 |
| Experiencia prejudicada devido ao fato de ser PCD                                                                                 |    2719 |  0.0246414  | 0.155058  |     0 |     0 |     0 |     0 |     1 |
| Quantidade de oportunidades de emprego/vagas recebidas                                                                            |    1245 |  0.389558   | 0.487846  |     0 |     0 |     0 |     1 |     1 |
| Senioridade das vagas recebidas em relação à sua experiência                                                                      |    1245 |  0.342972   | 0.474893  |     0 |     0 |     0 |     1 |     1 |
| Aprovação em processos seletivos/entrevistas                                                                                      |    1245 |  0.413655   | 0.492686  |     0 |     0 |     0 |     1 |     1 |
| Oportunidades de progressão de carreira                                                                                           |    1245 |  0.490763   | 0.500116  |     0 |     0 |     0 |     1 |     1 |
| Velocidade de progressão de carreira                                                                                              |    1245 |  0.516466   | 0.49993   |     0 |     0 |     1 |     1 |     1 |
| Nível de cobrança no trabalho/Stress no trabalho                                                                                  |    1245 |  0.279518   | 0.448943  |     0 |     0 |     0 |     1 |     1 |
| Atenção dada diante das minhas opiniões e ideias                                                                                  |    1245 |  0.53494    | 0.498978  |     0 |     0 |     1 |     1 |     1 |
| Relação com outros membros da empresa                                                                                             |    1245 |  0.321285   | 0.467158  |     0 |     0 |     0 |     1 |     1 |
| Relação com outros membros da empresa                                                                                             |    1245 |  0.249799   | 0.433071  |     0 |     0 |     0 |     0 |     1 |
| Relação com outros membros da empresa                                                                                             |    1245 |  0.321285   | 0.467158  |     0 |     0 |     0 |     1 |     1 |
| Relação com outros membros da empresa                                                                                             |    1245 |  0.249799   | 0.433071  |     0 |     0 |     0 |     0 |     1 |
| vive_no_brasil                                                                                                                    |    5293 |  0.97714    | 0.149472  |     0 |     1 |     1 |     1 |     1 |
| Mudou de Estado?                                                                                                                  |    5172 |  0.794277   | 0.404268  |     0 |     1 |     1 |     1 |     1 |
| Gestor?                                                                                                                           |    4753 |  0.188513   | 0.391162  |     0 |     0 |     0 |     0 |     1 |
| Você está satisfeito na sua empresa atual?                                                                                        |    4753 |  0.719546   | 0.449269  |     0 |     0 |     1 |     1 |     1 |
| Falta de oportunidade de crescimento no emprego atual                                                                             |    1318 |  0.492413   | 0.500132  |     0 |     0 |     0 |     1 |     1 |
| Salário atual não corresponde ao mercado                                                                                          |    1318 |  0.427162   | 0.494854  |     0 |     0 |     0 |     1 |     1 |
| Não tenho uma boa relação com meu líder/gestor                                                                                    |    1318 |  0.0766313  | 0.266106  |     0 |     0 |     0 |     0 |     1 |
| Gostaria de trabalhar em em outra área de atuação                                                                                 |    1318 |  0.248862   | 0.432518  |     0 |     0 |     0 |     0 |     1 |
| Gostaria de receber mais benefícios                                                                                               |    1318 |  0.186646   | 0.389775  |     0 |     0 |     0 |     0 |     1 |
| O clima de trabalho/ambiente não é bom                                                                                            |    1318 |  0.159332   | 0.366125  |     0 |     0 |     0 |     0 |     1 |
| Falta de maturidade analítica na empresa                                                                                          |    1318 |  0.377086   | 0.484841  |     0 |     0 |     0 |     1 |     1 |
| Remuneração/Salário                                                                                                               |    4727 |  0.813624   | 0.389451  |     0 |     1 |     1 |     1 |     1 |
| Benefícios                                                                                                                        |    4727 |  0.227417   | 0.419208  |     0 |     0 |     0 |     0 |     1 |
| Propósito do trabalho e da empresa                                                                                                |    4727 |  0.152105   | 0.359161  |     0 |     0 |     0 |     0 |     1 |
| Flexibilidade de trabalho remoto                                                                                                  |    4727 |  0.584303   | 0.492894  |     0 |     0 |     1 |     1 |     1 |
| Ambiente e clima de trabalho                                                                                                      |    4727 |  0.185741   | 0.388939  |     0 |     0 |     0 |     0 |     1 |
| Oportunidade de aprendizado e trabalhar com referências na área                                                                   |    4727 |  0.245822   | 0.430619  |     0 |     0 |     0 |     0 |     1 |
| Plano de carreira e oportunidades de crescimento profissional                                                                     |    4727 |  0.335308   | 0.472148  |     0 |     0 |     0 |     1 |     1 |
| Maturidade da empresa em termos de tecnologia e dados                                                                             |    4727 |  0.125661   | 0.331502  |     0 |     0 |     0 |     0 |     1 |
| Qualidade dos gestores e líderes                                                                                                  |    4727 |  0.0738312  | 0.261524  |     0 |     0 |     0 |     0 |     1 |
| Reputação que a empresa tem no mercado                                                                                            |    4727 |  0.0560609  | 0.230064  |     0 |     0 |     0 |     0 |     1 |
| Analytics Engineer                                                                                                                |     859 |  0.322468   | 0.467693  |     0 |     0 |     0 |     1 |     1 |
| Engenharia de Dados/Data Engineer                                                                                                 |     859 |  0.654249   | 0.47589   |     0 |     0 |     1 |     1 |     1 |
| Analista de Dados/Data Analyst                                                                                                    |     859 |  0.675204   | 0.468572  |     0 |     0 |     1 |     1 |     1 |
| Cientista de Dados/Data Scientist                                                                                                 |     859 |  0.623981   | 0.484667  |     0 |     0 |     1 |     1 |     1 |
| Database Administrator/DBA                                                                                                        |     859 |  0.222352   | 0.416068  |     0 |     0 |     0 |     0 |     1 |
| Analista de Business Intelligence/BI                                                                                              |     859 |  0.547148   | 0.498062  |     0 |     0 |     1 |     1 |     1 |
| Arquiteto de Dados/Data Architect                                                                                                 |     859 |  0.324796   | 0.468572  |     0 |     0 |     0 |     1 |     1 |
| Data Product Manager/DPM                                                                                                          |     859 |  0.240978   | 0.427926  |     0 |     0 |     0 |     0 |     1 |
| Business Analyst                                                                                                                  |     859 |  0.395809   | 0.489309  |     0 |     0 |     0 |     1 |     1 |
| Pensar na visão de longo prazo de dados da empresa e fortalecimento da cultura analítica da companhia.                            |     874 |  0.630435   | 0.482963  |     0 |     0 |     1 |     1 |     1 |
| Organização de treinamentos e iniciativas com o objetivo de aumentar a maturidade analítica das áreas de negócios.                |     874 |  0.40389    | 0.490957  |     0 |     0 |     0 |     1 |     1 |
| Atração                                                                                                                           |     874 |  0.457666   | 0.49849   |     0 |     0 |     0 |     1 |     1 |
| Decisão sobre contratação de ferramentas e tecnologias relacionadas a dados.                                                      |     874 |  0.378719   | 0.485346  |     0 |     0 |     0 |     1 |     1 |
| Sou gestor da equipe responsável pela engenharia de dados e por manter o Data Lake da empresa como fonte única dos dados          |     874 |  0.306636   | 0.461361  |     0 |     0 |     0 |     1 |     1 |
| Sou gestor da equipe responsável pela entrega de dados                                                                            |     874 |  0.516018   | 0.500029  |     0 |     0 |     1 |     1 |     1 |
| Sou gestor da equipe responsável por iniciativas e projetos envolvendo Inteligência Artificial e Machine Learning.                |     874 |  0.324943   | 0.468622  |     0 |     0 |     0 |     1 |     1 |
| Apesar de ser gestor ainda atuo na parte técnica                                                                                  |     874 |  0.393593   | 0.488826  |     0 |     0 |     0 |     1 |     1 |
| Gestão de projetos de dados                                                                                                       |     874 |  0.447368   | 0.497507  |     0 |     0 |     0 |     1 |     1 |
| Gestão de produtos de dados                                                                                                       |     874 |  0.342105   | 0.474686  |     0 |     0 |     0 |     1 |     1 |
| Gestão de pessoas                                                                                                                 |     874 |  0.574371   | 0.494721  |     0 |     0 |     1 |     1 |     1 |
| a Contratar novos talentos.                                                                                                       |     874 |  0.162471   | 0.369094  |     0 |     0 |     0 |     0 |     1 |
| b Reter talentos.                                                                                                                 |     874 |  0.132723   | 0.339469  |     0 |     0 |     0 |     0 |     1 |
| c Convencer a empresa a aumentar os investimentos na área de dados.                                                               |     874 |  0.169336   | 0.375264  |     0 |     0 |     0 |     0 |     1 |
| d Gestão de equipes no ambiente remoto.                                                                                           |     874 |  0.0858124  | 0.280247  |     0 |     0 |     0 |     0 |     1 |
| e Gestão de projetos envolvendo áreas multidisciplinares da empresa.                                                              |     874 |  0.188787   | 0.391564  |     0 |     0 |     0 |     0 |     1 |
| f Organizar as informações e garantir a qualidade e confiabilidade.                                                               |     874 |  0.308924   | 0.462314  |     0 |     0 |     0 |     1 |     1 |
| g Conseguir processar e armazenar um alto volume de dados.                                                                        |     874 |  0.0526316  | 0.223425  |     0 |     0 |     0 |     0 |     1 |
| h Conseguir gerar valor para as áreas de negócios através de estudos e experimentos.                                              |     874 |  0.305492   | 0.460879  |     0 |     0 |     0 |     1 |     1 |
| i Desenvolver e manter modelos Machine Learning em produção.                                                                      |     874 |  0.0789474  | 0.269811  |     0 |     0 |     0 |     0 |     1 |
| j Gerenciar a expectativa das áreas de negócio em relação as entregas das equipes de dados.                                       |     874 |  0.363844   | 0.48138   |     0 |     0 |     0 |     1 |     1 |
| k Garantir a manutenção dos projetos e modelos em produção                                                                        |     874 |  0.129291   | 0.335713  |     0 |     0 |     0 |     0 |     1 |
| Conseguir levar inovação para a empresa através dos dados.                                                                        |     874 |  0.240275   | 0.427495  |     0 |     0 |     0 |     0 |     1 |
| Garantir retorno do investimento (ROI) em projetos de dados.                                                                      |     874 |  0.227689   | 0.419581  |     0 |     0 |     0 |     0 |     1 |
| Dividir o tempo entre entregas técnicas e gestão.                                                                                 |     874 |  0.29405    | 0.455876  |     0 |     0 |     0 |     1 |     1 |
| Colaboradores usando AI generativa de forma independente e descentralizada                                                        |     862 |  0.351508   | 0.477718  |     0 |     0 |     0 |     1 |     1 |
| Colaboradores usando AI generativa de forma independente e descentralizada                                                        |    3772 |  0.456787   | 0.498195  |     0 |     0 |     0 |     1 |     1 |
| Direcionamento centralizado do uso de AI generativa                                                                               |     862 |  0.13109    | 0.337695  |     0 |     0 |     0 |     0 |     1 |
| Direcionamento centralizado do uso de AI generativa                                                                               |    3772 |  0.104454   | 0.305889  |     0 |     0 |     0 |     0 |     1 |
| Desenvolvedores utilizando Copilots                                                                                               |     862 |  0.215777   | 0.411599  |     0 |     0 |     0 |     0 |     1 |
| Desenvolvedores utilizando Copilots                                                                                               |    3772 |  0.153234   | 0.360261  |     0 |     0 |     0 |     0 |     1 |
| AI Generativa e LLMs para melhorar produtos externos                                                                              |     862 |  0.277262   | 0.447907  |     0 |     0 |     0 |     1 |     1 |
| AI Generativa e LLMs para melhorar produtos internos para os colaboradores                                                        |     862 |  0.25174    | 0.434265  |     0 |     0 |     0 |     1 |     1 |
| AI Generativa e LLMs para melhorar produtos internos para os colaboradores                                                        |    3772 |  0.158802   | 0.36554   |     0 |     0 |     0 |     0 |     1 |
| IA Generativa e LLMs como principal frente do negócio                                                                             |     862 |  0.0614849  | 0.240357  |     0 |     0 |     0 |     0 |     1 |
| IA Generativa e LLMs como principal frente do negócio                                                                             |    3772 |  0.0387063  | 0.19292   |     0 |     0 |     0 |     0 |     1 |
| IA Generativa e LLMs não é prioridade                                                                                             |     862 |  0.208817   | 0.406699  |     0 |     0 |     0 |     0 |     1 |
| IA Generativa e LLMs não é prioridade                                                                                             |    3772 |  0.208112   | 0.406011  |     0 |     0 |     0 |     0 |     1 |
| Não sei opinar sobre o uso de IA Generativa e LLMs na empresa                                                                     |     862 |  0.167053   | 0.37324   |     0 |     0 |     0 |     0 |     1 |
| Não sei opinar sobre o uso de IA Generativa e LLMs na empresa                                                                     |    3772 |  0.135207   | 0.34199   |     0 |     0 |     0 |     0 |     1 |
| Falta de compreensão dos casos de uso                                                                                             |     823 |  0.368165   | 0.4826    |     0 |     0 |     0 |     1 |     1 |
| Falta de confiabilidade das saídas (alucinação dos modelos                                                                        |     823 |  0.156744   | 0.36378   |     0 |     0 |     0 |     0 |     1 |
| Incerteza em relação a regulamentação                                                                                             |     823 |  0.144593   | 0.351904  |     0 |     0 |     0 |     0 |     1 |
| Preocupações com segurança e privacidade de dados                                                                                 |     823 |  0.318348   | 0.466118  |     0 |     0 |     0 |     1 |     1 |
| Retorno sobre investimento (ROI) não comprovado de IA Generativa                                                                  |     823 |  0.153098   | 0.360301  |     0 |     0 |     0 |     0 |     1 |
| Dados da empresa não estão prontos para uso de IA Generativa                                                                      |     823 |  0.306197   | 0.461193  |     0 |     0 |     0 |     1 |     1 |
| Falta de expertise ou falta de recursos                                                                                           |     823 |  0.347509   | 0.476469  |     0 |     0 |     0 |     1 |     1 |
| Alta direção da empresa não vê valor ou não vê como prioridade                                                                    |     823 |  0.108141   | 0.310747  |     0 |     0 |     0 |     0 |     1 |
| Preocupações com propriedade intelectual                                                                                          |     823 |  0.147023   | 0.354344  |     0 |     0 |     0 |     0 |     1 |
| Dados relacionais (estruturados em bancos SQL                                                                                     |    3772 |  0.898197   | 0.302429  |     0 |     1 |     1 |     1 |     1 |
| Dados relacionais (estruturados em bancos SQL                                                                                     |    3772 |  0.794008   | 0.404478  |     0 |     1 |     1 |     1 |     1 |
| Dados armazenados em bancos NoSQL                                                                                                 |    3772 |  0.362407   | 0.480759  |     0 |     0 |     0 |     1 |     1 |
| Dados armazenados em bancos NoSQL                                                                                                 |    3772 |  0.133351   | 0.339999  |     0 |     0 |     0 |     0 |     1 |
| Imagens                                                                                                                           |    3772 |  0.152704   | 0.35975   |     0 |     0 |     0 |     0 |     1 |
| Imagens                                                                                                                           |    3772 |  0.0185578  | 0.134975  |     0 |     0 |     0 |     0 |     1 |
| Textos/Documentos                                                                                                                 |    3772 |  0.577147   | 0.494078  |     0 |     0 |     1 |     1 |     1 |
| Textos/Documentos                                                                                                                 |    3772 |  0.135207   | 0.34199   |     0 |     0 |     0 |     0 |     1 |
| Vídeos                                                                                                                            |    3772 |  0.040562   | 0.197299  |     0 |     0 |     0 |     0 |     1 |
| Vídeos                                                                                                                            |    3772 |  0.00636267 | 0.0795227 |     0 |     0 |     0 |     0 |     1 |
| Áudios                                                                                                                            |    3772 |  0.0421527  | 0.200964  |     0 |     0 |     0 |     0 |     1 |
| Áudios                                                                                                                            |    3772 |  0.00371156 | 0.0608175 |     0 |     0 |     0 |     0 |     1 |
| Planilhas                                                                                                                         |    3772 |  0.909067   | 0.287552  |     0 |     1 |     1 |     1 |     1 |
| Planilhas                                                                                                                         |    3772 |  0.575292   | 0.494364  |     0 |     0 |     1 |     1 |     1 |
| Dados georeferenciados                                                                                                            |    3772 |  0.302227   | 0.459284  |     0 |     0 |     0 |     1 |     1 |
| Dados georeferenciados                                                                                                            |    3772 |  0.0233298  | 0.150969  |     0 |     0 |     0 |     0 |     1 |
| Dados relacionais (estruturados em bancos SQL                                                                                     |    3772 |  0.898197   | 0.302429  |     0 |     1 |     1 |     1 |     1 |
| Dados relacionais (estruturados em bancos SQL                                                                                     |    3772 |  0.794008   | 0.404478  |     0 |     1 |     1 |     1 |     1 |
| Dados armazenados em bancos NoSQL                                                                                                 |    3772 |  0.362407   | 0.480759  |     0 |     0 |     0 |     1 |     1 |
| Dados armazenados em bancos NoSQL                                                                                                 |    3772 |  0.133351   | 0.339999  |     0 |     0 |     0 |     0 |     1 |
| Imagens                                                                                                                           |    3772 |  0.152704   | 0.35975   |     0 |     0 |     0 |     0 |     1 |
| Imagens                                                                                                                           |    3772 |  0.0185578  | 0.134975  |     0 |     0 |     0 |     0 |     1 |
| Textos/Documentos                                                                                                                 |    3772 |  0.577147   | 0.494078  |     0 |     0 |     1 |     1 |     1 |
| Textos/Documentos                                                                                                                 |    3772 |  0.135207   | 0.34199   |     0 |     0 |     0 |     0 |     1 |
| Vídeos                                                                                                                            |    3772 |  0.040562   | 0.197299  |     0 |     0 |     0 |     0 |     1 |
| Vídeos                                                                                                                            |    3772 |  0.00636267 | 0.0795227 |     0 |     0 |     0 |     0 |     1 |
| Áudios                                                                                                                            |    3772 |  0.0421527  | 0.200964  |     0 |     0 |     0 |     0 |     1 |
| Áudios                                                                                                                            |    3772 |  0.00371156 | 0.0608175 |     0 |     0 |     0 |     0 |     1 |
| Planilhas                                                                                                                         |    3772 |  0.909067   | 0.287552  |     0 |     1 |     1 |     1 |     1 |
| Planilhas                                                                                                                         |    3772 |  0.575292   | 0.494364  |     0 |     0 |     1 |     1 |     1 |
| Dados georeferenciados                                                                                                            |    3772 |  0.302227   | 0.459284  |     0 |     0 |     0 |     1 |     1 |
| Dados georeferenciados                                                                                                            |    3772 |  0.0233298  | 0.150969  |     0 |     0 |     0 |     0 |     1 |
| SQL                                                                                                                               |    3772 |  0.836691   | 0.369696  |     0 |     1 |     1 |     1 |     1 |
| R                                                                                                                                 |    3772 |  0.108165   | 0.31063   |     0 |     0 |     0 |     0 |     1 |
| Python                                                                                                                            |    3772 |  0.74894    | 0.433681  |     0 |     0 |     1 |     1 |     1 |
| C/C++/C#                                                                                                                          |    3772 |  0.0185578  | 0.134975  |     0 |     0 |     0 |     0 |     1 |
| .NET                                                                                                                              |    3772 |  0.0106045  | 0.102444  |     0 |     0 |     0 |     0 |     1 |
| Java                                                                                                                              |    3772 |  0.0941145  | 0.292027  |     0 |     0 |     0 |     0 |     1 |
| Julia                                                                                                                             |    3772 |  0.00212089 | 0.0460104 |     0 |     0 |     0 |     0 |     1 |
| SAS/Stata                                                                                                                         |    3772 |  0.0400318  | 0.19606   |     0 |     0 |     0 |     0 |     1 |
| Visual Basic/VBA                                                                                                                  |    3772 |  0.0755567  | 0.264323  |     0 |     0 |     0 |     0 |     1 |
| Scala                                                                                                                             |    3772 |  0.0347296  | 0.183118  |     0 |     0 |     0 |     0 |     1 |
| Matlab                                                                                                                            |    3772 |  0.00795334 | 0.0888379 |     0 |     0 |     0 |     0 |     1 |
| Rust                                                                                                                              |    3772 |  0.00185578 | 0.0430445 |     0 |     0 |     0 |     0 |     1 |
| PHP                                                                                                                               |    3772 |  0.0148462  | 0.120953  |     0 |     0 |     0 |     0 |     1 |
| JavaScript                                                                                                                        |    3772 |  0.0747614  | 0.263041  |     0 |     0 |     0 |     0 |     1 |
| Não utilizo nenhuma linguagem                                                                                                     |    3772 |  0.080859   | 0.272655  |     0 |     0 |     0 |     0 |     1 |
| MySQL                                                                                                                             |    3772 |  0.245758   | 0.430593  |     0 |     0 |     0 |     0 |     1 |
| Oracle                                                                                                                            |    3772 |  0.181866   | 0.385786  |     0 |     0 |     0 |     0 |     1 |
| SQL SERVER                                                                                                                        |    3772 |  0.32052    | 0.466738  |     0 |     0 |     0 |     1 |     1 |
| Amazon Aurora ou RDS                                                                                                              |    3772 |  0.0638918  | 0.244593  |     0 |     0 |     0 |     0 |     1 |
| DynamoDB                                                                                                                          |    3772 |  0.0551432  | 0.22829   |     0 |     0 |     0 |     0 |     1 |
| CoachDB                                                                                                                           |    3772 |  0.00106045 | 0.0325515 |     0 |     0 |     0 |     0 |     1 |
| Cassandra                                                                                                                         |    3772 |  0.0111347  | 0.104946  |     0 |     0 |     0 |     0 |     1 |
| MongoDB                                                                                                                           |    3772 |  0.113468   | 0.317206  |     0 |     0 |     0 |     0 |     1 |
| MariaDB                                                                                                                           |    3772 |  0.0328738  | 0.17833   |     0 |     0 |     0 |     0 |     1 |
| Datomic                                                                                                                           |    3772 |  0.00530223 | 0.0726327 |     0 |     0 |     0 |     0 |     1 |
| S3                                                                                                                                |    3772 |  0.209173   | 0.406772  |     0 |     0 |     0 |     0 |     1 |
| PostgreSQL                                                                                                                        |    3772 |  0.283139   | 0.450583  |     0 |     0 |     0 |     1 |     1 |
| ElasticSearch                                                                                                                     |    3772 |  0.0395016  | 0.194811  |     0 |     0 |     0 |     0 |     1 |
| DB2                                                                                                                               |    3772 |  0.0265111  | 0.160671  |     0 |     0 |     0 |     0 |     1 |
| Microsoft Access                                                                                                                  |    3772 |  0.0341994  | 0.181765  |     0 |     0 |     0 |     0 |     1 |
| SQLite                                                                                                                            |    3772 |  0.0474549  | 0.212638  |     0 |     0 |     0 |     0 |     1 |
| Sybase                                                                                                                            |    3772 |  0.00768823 | 0.0873564 |     0 |     0 |     0 |     0 |     1 |
| Firebase                                                                                                                          |    3772 |  0.0275716  | 0.163764  |     0 |     0 |     0 |     0 |     1 |
| Vertica                                                                                                                           |    3772 |  0.00291622 | 0.0539304 |     0 |     0 |     0 |     0 |     1 |
| Redis                                                                                                                             |    3772 |  0.0265111  | 0.160671  |     0 |     0 |     0 |     0 |     1 |
| Neo4J                                                                                                                             |    3772 |  0.00901379 | 0.0945246 |     0 |     0 |     0 |     0 |     1 |
| Google BigQuery                                                                                                                   |    3772 |  0.260604   | 0.439023  |     0 |     0 |     0 |     1 |     1 |
| Google Firestore                                                                                                                  |    3772 |  0.0172322  | 0.130153  |     0 |     0 |     0 |     0 |     1 |
| Amazon Redshift                                                                                                                   |    3772 |  0.109756   | 0.312627  |     0 |     0 |     0 |     0 |     1 |
| Amazon Athena                                                                                                                     |    3772 |  0.119565   | 0.324495  |     0 |     0 |     0 |     0 |     1 |
| Snowflake                                                                                                                         |    3772 |  0.0583245  | 0.234387  |     0 |     0 |     0 |     0 |     1 |
| Databricks                                                                                                                        |    3772 |  0.213945   | 0.410143  |     0 |     0 |     0 |     0 |     1 |
| Databricks                                                                                                                        |     912 |  0.319079   | 0.466375  |     0 |     0 |     0 |     1 |     1 |
| Databricks                                                                                                                        |    1795 |  0.148189   | 0.355387  |     0 |     0 |     0 |     0 |     1 |
| HBase                                                                                                                             |    3772 |  0.00636267 | 0.0795227 |     0 |     0 |     0 |     0 |     1 |
| Presto                                                                                                                            |    3772 |  0.0368505  | 0.18842   |     0 |     0 |     0 |     0 |     1 |
| Splunk                                                                                                                            |    3772 |  0.0129905  | 0.113248  |     0 |     0 |     0 |     0 |     1 |
| SAP HANA                                                                                                                          |    3772 |  0.0559385  | 0.229833  |     0 |     0 |     0 |     0 |     1 |
| Hive                                                                                                                              |    3772 |  0.0782078  | 0.268534  |     0 |     0 |     0 |     0 |     1 |
| Firebird                                                                                                                          |    3772 |  0.0113998  | 0.106174  |     0 |     0 |     0 |     0 |     1 |
| Azure (Microsoft                                                                                                                  |    3613 |  0.423194   | 0.494134  |     0 |     0 |     0 |     1 |     1 |
| Amazon Web Services (AWS                                                                                                          |    3613 |  0.306117   | 0.460943  |     0 |     0 |     0 |     1 |     1 |
| Google Cloud (GCP                                                                                                                 |    3613 |  0.315804   | 0.4649    |     0 |     0 |     0 |     1 |     1 |
| Oracle Cloud                                                                                                                      |    3613 |  0.0426239  | 0.202036  |     0 |     0 |     0 |     0 |     1 |
| IBM                                                                                                                               |    3613 |  0.0130086  | 0.113327  |     0 |     0 |     0 |     0 |     1 |
| Servidores On Premise/Não utilizamos Cloud                                                                                        |    3613 |  0.161085   | 0.36766   |     0 |     0 |     0 |     0 |     1 |
| Cloud Própria                                                                                                                     |    3613 |  0.0694714  | 0.254289  |     0 |     0 |     0 |     0 |     1 |
| Microsoft PowerBI                                                                                                                 |    3772 |  0.57105    | 0.494992  |     0 |     0 |     1 |     1 |     1 |
| Qlik View/Qlik Sense                                                                                                              |    3772 |  0.0514316  | 0.220906  |     0 |     0 |     0 |     0 |     1 |
| Tableau                                                                                                                           |    3772 |  0.189024   | 0.39158   |     0 |     0 |     0 |     0 |     1 |
| Metabase                                                                                                                          |    3772 |  0.0858961  | 0.280248  |     0 |     0 |     0 |     0 |     1 |
| Superset                                                                                                                          |    3772 |  0.0225345  | 0.148433  |     0 |     0 |     0 |     0 |     1 |
| Redash                                                                                                                            |    3772 |  0.0164369  | 0.127165  |     0 |     0 |     0 |     0 |     1 |
| Looker                                                                                                                            |    3772 |  0.23807    | 0.425959  |     0 |     0 |     0 |     0 |     1 |
| Looker Studio(Google Data Studio                                                                                                  |    3772 |  0.173118   | 0.378399  |     0 |     0 |     0 |     0 |     1 |
| Amazon Quicksight                                                                                                                 |    3772 |  0.0365854  | 0.187766  |     0 |     0 |     0 |     0 |     1 |
| Mode                                                                                                                              |    3772 |  0.00344645 | 0.058613  |     0 |     0 |     0 |     0 |     1 |
| Alteryx                                                                                                                           |    3772 |  0.0265111  | 0.160671  |     0 |     0 |     0 |     0 |     1 |
| Alteryx                                                                                                                           |     912 |  0.0186404  | 0.135325  |     0 |     0 |     0 |     0 |     1 |
| Alteryx                                                                                                                           |    1795 |  0.032312   | 0.176877  |     0 |     0 |     0 |     0 |     1 |
| MicroStrategy                                                                                                                     |    3772 |  0.00980912 | 0.0985671 |     0 |     0 |     0 |     0 |     1 |
| IBM Analytics/Cognos                                                                                                              |    3772 |  0.00662778 | 0.0811517 |     0 |     0 |     0 |     0 |     1 |
| SAP Business Objects/SAP Analytics                                                                                                |    3772 |  0.0212089  | 0.144099  |     0 |     0 |     0 |     0 |     1 |
| Oracle Business Intelligence                                                                                                      |    3772 |  0.0129905  | 0.113248  |     0 |     0 |     0 |     0 |     1 |
| Salesforce/Einstein Analytics                                                                                                     |    3772 |  0.0225345  | 0.148433  |     0 |     0 |     0 |     0 |     1 |
| Birst                                                                                                                             |    3772 |  0.00132556 | 0.0363889 |     0 |     0 |     0 |     0 |     1 |
| SAS Visual Analytics                                                                                                              |    3772 |  0.0225345  | 0.148433  |     0 |     0 |     0 |     0 |     1 |
| Grafana                                                                                                                           |    3772 |  0.0731707  | 0.260451  |     0 |     0 |     0 |     0 |     1 |
| TIBCO Spotfire                                                                                                                    |    3772 |  0.00715801 | 0.0843128 |     0 |     0 |     0 |     0 |     1 |
| Pentaho                                                                                                                           |    3772 |  0.0466596  | 0.210937  |     0 |     0 |     0 |     0 |     1 |
| Pentaho                                                                                                                           |     912 |  0.066886   | 0.249961  |     0 |     0 |     0 |     0 |     1 |
| Pentaho                                                                                                                           |    1795 |  0.0618384  | 0.240929  |     0 |     0 |     0 |     0 |     1 |
| Fazemos todas as análises utilizando apenas Excel ou planilhas do google                                                          |    3772 |  0.103659   | 0.304857  |     0 |     0 |     0 |     0 |     1 |
| Não utilizo nenhuma ferramenta de BI no trabalho                                                                                  |    3772 |  0.108431   | 0.310965  |     0 |     0 |     0 |     0 |     1 |
| Colaboradores usando AI generativa de forma independente e descentralizada                                                        |     862 |  0.351508   | 0.477718  |     0 |     0 |     0 |     1 |     1 |
| Colaboradores usando AI generativa de forma independente e descentralizada                                                        |    3772 |  0.456787   | 0.498195  |     0 |     0 |     0 |     1 |     1 |
| Direcionamento centralizado do uso de AI generativa                                                                               |     862 |  0.13109    | 0.337695  |     0 |     0 |     0 |     0 |     1 |
| Direcionamento centralizado do uso de AI generativa                                                                               |    3772 |  0.104454   | 0.305889  |     0 |     0 |     0 |     0 |     1 |
| Desenvolvedores utilizando Copilots                                                                                               |     862 |  0.215777   | 0.411599  |     0 |     0 |     0 |     0 |     1 |
| Desenvolvedores utilizando Copilots                                                                                               |    3772 |  0.153234   | 0.360261  |     0 |     0 |     0 |     0 |     1 |
| AI Generativa e LLMs para melhorar produtos externos para os clientes finais                                                      |    3772 |  0.211824   | 0.408655  |     0 |     0 |     0 |     0 |     1 |
| AI Generativa e LLMs para melhorar produtos internos para os colaboradores                                                        |     862 |  0.25174    | 0.434265  |     0 |     0 |     0 |     1 |     1 |
| AI Generativa e LLMs para melhorar produtos internos para os colaboradores                                                        |    3772 |  0.158802   | 0.36554   |     0 |     0 |     0 |     0 |     1 |
| IA Generativa e LLMs como principal frente do negócio                                                                             |     862 |  0.0614849  | 0.240357  |     0 |     0 |     0 |     0 |     1 |
| IA Generativa e LLMs como principal frente do negócio                                                                             |    3772 |  0.0387063  | 0.19292   |     0 |     0 |     0 |     0 |     1 |
| IA Generativa e LLMs não é prioridade                                                                                             |     862 |  0.208817   | 0.406699  |     0 |     0 |     0 |     0 |     1 |
| IA Generativa e LLMs não é prioridade                                                                                             |    3772 |  0.208112   | 0.406011  |     0 |     0 |     0 |     0 |     1 |
| Não sei opinar sobre o uso de IA Generativa e LLMs na empresa                                                                     |     862 |  0.167053   | 0.37324   |     0 |     0 |     0 |     0 |     1 |
| Não sei opinar sobre o uso de IA Generativa e LLMs na empresa                                                                     |    3772 |  0.135207   | 0.34199   |     0 |     0 |     0 |     0 |     1 |
| Não uso soluções de AI Generativa com foco em produtividade                                                                       |    3772 |  0.197243   | 0.39797   |     0 |     0 |     0 |     0 |     1 |
| Uso soluções gratuitas de AI Generativa com foco em produtividade                                                                 |    3772 |  0.636532   | 0.481062  |     0 |     0 |     1 |     1 |     1 |
| Uso e pago pelas soluções de AI Generativa com foco em produtividade                                                              |    3772 |  0.0691941  | 0.253817  |     0 |     0 |     0 |     0 |     1 |
| A empresa que trabalho paga pelas soluções de AI Generativa com foco em produtividade                                             |    3772 |  0.0636267  | 0.244119  |     0 |     0 |     0 |     0 |     1 |
| Uso soluções do tipo Copilot                                                                                                      |    3772 |  0.117709   | 0.322306  |     0 |     0 |     0 |     0 |     1 |
| Desenvolvo pipelines de dados utilizando linguagens de programação como Python                                                    |     912 |  0.791667   | 0.406339  |     0 |     1 |     1 |     1 |     1 |
| Realizo construções de ETLs em ferramentas como Pentaho                                                                           |     912 |  0.382675   | 0.486307  |     0 |     0 |     0 |     1 |     1 |
| Crio consultas através da linguagem SQL para exportar informações e compartilhar com as áreas de negócio.                         |     912 |  0.747807   | 0.43451   |     0 |     0 |     1 |     1 |     1 |
| Crio consultas através da linguagem SQL para exportar informações e compartilhar com as áreas de negócio.                         |    1795 |  0.709749   | 0.454004  |     0 |     0 |     1 |     1 |     1 |
| Atuo na integração de diferentes fontes de dados através de plataformas proprietárias como Stitch Data                            |     912 |  0.173246   | 0.378667  |     0 |     0 |     0 |     0 |     1 |
| Modelo soluções de arquitetura de dados                                                                                           |     912 |  0.529605   | 0.499397  |     0 |     0 |     1 |     1 |     1 |
| Desenvolvo/cuido da manutenção de repositórios de dados baseados em streaming de eventos como Data Lakes e Data Lakehouses.       |     912 |  0.364035   | 0.481423  |     0 |     0 |     0 |     1 |     1 |
| Atuo na modelagem dos dados                                                                                                       |     912 |  0.605263   | 0.489062  |     0 |     0 |     1 |     1 |     1 |
| Atuo na modelagem dos dados                                                                                                       |    1795 |  0.247354   | 0.431594  |     0 |     0 |     0 |     0 |     1 |
| Cuido da qualidade dos dados                                                                                                      |     912 |  0.527412   | 0.499522  |     0 |     0 |     1 |     1 |     1 |
| Nenhuma das opções listadas refletem meu dia a dia.                                                                               |     912 |  0.0175439  | 0.131358  |     0 |     0 |     0 |     0 |     1 |
| Nenhuma das opções listadas refletem meu dia a dia.                                                                               |     912 |  0.0339912  | 0.181306  |     0 |     0 |     0 |     0 |     1 |
| Nenhuma das opções listadas refletem meu dia a dia.                                                                               |    1795 |  0.0233983  | 0.151207  |     0 |     0 |     0 |     0 |     1 |
| Nenhuma das opções listadas refletem meu dia a dia.                                                                               |    1795 |  0.0534819  | 0.225055  |     0 |     0 |     0 |     0 |     1 |
| Scripts Python                                                                                                                    |     912 |  0.794956   | 0.403955  |     0 |     1 |     1 |     1 |     1 |
| Scripts Python                                                                                                                    |    1795 |  0.464624   | 0.498886  |     0 |     0 |     0 |     1 |     1 |
| SQL & Stored Procedures                                                                                                           |     912 |  0.666667   | 0.471663  |     0 |     0 |     1 |     1 |     1 |
| SQL & Stored Procedures                                                                                                           |    1795 |  0.48468    | 0.499905  |     0 |     0 |     0 |     1 |     1 |
| Apache Airflow                                                                                                                    |     912 |  0.450658   | 0.497832  |     0 |     0 |     0 |     1 |     1 |
| Apache Airflow                                                                                                                    |    1795 |  0.0802228  | 0.271714  |     0 |     0 |     0 |     0 |     1 |
| Apache NiFi                                                                                                                       |     912 |  0.0416667  | 0.199936  |     0 |     0 |     0 |     0 |     1 |
| Apache NiFi                                                                                                                       |    1795 |  0.00668524 | 0.0815122 |     0 |     0 |     0 |     0 |     1 |
| Luigi                                                                                                                             |     912 |  0.00438596 | 0.0661175 |     0 |     0 |     0 |     0 |     1 |
| Luigi                                                                                                                             |    1795 |  0.00111421 | 0.0333704 |     0 |     0 |     0 |     0 |     1 |
| AWS Glue                                                                                                                          |     912 |  0.200658   | 0.400712  |     0 |     0 |     0 |     0 |     1 |
| AWS Glue                                                                                                                          |    1795 |  0.0256267  | 0.158063  |     0 |     0 |     0 |     0 |     1 |
| Talend                                                                                                                            |     912 |  0.0164474  | 0.127258  |     0 |     0 |     0 |     0 |     1 |
| Talend                                                                                                                            |    1795 |  0.0116992  | 0.107558  |     0 |     0 |     0 |     0 |     1 |
| Pentaho                                                                                                                           |    3772 |  0.0466596  | 0.210937  |     0 |     0 |     0 |     0 |     1 |
| Pentaho                                                                                                                           |     912 |  0.066886   | 0.249961  |     0 |     0 |     0 |     0 |     1 |
| Pentaho                                                                                                                           |    1795 |  0.0618384  | 0.240929  |     0 |     0 |     0 |     0 |     1 |
| Alteryx                                                                                                                           |    3772 |  0.0265111  | 0.160671  |     0 |     0 |     0 |     0 |     1 |
| Alteryx                                                                                                                           |     912 |  0.0186404  | 0.135325  |     0 |     0 |     0 |     0 |     1 |
| Alteryx                                                                                                                           |    1795 |  0.032312   | 0.176877  |     0 |     0 |     0 |     0 |     1 |
| Stitch                                                                                                                            |     912 |  0.0175439  | 0.131358  |     0 |     0 |     0 |     0 |     1 |
| Stitch                                                                                                                            |    1795 |  0.00668524 | 0.0815122 |     0 |     0 |     0 |     0 |     1 |
| Fivetran                                                                                                                          |     912 |  0.0241228  | 0.153515  |     0 |     0 |     0 |     0 |     1 |
| Fivetran                                                                                                                          |    1795 |  0.00334262 | 0.0577348 |     0 |     0 |     0 |     0 |     1 |
| Google Dataflow                                                                                                                   |     912 |  0.110746   | 0.313989  |     0 |     0 |     0 |     0 |     1 |
| Google Dataflow                                                                                                                   |    1795 |  0.0194986  | 0.138308  |     0 |     0 |     0 |     0 |     1 |
| Oracle Data Integrator                                                                                                            |     912 |  0.0131579  | 0.114013  |     0 |     0 |     0 |     0 |     1 |
| Oracle Data Integrator                                                                                                            |    1795 |  0.0100279  | 0.0996636 |     0 |     0 |     0 |     0 |     1 |
| IBM DataStage                                                                                                                     |     912 |  0.00986842 | 0.0989028 |     0 |     0 |     0 |     0 |     1 |
| IBM DataStage                                                                                                                     |    1795 |  0.00167131 | 0.0408589 |     0 |     0 |     0 |     0 |     1 |
| SAP BW ETL                                                                                                                        |     912 |  0.0153509  | 0.123011  |     0 |     0 |     0 |     0 |     1 |
| SAP BW ETL                                                                                                                        |    1795 |  0.010585   | 0.102366  |     0 |     0 |     0 |     0 |     1 |
| SQL Server Integration Services (SSIS                                                                                             |     912 |  0.0964912  | 0.295426  |     0 |     0 |     0 |     0 |     1 |
| SQL Server Integration Services (SSIS                                                                                             |    1795 |  0.0735376  | 0.26109   |     0 |     0 |     0 |     0 |     1 |
| SAS Data Integration                                                                                                              |     912 |  0.00986842 | 0.0989028 |     0 |     0 |     0 |     0 |     1 |
| SAS Data Integration                                                                                                              |    1795 |  0.0194986  | 0.138308  |     0 |     0 |     0 |     0 |     1 |
| Qlik Sense                                                                                                                        |     912 |  0.0164474  | 0.127258  |     0 |     0 |     0 |     0 |     1 |
| Qlik Sense                                                                                                                        |    1795 |  0.032312   | 0.176877  |     0 |     0 |     0 |     0 |     1 |
| Knime                                                                                                                             |     912 |  0.00877193 | 0.0932981 |     0 |     0 |     0 |     0 |     1 |
| Knime                                                                                                                             |    1795 |  0.0183844  | 0.134374  |     0 |     0 |     0 |     0 |     1 |
| Databricks                                                                                                                        |    3772 |  0.213945   | 0.410143  |     0 |     0 |     0 |     0 |     1 |
| Databricks                                                                                                                        |     912 |  0.319079   | 0.466375  |     0 |     0 |     0 |     1 |     1 |
| Databricks                                                                                                                        |    1795 |  0.148189   | 0.355387  |     0 |     0 |     0 |     0 |     1 |
| Não utilizo ferramentas de ETL                                                                                                    |     912 |  0.0186404  | 0.135325  |     0 |     0 |     0 |     0 |     1 |
| Não utilizo ferramentas de ETL                                                                                                    |    1795 |  0.1961     | 0.397156  |     0 |     0 |     0 |     0 |     1 |
| Sua organização possui um Data Lake?                                                                                              |     911 |  0.824369   | 0.380715  |     0 |     1 |     1 |     1 |     1 |
| Sua organização possui um Data Warehouse?                                                                                         |     909 |  0.830583   | 0.375326  |     0 |     1 |     1 |     1 |     1 |
| Desenvolvendo pipelines de dados utilizando linguagens de programação como Python                                                 |     912 |  0.564693   | 0.496069  |     0 |     0 |     1 |     1 |     1 |
| Realizando construções de ETLs em ferramentas como Pentaho                                                                        |     912 |  0.148026   | 0.355321  |     0 |     0 |     0 |     0 |     1 |
| Criando consultas através da linguagem SQL para exportar informações e compartilhar com as áreas de negócio.                      |     912 |  0.324561   | 0.468468  |     0 |     0 |     0 |     1 |     1 |
| Criando consultas através da linguagem SQL para exportar informações e compartilhar com as áreas de negócio.                      |    1795 |  0.427855   | 0.494906  |     0 |     0 |     0 |     1 |     1 |
| Atuando na integração de diferentes fontes de dados através de plataformas proprietárias como Stitch Data                         |     912 |  0.0307018  | 0.172603  |     0 |     0 |     0 |     0 |     1 |
| Modelando soluções de arquitetura de dados                                                                                        |     912 |  0.20943    | 0.407125  |     0 |     0 |     0 |     0 |     1 |
| Desenvolvendo/cuidando da manutenção de repositórios de dados baseados em streaming de eventos como Data Lakes e Data Lakehouses. |     912 |  0.0986842  | 0.298401  |     0 |     0 |     0 |     0 |     1 |
| Atuando na modelagem dos dados                                                                                                    |     912 |  0.195175   | 0.396553  |     0 |     0 |     0 |     0 |     1 |
| Atuando na modelagem dos dados                                                                                                    |    1795 |  0.0557103  | 0.229425  |     0 |     0 |     0 |     0 |     1 |
| Cuidando da qualidade dos dados                                                                                                   |     912 |  0.108553   | 0.311248  |     0 |     0 |     0 |     0 |     1 |
| Nenhuma das opções listadas refletem meu dia a dia.                                                                               |     912 |  0.0175439  | 0.131358  |     0 |     0 |     0 |     0 |     1 |
| Nenhuma das opções listadas refletem meu dia a dia.                                                                               |     912 |  0.0339912  | 0.181306  |     0 |     0 |     0 |     0 |     1 |
| Nenhuma das opções listadas refletem meu dia a dia.                                                                               |    1795 |  0.0233983  | 0.151207  |     0 |     0 |     0 |     0 |     1 |
| Nenhuma das opções listadas refletem meu dia a dia.                                                                               |    1795 |  0.0534819  | 0.225055  |     0 |     0 |     0 |     0 |     1 |
| Processo e analiso dados utilizando linguagens de programação como Python                                                         |    1795 |  0.495822   | 0.500122  |     0 |     0 |     0 |     1 |     1 |
| Realizo construções de dashboards em ferramentas de BI como PowerBI                                                               |    1795 |  0.840669   | 0.366087  |     0 |     1 |     1 |     1 |     1 |
| Realizo construções de dashboards em ferramentas de BI como PowerBI                                                               |     748 |  0.274064   | 0.44634   |     0 |     0 |     0 |     1 |     1 |
| Crio consultas através da linguagem SQL para exportar informações e compartilhar com as áreas de negócio.                         |     912 |  0.747807   | 0.43451   |     0 |     0 |     1 |     1 |     1 |
| Crio consultas através da linguagem SQL para exportar informações e compartilhar com as áreas de negócio.                         |    1795 |  0.709749   | 0.454004  |     0 |     0 |     1 |     1 |     1 |
| Utilizo APIs para extrair dados e complementar minhas análises.                                                                   |    1795 |  0.284123   | 0.451121  |     0 |     0 |     0 |     1 |     1 |
| Realizo experimentos e estudos utilizando metodologias estatísticas como teste de hipótese                                        |    1795 |  0.214485   | 0.410579  |     0 |     0 |     0 |     0 |     1 |
| Desenvolvo/cuido da manutenção de ETLs utilizando tecnologias como Talend                                                         |    1795 |  0.203343   | 0.402597  |     0 |     0 |     0 |     0 |     1 |
| Atuo na modelagem dos dados                                                                                                       |     912 |  0.605263   | 0.489062  |     0 |     0 |     1 |     1 |     1 |
| Atuo na modelagem dos dados                                                                                                       |    1795 |  0.247354   | 0.431594  |     0 |     0 |     0 |     0 |     1 |
| Desenvolvo/cuido da manutenção de planilhas para atender as áreas de negócio.                                                     |    1795 |  0.430641   | 0.495304  |     0 |     0 |     0 |     1 |     1 |
| Utilizo ferramentas avançadas de estatística como SASS                                                                            |    1795 |  0.0345404  | 0.182663  |     0 |     0 |     0 |     0 |     1 |
| Nenhuma das opções listadas refletem meu dia a dia.                                                                               |     912 |  0.0175439  | 0.131358  |     0 |     0 |     0 |     0 |     1 |
| Nenhuma das opções listadas refletem meu dia a dia.                                                                               |     912 |  0.0339912  | 0.181306  |     0 |     0 |     0 |     0 |     1 |
| Nenhuma das opções listadas refletem meu dia a dia.                                                                               |    1795 |  0.0233983  | 0.151207  |     0 |     0 |     0 |     0 |     1 |
| Nenhuma das opções listadas refletem meu dia a dia.                                                                               |    1795 |  0.0534819  | 0.225055  |     0 |     0 |     0 |     0 |     1 |
| Scripts Python                                                                                                                    |     912 |  0.794956   | 0.403955  |     0 |     1 |     1 |     1 |     1 |
| Scripts Python                                                                                                                    |    1795 |  0.464624   | 0.498886  |     0 |     0 |     0 |     1 |     1 |
| SQL & Stored Procedures                                                                                                           |     912 |  0.666667   | 0.471663  |     0 |     0 |     1 |     1 |     1 |
| SQL & Stored Procedures                                                                                                           |    1795 |  0.48468    | 0.499905  |     0 |     0 |     0 |     1 |     1 |
| Apache Airflow                                                                                                                    |     912 |  0.450658   | 0.497832  |     0 |     0 |     0 |     1 |     1 |
| Apache Airflow                                                                                                                    |    1795 |  0.0802228  | 0.271714  |     0 |     0 |     0 |     0 |     1 |
| Apache NiFi                                                                                                                       |     912 |  0.0416667  | 0.199936  |     0 |     0 |     0 |     0 |     1 |
| Apache NiFi                                                                                                                       |    1795 |  0.00668524 | 0.0815122 |     0 |     0 |     0 |     0 |     1 |
| Luigi                                                                                                                             |     912 |  0.00438596 | 0.0661175 |     0 |     0 |     0 |     0 |     1 |
| Luigi                                                                                                                             |    1795 |  0.00111421 | 0.0333704 |     0 |     0 |     0 |     0 |     1 |
| AWS Glue                                                                                                                          |     912 |  0.200658   | 0.400712  |     0 |     0 |     0 |     0 |     1 |
| AWS Glue                                                                                                                          |    1795 |  0.0256267  | 0.158063  |     0 |     0 |     0 |     0 |     1 |
| Talend                                                                                                                            |     912 |  0.0164474  | 0.127258  |     0 |     0 |     0 |     0 |     1 |
| Talend                                                                                                                            |    1795 |  0.0116992  | 0.107558  |     0 |     0 |     0 |     0 |     1 |
| Pentaho                                                                                                                           |    3772 |  0.0466596  | 0.210937  |     0 |     0 |     0 |     0 |     1 |
| Pentaho                                                                                                                           |     912 |  0.066886   | 0.249961  |     0 |     0 |     0 |     0 |     1 |
| Pentaho                                                                                                                           |    1795 |  0.0618384  | 0.240929  |     0 |     0 |     0 |     0 |     1 |
| Alteryx                                                                                                                           |    3772 |  0.0265111  | 0.160671  |     0 |     0 |     0 |     0 |     1 |
| Alteryx                                                                                                                           |     912 |  0.0186404  | 0.135325  |     0 |     0 |     0 |     0 |     1 |
| Alteryx                                                                                                                           |    1795 |  0.032312   | 0.176877  |     0 |     0 |     0 |     0 |     1 |
| Stitch                                                                                                                            |     912 |  0.0175439  | 0.131358  |     0 |     0 |     0 |     0 |     1 |
| Stitch                                                                                                                            |    1795 |  0.00668524 | 0.0815122 |     0 |     0 |     0 |     0 |     1 |
| Fivetran                                                                                                                          |     912 |  0.0241228  | 0.153515  |     0 |     0 |     0 |     0 |     1 |
| Fivetran                                                                                                                          |    1795 |  0.00334262 | 0.0577348 |     0 |     0 |     0 |     0 |     1 |
| Google Dataflow                                                                                                                   |     912 |  0.110746   | 0.313989  |     0 |     0 |     0 |     0 |     1 |
| Google Dataflow                                                                                                                   |    1795 |  0.0194986  | 0.138308  |     0 |     0 |     0 |     0 |     1 |
| Oracle Data Integrator                                                                                                            |     912 |  0.0131579  | 0.114013  |     0 |     0 |     0 |     0 |     1 |
| Oracle Data Integrator                                                                                                            |    1795 |  0.0100279  | 0.0996636 |     0 |     0 |     0 |     0 |     1 |
| IBM DataStage                                                                                                                     |     912 |  0.00986842 | 0.0989028 |     0 |     0 |     0 |     0 |     1 |
| IBM DataStage                                                                                                                     |    1795 |  0.00167131 | 0.0408589 |     0 |     0 |     0 |     0 |     1 |
| SAP BW ETL                                                                                                                        |     912 |  0.0153509  | 0.123011  |     0 |     0 |     0 |     0 |     1 |
| SAP BW ETL                                                                                                                        |    1795 |  0.010585   | 0.102366  |     0 |     0 |     0 |     0 |     1 |
| SQL Server Integration Services (SSIS                                                                                             |     912 |  0.0964912  | 0.295426  |     0 |     0 |     0 |     0 |     1 |
| SQL Server Integration Services (SSIS                                                                                             |    1795 |  0.0735376  | 0.26109   |     0 |     0 |     0 |     0 |     1 |
| SAS Data Integration                                                                                                              |     912 |  0.00986842 | 0.0989028 |     0 |     0 |     0 |     0 |     1 |
| SAS Data Integration                                                                                                              |    1795 |  0.0194986  | 0.138308  |     0 |     0 |     0 |     0 |     1 |
| Qlik Sense                                                                                                                        |     912 |  0.0164474  | 0.127258  |     0 |     0 |     0 |     0 |     1 |
| Qlik Sense                                                                                                                        |    1795 |  0.032312   | 0.176877  |     0 |     0 |     0 |     0 |     1 |
| Knime                                                                                                                             |     912 |  0.00877193 | 0.0932981 |     0 |     0 |     0 |     0 |     1 |
| Knime                                                                                                                             |    1795 |  0.0183844  | 0.134374  |     0 |     0 |     0 |     0 |     1 |
| Databricks                                                                                                                        |    3772 |  0.213945   | 0.410143  |     0 |     0 |     0 |     0 |     1 |
| Databricks                                                                                                                        |     912 |  0.319079   | 0.466375  |     0 |     0 |     0 |     1 |     1 |
| Databricks                                                                                                                        |    1795 |  0.148189   | 0.355387  |     0 |     0 |     0 |     0 |     1 |
| Não utilizo ferramentas de ETL                                                                                                    |     912 |  0.0186404  | 0.135325  |     0 |     0 |     0 |     0 |     1 |
| Não utilizo ferramentas de ETL                                                                                                    |    1795 |  0.1961     | 0.397156  |     0 |     0 |     0 |     0 |     1 |
| Ferramentas de AutoML como H2O.ai                                                                                                 |    1795 |  0.0267409  | 0.16137   |     0 |     0 |     0 |     0 |     1 |
| ""Point and Click"" Analytics como Alteryx                                                                                        |    1795 |  0.0685237  | 0.252713  |     0 |     0 |     0 |     0 |     1 |
| Product metricts & Insights como Mixpanel                                                                                         |    1795 |  0.0662953  | 0.248867  |     0 |     0 |     0 |     0 |     1 |
| Ferramentas de análise dentro de ferramentas de CRM como Salesforce Einstein Anaytics ou Zendesk dashboards.                      |    1795 |  0.146518   | 0.353723  |     0 |     0 |     0 |     0 |     1 |
| Minha empresa não utiliza essas ferramentas.                                                                                      |    1795 |  0.423955   | 0.494321  |     0 |     0 |     0 |     1 |     1 |
| Não sei informar.                                                                                                                 |    1795 |  0.341504   | 0.474346  |     0 |     0 |     0 |     1 |     1 |
| Processando e analisando dados utilizando linguagens de programação como Python                                                   |    1795 |  0.261838   | 0.439758  |     0 |     0 |     0 |     1 |     1 |
| Realizando construções de dashboards em ferramentas de BI como PowerBI                                                            |    1795 |  0.57883    | 0.493884  |     0 |     0 |     1 |     1 |     1 |
| Realizando construções de dashboards em ferramentas de BI como PowerBI                                                            |     748 |  0.0454545  | 0.208438  |     0 |     0 |     0 |     0 |     1 |
| Criando consultas através da linguagem SQL para exportar informações e compartilhar com as áreas de negócio.                      |     912 |  0.324561   | 0.468468  |     0 |     0 |     0 |     1 |     1 |
| Criando consultas através da linguagem SQL para exportar informações e compartilhar com as áreas de negócio.                      |    1795 |  0.427855   | 0.494906  |     0 |     0 |     0 |     1 |     1 |
| Utilizando APIs para extrair dados e complementar minhas análises.                                                                |    1795 |  0.0272981  | 0.162996  |     0 |     0 |     0 |     0 |     1 |
| Realizando experimentos e estudos utilizando metodologias estatísticas como teste de hipótese                                     |    1795 |  0.0350975  | 0.184078  |     0 |     0 |     0 |     0 |     1 |
| Desenvolvendo/cuidando da manutenção de ETLs utilizando tecnologias como Talend                                                   |    1795 |  0.0495822  | 0.217141  |     0 |     0 |     0 |     0 |     1 |
| Atuando na modelagem dos dados                                                                                                    |     912 |  0.195175   | 0.396553  |     0 |     0 |     0 |     0 |     1 |
| Atuando na modelagem dos dados                                                                                                    |    1795 |  0.0557103  | 0.229425  |     0 |     0 |     0 |     0 |     1 |
| Desenvolvendo/cuidando da manutenção de planilhas do Excel ou Google Sheets para atender as áreas de negócio.                     |    1795 |  0.158774   | 0.365567  |     0 |     0 |     0 |     0 |     1 |
| Utilizando ferramentas avançadas de estatística como SAS                                                                          |    1795 |  0.0116992  | 0.107558  |     0 |     0 |     0 |     0 |     1 |
| Utilizando ferramentas avançadas de estatística como SAS                                                                          |     748 |  0.00935829 | 0.096349  |     0 |     0 |     0 |     0 |     1 |
| Nenhuma das opções listadas refletem meu dia a dia.                                                                               |     912 |  0.0175439  | 0.131358  |     0 |     0 |     0 |     0 |     1 |
| Nenhuma das opções listadas refletem meu dia a dia.                                                                               |     912 |  0.0339912  | 0.181306  |     0 |     0 |     0 |     0 |     1 |
| Nenhuma das opções listadas refletem meu dia a dia.                                                                               |    1795 |  0.0233983  | 0.151207  |     0 |     0 |     0 |     0 |     1 |
| Nenhuma das opções listadas refletem meu dia a dia.                                                                               |    1795 |  0.0534819  | 0.225055  |     0 |     0 |     0 |     0 |     1 |
| Estudos Ad-hoc com o objetivo de confirmar hipóteses                                                                              |     748 |  0.667112   | 0.471562  |     0 |     0 |     1 |     1 |     1 |
| Estudos Ad-hoc com o objetivo de confirmar hipóteses                                                                              |     748 |  0.375668   | 0.484619  |     0 |     0 |     0 |     1 |     1 |
| Sou responsável pela coleta e limpeza dos dados que uso para análise e modelagem.                                                 |     748 |  0.582888   | 0.493412  |     0 |     0 |     1 |     1 |     1 |
| Sou responsável por entrar em contato com os times de negócio para definição do problema                                          |     748 |  0.542781   | 0.4985    |     0 |     0 |     1 |     1 |     1 |
| Desenvolvo modelos de Machine Learning com o objetivo de colocar em produção em sistemas (produtos de dados).                     |     748 |  0.71123    | 0.453494  |     0 |     0 |     1 |     1 |     1 |
| Sou responsável por colocar modelos em produção                                                                                   |     748 |  0.375668   | 0.484619  |     0 |     0 |     0 |     1 |     1 |
| Cuido da manutenção de modelos de Machine Learning já em produção                                                                 |     748 |  0.435829   | 0.496197  |     0 |     0 |     0 |     1 |     1 |
| Realizo construções de dashboards em ferramentas de BI como PowerBI                                                               |    1795 |  0.840669   | 0.366087  |     0 |     1 |     1 |     1 |     1 |
| Realizo construções de dashboards em ferramentas de BI como PowerBI                                                               |     748 |  0.274064   | 0.44634   |     0 |     0 |     0 |     1 |     1 |
| Utilizo ferramentas avançadas de estatística como SAS                                                                             |     748 |  0.0735294  | 0.261178  |     0 |     0 |     0 |     0 |     1 |
| Crio e dou manutenção em ETLs                                                                                                     |     748 |  0.203209   | 0.402656  |     0 |     0 |     0 |     0 |     1 |
| Crio e gerencio soluções de Feature Store e cultura de MLOps.                                                                     |     748 |  0.122995   | 0.328651  |     0 |     0 |     0 |     0 |     1 |
| Sou responsável por criar e manter a infra que meus modelos e soluções rodam (clusters                                            |     748 |  0.118984   | 0.323986  |     0 |     0 |     0 |     0 |     1 |
| Treino e aplico LLMs para solucionar problemas de negócio.                                                                        |     748 |  0.168449   | 0.374515  |     0 |     0 |     0 |     0 |     1 |
| Utilizo modelos de regressão (linear                                                                                              |     748 |  0.735294   | 0.441472  |     0 |     0 |     1 |     1 |     1 |
| Utilizo redes neurais ou modelos baseados em árvore para criar modelos de classificação                                           |     748 |  0.606952   | 0.488754  |     0 |     0 |     1 |     1 |     1 |
| Desenvolvo sistemas de recomendação (RecSys                                                                                       |     748 |  0.108289   | 0.310953  |     0 |     0 |     0 |     0 |     1 |
| Utilizo métodos estatísticos Bayesianos para analisar dados                                                                       |     748 |  0.247326   | 0.431747  |     0 |     0 |     0 |     0 |     1 |
| Utilizo técnicas de NLP (Natural Language Processing) para análisar dados não-estruturados                                        |     748 |  0.338235   | 0.473426  |     0 |     0 |     0 |     1 |     1 |
| Utilizo métodos estatísticos clássicos (Testes de hipótese                                                                        |     748 |  0.552139   | 0.497607  |     0 |     0 |     1 |     1 |     1 |
| Utilizo cadeias de Markov ou HMMs para realizar análises de dados                                                                 |     748 |  0.0588235  | 0.235452  |     0 |     0 |     0 |     0 |     1 |
| Desenvolvo técnicas de Clusterização (K-means                                                                                     |     748 |  0.53877    | 0.498828  |     0 |     0 |     1 |     1 |     1 |
| Realizo previsões através de modelos de Séries Temporais (Time Series                                                             |     748 |  0.385027   | 0.486927  |     0 |     0 |     0 |     1 |     1 |
| Utilizo modelos de Reinforcement Learning (aprendizado por reforço                                                                |     748 |  0.065508   | 0.247586  |     0 |     0 |     0 |     0 |     1 |
| Utilizo modelos de Machine Learning para detecção de fraude                                                                       |     748 |  0.244652   | 0.430169  |     0 |     0 |     0 |     0 |     1 |
| Utilizo métodos de Visão Computacional                                                                                            |     748 |  0.139037   | 0.346217  |     0 |     0 |     0 |     0 |     1 |
| Utilizo modelos de Detecção de Churn                                                                                              |     748 |  0.21123    | 0.408454  |     0 |     0 |     0 |     0 |     1 |
| Utilizo LLMs para solucionar problemas de negócio                                                                                 |     748 |  0.200535   | 0.400668  |     0 |     0 |     0 |     0 |     1 |
| Ferramentas de BI (PowerBI                                                                                                        |     748 |  0.429144   | 0.495285  |     0 |     0 |     0 |     1 |     1 |
| Planilhas (Excel                                                                                                                  |     748 |  0.687166   | 0.463958  |     0 |     0 |     1 |     1 |     1 |
| Ambientes de desenvolvimento local (R-studio                                                                                      |     748 |  0.716578   | 0.450961  |     0 |     0 |     1 |     1 |     1 |
| Ambientes de desenvolvimento na nuvem (Google Colab                                                                               |     748 |  0.574866   | 0.494694  |     0 |     0 |     1 |     1 |     1 |
| Ferramentas de AutoML (Datarobot                                                                                                  |     748 |  0.108289   | 0.310953  |     0 |     0 |     0 |     0 |     1 |
| Ferramentas de ETL (Apache Airflow                                                                                                |     748 |  0.204545   | 0.403639  |     0 |     0 |     0 |     0 |     1 |
| Plataformas de Machine Learning (TensorFlow                                                                                       |     748 |  0.393048   | 0.488754  |     0 |     0 |     0 |     1 |     1 |
| Feature Store (Feast                                                                                                              |     748 |  0.143048   | 0.350356  |     0 |     0 |     0 |     0 |     1 |
| Sistemas de controle de versão (Github                                                                                            |     748 |  0.625668   | 0.484274  |     0 |     0 |     1 |     1 |     1 |
| Plataformas de Data Apps (Streamlit                                                                                               |     748 |  0.237968   | 0.426124  |     0 |     0 |     0 |     0 |     1 |
| Ferramentas de estatística avançada como SPSS                                                                                     |     748 |  0.0802139  | 0.271806  |     0 |     0 |     0 |     0 |     1 |
| Estudos Ad-hoc com o objetivo de confirmar hipóteses                                                                              |     748 |  0.667112   | 0.471562  |     0 |     0 |     1 |     1 |     1 |
| Estudos Ad-hoc com o objetivo de confirmar hipóteses                                                                              |     748 |  0.375668   | 0.484619  |     0 |     0 |     0 |     1 |     1 |
| Coletando e limpando os dados que uso para análise e modelagem.                                                                   |     748 |  0.457219   | 0.4985    |     0 |     0 |     0 |     1 |     1 |
| Entrando em contato com os times de negócio para definição do problema                                                            |     748 |  0.243316   | 0.429371  |     0 |     0 |     0 |     0 |     1 |
| Desenvolvendo modelos de Machine Learning com o objetivo de colocar em produção em sistemas (produtos de dados).                  |     748 |  0.315508   | 0.465029  |     0 |     0 |     0 |     1 |     1 |
| Colocando modelos em produção                                                                                                     |     748 |  0.0708556  | 0.256755  |     0 |     0 |     0 |     0 |     1 |
| Cuidando da manutenção de modelos de Machine Learning já em produção                                                              |     748 |  0.0935829  | 0.291442  |     0 |     0 |     0 |     0 |     1 |
| Realizando construções de dashboards em ferramentas de BI como PowerBI                                                            |    1795 |  0.57883    | 0.493884  |     0 |     0 |     1 |     1 |     1 |
| Realizando construções de dashboards em ferramentas de BI como PowerBI                                                            |     748 |  0.0454545  | 0.208438  |     0 |     0 |     0 |     0 |     1 |
| Utilizando ferramentas avançadas de estatística como SAS                                                                          |    1795 |  0.0116992  | 0.107558  |     0 |     0 |     0 |     0 |     1 |
| Utilizando ferramentas avançadas de estatística como SAS                                                                          |     748 |  0.00935829 | 0.096349  |     0 |     0 |     0 |     0 |     1 |
| Criando e dando manutenção em ETLs                                                                                                |     748 |  0.0254011  | 0.157445  |     0 |     0 |     0 |     0 |     1 |
| Criando e gerenciando soluções de Feature Store e cultura de MLOps.                                                               |     748 |  0.0200535  | 0.140277  |     0 |     0 |     0 |     0 |     1 |
| Criando e mantendo a infra que meus modelos e soluções rodam (clusters                                                            |     748 |  0.0240642  | 0.153351  |     0 |     0 |     0 |     0 |     1 |
| Treinando e aplicando LLMs para solucionar problemas de negócio.                                                                  |     748 |  0.0481283  | 0.214181  |     0 |     0 |     0 |     0 |     1 |

## Agrupamento por Prefixo

### Grupo id
**Quantidade de colunas**: 1

| Colunas |
|----------|
| `id` |

### Grupo Idade
**Quantidade de colunas**: 1

| Colunas |
|----------|
| `Idade` |

### Grupo Faixa idade
**Quantidade de colunas**: 1

| Colunas |
|----------|
| `Faixa idade` |

### Grupo Genero
**Quantidade de colunas**: 1

| Colunas |
|----------|
| `Genero` |

### Grupo Cor/raca/etnia
**Quantidade de colunas**: 1

| Colunas |
|----------|
| `Cor/raca/etnia` |

### Grupo PCD
**Quantidade de colunas**: 1

| Colunas |
|----------|
| `PCD` |

### Grupo experiencia
**Quantidade de colunas**: 1

| Colunas |
|----------|
| `experiencia_profissional_prejudicada` |

### Grupo Não acredito que minha experiência profissional seja afetada
**Quantidade de colunas**: 1

| Colunas |
|----------|
| `Não acredito que minha experiência profissional seja afetada` |

### Grupo Experiencia prejudicada devido a minha Cor Raça Etnia
**Quantidade de colunas**: 1

| Colunas |
|----------|
| `Experiencia prejudicada devido a minha Cor Raça Etnia` |

### Grupo Experiencia prejudicada devido a minha identidade de gênero
**Quantidade de colunas**: 1

| Colunas |
|----------|
| `Experiencia prejudicada devido a minha identidade de gênero` |

### Grupo Experiencia prejudicada devido ao fato de ser PCD
**Quantidade de colunas**: 1

| Colunas |
|----------|
| `Experiencia prejudicada devido ao fato de ser PCD` |

### Grupo aspectos
**Quantidade de colunas**: 1

| Colunas |
|----------|
| `aspectos_prejudicados` |

### Grupo Quantidade de oportunidades de emprego/vagas recebidas
**Quantidade de colunas**: 1

| Colunas |
|----------|
| `Quantidade de oportunidades de emprego/vagas recebidas` |

### Grupo Senioridade das vagas recebidas em relação à sua experiência
**Quantidade de colunas**: 1

| Colunas |
|----------|
| `Senioridade das vagas recebidas em relação à sua experiência` |

### Grupo Aprovação em processos seletivos/entrevistas
**Quantidade de colunas**: 1

| Colunas |
|----------|
| `Aprovação em processos seletivos/entrevistas` |

### Grupo Oportunidades de progressão de carreira
**Quantidade de colunas**: 1

| Colunas |
|----------|
| `Oportunidades de progressão de carreira` |

### Grupo Velocidade de progressão de carreira
**Quantidade de colunas**: 1

| Colunas |
|----------|
| `Velocidade de progressão de carreira` |

### Grupo Nível de cobrança no trabalho/Stress no trabalho
**Quantidade de colunas**: 1

| Colunas |
|----------|
| `Nível de cobrança no trabalho/Stress no trabalho` |

### Grupo Atenção dada diante das minhas opiniões e ideias
**Quantidade de colunas**: 1

| Colunas |
|----------|
| `Atenção dada diante das minhas opiniões e ideias` |

### Grupo Relação com outros membros da empresa
**Quantidade de colunas**: 2

| Colunas |
|----------|
| `Relação com outros membros da empresa` |
| `Relação com outros membros da empresa` |

### Grupo vive
**Quantidade de colunas**: 1

| Colunas |
|----------|
| `vive_no_brasil` |

### Grupo Estado onde mora
**Quantidade de colunas**: 1

| Colunas |
|----------|
| `Estado onde mora` |

### Grupo uf onde mora
**Quantidade de colunas**: 1

| Colunas |
|----------|
| `uf onde mora` |

### Grupo Regiao onde mora
**Quantidade de colunas**: 1

| Colunas |
|----------|
| `Regiao onde mora` |

### Grupo Mudou de Estado?
**Quantidade de colunas**: 1

| Colunas |
|----------|
| `Mudou de Estado?` |

### Grupo Regiao de origem
**Quantidade de colunas**: 1

| Colunas |
|----------|
| `Regiao de origem` |

### Grupo Nivel de Ensino
**Quantidade de colunas**: 1

| Colunas |
|----------|
| `Nivel de Ensino` |

### Grupo Área de Formação
**Quantidade de colunas**: 1

| Colunas |
|----------|
| `Área de Formação` |

### Grupo Qual sua situação atual de trabalho?
**Quantidade de colunas**: 1

| Colunas |
|----------|
| `Qual sua situação atual de trabalho?` |

### Grupo Setor
**Quantidade de colunas**: 1

| Colunas |
|----------|
| `Setor` |

### Grupo Numero de Funcionarios
**Quantidade de colunas**: 1

| Colunas |
|----------|
| `Numero de Funcionarios` |

### Grupo Gestor?
**Quantidade de colunas**: 1

| Colunas |
|----------|
| `Gestor?` |

### Grupo Cargo como Gestor
**Quantidade de colunas**: 1

| Colunas |
|----------|
| `Cargo como Gestor` |

### Grupo Cargo Atual
**Quantidade de colunas**: 1

| Colunas |
|----------|
| `Cargo Atual` |

### Grupo Nivel
**Quantidade de colunas**: 1

| Colunas |
|----------|
| `Nivel` |

### Grupo Faixa salarial
**Quantidade de colunas**: 1

| Colunas |
|----------|
| `Faixa salarial` |

### Grupo Quanto tempo de experiência na área de dados você tem?
**Quantidade de colunas**: 1

| Colunas |
|----------|
| `Quanto tempo de experiência na área de dados você tem?` |

### Grupo Quanto tempo de experiência na área de TI/Engenharia de Software você teve antes de começar a trabalhar na área de dados?
**Quantidade de colunas**: 1

| Colunas |
|----------|
| `Quanto tempo de experiência na área de TI/Engenharia de Software você teve antes de começar a trabalhar na área de dados?` |

### Grupo Você está satisfeito na sua empresa atual?
**Quantidade de colunas**: 1

| Colunas |
|----------|
| `Você está satisfeito na sua empresa atual?` |

### Grupo Qual o principal motivo da sua insatisfação com a empresa atual?
**Quantidade de colunas**: 1

| Colunas |
|----------|
| `Qual o principal motivo da sua insatisfação com a empresa atual?` |

### Grupo Falta de oportunidade de crescimento no emprego atual
**Quantidade de colunas**: 1

| Colunas |
|----------|
| `Falta de oportunidade de crescimento no emprego atual` |

### Grupo Salário atual não corresponde ao mercado
**Quantidade de colunas**: 1

| Colunas |
|----------|
| `Salário atual não corresponde ao mercado` |

### Grupo Não tenho uma boa relação com meu líder/gestor
**Quantidade de colunas**: 1

| Colunas |
|----------|
| `Não tenho uma boa relação com meu líder/gestor` |

### Grupo Gostaria de trabalhar em em outra área de atuação
**Quantidade de colunas**: 1

| Colunas |
|----------|
| `Gostaria de trabalhar em em outra área de atuação` |

### Grupo Gostaria de receber mais benefícios
**Quantidade de colunas**: 1

| Colunas |
|----------|
| `Gostaria de receber mais benefícios` |

### Grupo O clima de trabalho/ambiente não é bom
**Quantidade de colunas**: 1

| Colunas |
|----------|
| `O clima de trabalho/ambiente não é bom` |

### Grupo Falta de maturidade analítica na empresa
**Quantidade de colunas**: 1

| Colunas |
|----------|
| `Falta de maturidade analítica na empresa` |

### Grupo Você participou de entrevistas de emprego nos últimos 6 meses?
**Quantidade de colunas**: 1

| Colunas |
|----------|
| `Você participou de entrevistas de emprego nos últimos 6 meses?` |

### Grupo Você pretende mudar de emprego nos próximos 6 meses?
**Quantidade de colunas**: 1

| Colunas |
|----------|
| `Você pretende mudar de emprego nos próximos 6 meses?` |

### Grupo Quais os principais critérios que você leva em consideração no momento de decidir onde trabalhar?
**Quantidade de colunas**: 1

| Colunas |
|----------|
| `Quais os principais critérios que você leva em consideração no momento de decidir onde trabalhar?` |

### Grupo Remuneração/Salário
**Quantidade de colunas**: 1

| Colunas |
|----------|
| `Remuneração/Salário` |

### Grupo Benefícios
**Quantidade de colunas**: 1

| Colunas |
|----------|
| `Benefícios` |

### Grupo Propósito do trabalho e da empresa
**Quantidade de colunas**: 1

| Colunas |
|----------|
| `Propósito do trabalho e da empresa` |

### Grupo Flexibilidade de trabalho remoto
**Quantidade de colunas**: 1

| Colunas |
|----------|
| `Flexibilidade de trabalho remoto` |

### Grupo Ambiente e clima de trabalho
**Quantidade de colunas**: 1

| Colunas |
|----------|
| `Ambiente e clima de trabalho` |

### Grupo Oportunidade de aprendizado e trabalhar com referências na área
**Quantidade de colunas**: 1

| Colunas |
|----------|
| `Oportunidade de aprendizado e trabalhar com referências na área` |

### Grupo Plano de carreira e oportunidades de crescimento profissional
**Quantidade de colunas**: 1

| Colunas |
|----------|
| `Plano de carreira e oportunidades de crescimento profissional` |

### Grupo Maturidade da empresa em termos de tecnologia e dados
**Quantidade de colunas**: 1

| Colunas |
|----------|
| `Maturidade da empresa em termos de tecnologia e dados` |

### Grupo Qualidade dos gestores e líderes
**Quantidade de colunas**: 1

| Colunas |
|----------|
| `Qualidade dos gestores e líderes` |

### Grupo Reputação que a empresa tem no mercado
**Quantidade de colunas**: 1

| Colunas |
|----------|
| `Reputação que a empresa tem no mercado` |

### Grupo Empresa que trabaha passou por layoff em 2023
**Quantidade de colunas**: 1

| Colunas |
|----------|
| `Empresa que trabaha passou por layoff em 2023` |

### Grupo Atualmente qual a sua forma de trabalho?
**Quantidade de colunas**: 1

| Colunas |
|----------|
| `Atualmente qual a sua forma de trabalho?` |

### Grupo Qual a forma de trabalho ideal para você?
**Quantidade de colunas**: 1

| Colunas |
|----------|
| `Qual a forma de trabalho ideal para você?` |

### Grupo Caso sua empresa decida pelo modelo 100% presencial qual será sua atitude?
**Quantidade de colunas**: 1

| Colunas |
|----------|
| `Caso sua empresa decida pelo modelo 100% presencial qual será sua atitude?` |

### Grupo Qual o número aproximado de pessoas que atuam com dados na sua empresa hoje?
**Quantidade de colunas**: 1

| Colunas |
|----------|
| `Qual o número aproximado de pessoas que atuam com dados na sua empresa hoje?` |

### Grupo Quais desses papéis/cargos fazem parte do time (ou chapter) de dados da sua empresa?
**Quantidade de colunas**: 1

| Colunas |
|----------|
| `Quais desses papéis/cargos fazem parte do time (ou chapter) de dados da sua empresa?` |

### Grupo Analytics Engineer
**Quantidade de colunas**: 1

| Colunas |
|----------|
| `Analytics Engineer` |

### Grupo Engenharia de Dados/Data Engineer
**Quantidade de colunas**: 1

| Colunas |
|----------|
| `Engenharia de Dados/Data Engineer` |

### Grupo Analista de Dados/Data Analyst
**Quantidade de colunas**: 1

| Colunas |
|----------|
| `Analista de Dados/Data Analyst` |

### Grupo Cientista de Dados/Data Scientist
**Quantidade de colunas**: 1

| Colunas |
|----------|
| `Cientista de Dados/Data Scientist` |

### Grupo Database Administrator/DBA
**Quantidade de colunas**: 1

| Colunas |
|----------|
| `Database Administrator/DBA` |

### Grupo Analista de Business Intelligence/BI
**Quantidade de colunas**: 1

| Colunas |
|----------|
| `Analista de Business Intelligence/BI` |

### Grupo Arquiteto de Dados/Data Architect
**Quantidade de colunas**: 1

| Colunas |
|----------|
| `Arquiteto de Dados/Data Architect` |

### Grupo Data Product Manager/DPM
**Quantidade de colunas**: 1

| Colunas |
|----------|
| `Data Product Manager/DPM` |

### Grupo Business Analyst
**Quantidade de colunas**: 1

| Colunas |
|----------|
| `Business Analyst` |

### Grupo Quais dessas responsabilidades fazem parte da sua rotina atual de trabalho como gestor?
**Quantidade de colunas**: 1

| Colunas |
|----------|
| `Quais dessas responsabilidades fazem parte da sua rotina atual de trabalho como gestor?` |

### Grupo Pensar na visão de longo prazo de dados da empresa e fortalecimento da cultura analítica da companhia.
**Quantidade de colunas**: 1

| Colunas |
|----------|
| `Pensar na visão de longo prazo de dados da empresa e fortalecimento da cultura analítica da companhia.` |

### Grupo Organização de treinamentos e iniciativas com o objetivo de aumentar a maturidade analítica das áreas de negócios.
**Quantidade de colunas**: 1

| Colunas |
|----------|
| `Organização de treinamentos e iniciativas com o objetivo de aumentar a maturidade analítica das áreas de negócios.` |

### Grupo Atração
**Quantidade de colunas**: 1

| Colunas |
|----------|
| `Atração` |

### Grupo Decisão sobre contratação de ferramentas e tecnologias relacionadas a dados.
**Quantidade de colunas**: 1

| Colunas |
|----------|
| `Decisão sobre contratação de ferramentas e tecnologias relacionadas a dados.` |

### Grupo Sou gestor da equipe responsável pela engenharia de dados e por manter o Data Lake da empresa como fonte única dos dados
**Quantidade de colunas**: 1

| Colunas |
|----------|
| `Sou gestor da equipe responsável pela engenharia de dados e por manter o Data Lake da empresa como fonte única dos dados` |

### Grupo Sou gestor da equipe responsável pela entrega de dados
**Quantidade de colunas**: 1

| Colunas |
|----------|
| `Sou gestor da equipe responsável pela entrega de dados` |

### Grupo Sou gestor da equipe responsável por iniciativas e projetos envolvendo Inteligência Artificial e Machine Learning.
**Quantidade de colunas**: 1

| Colunas |
|----------|
| `Sou gestor da equipe responsável por iniciativas e projetos envolvendo Inteligência Artificial e Machine Learning.` |

### Grupo Apesar de ser gestor ainda atuo na parte técnica
**Quantidade de colunas**: 1

| Colunas |
|----------|
| `Apesar de ser gestor ainda atuo na parte técnica` |

### Grupo Gestão de projetos de dados
**Quantidade de colunas**: 1

| Colunas |
|----------|
| `Gestão de projetos de dados` |

### Grupo Gestão de produtos de dados
**Quantidade de colunas**: 1

| Colunas |
|----------|
| `Gestão de produtos de dados` |

### Grupo Gestão de pessoas
**Quantidade de colunas**: 1

| Colunas |
|----------|
| `Gestão de pessoas` |

### Grupo Quais são os 3 maiores desafios que você tem como gestor no atual momento?
**Quantidade de colunas**: 1

| Colunas |
|----------|
| `Quais são os 3 maiores desafios que você tem como gestor no atual momento?` |

### Grupo a Contratar novos talentos.
**Quantidade de colunas**: 1

| Colunas |
|----------|
| `a Contratar novos talentos.` |

### Grupo b Reter talentos.
**Quantidade de colunas**: 1

| Colunas |
|----------|
| `b Reter talentos.` |

### Grupo c Convencer a empresa a aumentar os investimentos na área de dados.
**Quantidade de colunas**: 1

| Colunas |
|----------|
| `c Convencer a empresa a aumentar os investimentos na área de dados.` |

### Grupo d Gestão de equipes no ambiente remoto.
**Quantidade de colunas**: 1

| Colunas |
|----------|
| `d Gestão de equipes no ambiente remoto.` |

### Grupo e Gestão de projetos envolvendo áreas multidisciplinares da empresa.
**Quantidade de colunas**: 1

| Colunas |
|----------|
| `e Gestão de projetos envolvendo áreas multidisciplinares da empresa.` |

### Grupo f Organizar as informações e garantir a qualidade e confiabilidade.
**Quantidade de colunas**: 1

| Colunas |
|----------|
| `f Organizar as informações e garantir a qualidade e confiabilidade.` |

### Grupo g Conseguir processar e armazenar um alto volume de dados.
**Quantidade de colunas**: 1

| Colunas |
|----------|
| `g Conseguir processar e armazenar um alto volume de dados.` |

### Grupo h Conseguir gerar valor para as áreas de negócios através de estudos e experimentos.
**Quantidade de colunas**: 1

| Colunas |
|----------|
| `h Conseguir gerar valor para as áreas de negócios através de estudos e experimentos.` |

### Grupo i Desenvolver e manter modelos Machine Learning em produção.
**Quantidade de colunas**: 1

| Colunas |
|----------|
| `i Desenvolver e manter modelos Machine Learning em produção.` |

### Grupo j Gerenciar a expectativa das áreas de negócio em relação as entregas das equipes de dados.
**Quantidade de colunas**: 1

| Colunas |
|----------|
| `j Gerenciar a expectativa das áreas de negócio em relação as entregas das equipes de dados.` |

### Grupo k Garantir a manutenção dos projetos e modelos em produção
**Quantidade de colunas**: 1

| Colunas |
|----------|
| `k Garantir a manutenção dos projetos e modelos em produção` |

### Grupo Conseguir levar inovação para a empresa através dos dados.
**Quantidade de colunas**: 1

| Colunas |
|----------|
| `Conseguir levar inovação para a empresa através dos dados.` |

### Grupo Garantir retorno do investimento (ROI) em projetos de dados.
**Quantidade de colunas**: 1

| Colunas |
|----------|
| `Garantir retorno do investimento (ROI) em projetos de dados.` |

### Grupo Dividir o tempo entre entregas técnicas e gestão.
**Quantidade de colunas**: 1

| Colunas |
|----------|
| `Dividir o tempo entre entregas técnicas e gestão.` |

### Grupo AI Generativa é uma prioridade em sua empresa?
**Quantidade de colunas**: 1

| Colunas |
|----------|
| `AI Generativa é uma prioridade em sua empresa?` |

### Grupo Tipos de uso de AI Generativa e LLMs na empresa
**Quantidade de colunas**: 1

| Colunas |
|----------|
| `Tipos de uso de AI Generativa e LLMs na empresa` |

### Grupo Colaboradores usando AI generativa de forma independente e descentralizada
**Quantidade de colunas**: 2

| Colunas |
|----------|
| `Colaboradores usando AI generativa de forma independente e descentralizada` |
| `Colaboradores usando AI generativa de forma independente e descentralizada` |

### Grupo Direcionamento centralizado do uso de AI generativa
**Quantidade de colunas**: 2

| Colunas |
|----------|
| `Direcionamento centralizado do uso de AI generativa` |
| `Direcionamento centralizado do uso de AI generativa` |

### Grupo Desenvolvedores utilizando Copilots
**Quantidade de colunas**: 2

| Colunas |
|----------|
| `Desenvolvedores utilizando Copilots` |
| `Desenvolvedores utilizando Copilots` |

### Grupo AI Generativa e LLMs para melhorar produtos externos
**Quantidade de colunas**: 1

| Colunas |
|----------|
| `AI Generativa e LLMs para melhorar produtos externos` |

### Grupo AI Generativa e LLMs para melhorar produtos internos para os colaboradores
**Quantidade de colunas**: 2

| Colunas |
|----------|
| `AI Generativa e LLMs para melhorar produtos internos para os colaboradores` |
| `AI Generativa e LLMs para melhorar produtos internos para os colaboradores` |

### Grupo IA Generativa e LLMs como principal frente do negócio
**Quantidade de colunas**: 2

| Colunas |
|----------|
| `IA Generativa e LLMs como principal frente do negócio` |
| `IA Generativa e LLMs como principal frente do negócio` |

### Grupo IA Generativa e LLMs não é prioridade
**Quantidade de colunas**: 2

| Colunas |
|----------|
| `IA Generativa e LLMs não é prioridade` |
| `IA Generativa e LLMs não é prioridade` |

### Grupo Não sei opinar sobre o uso de IA Generativa e LLMs na empresa
**Quantidade de colunas**: 2

| Colunas |
|----------|
| `Não sei opinar sobre o uso de IA Generativa e LLMs na empresa` |
| `Não sei opinar sobre o uso de IA Generativa e LLMs na empresa` |

### Grupo Motivos que levam a empresa a não usar AI Genrativa e LLMs
**Quantidade de colunas**: 1

| Colunas |
|----------|
| `Motivos que levam a empresa a não usar AI Genrativa e LLMs` |

### Grupo Falta de compreensão dos casos de uso
**Quantidade de colunas**: 1

| Colunas |
|----------|
| `Falta de compreensão dos casos de uso` |

### Grupo Falta de confiabilidade das saídas (alucinação dos modelos
**Quantidade de colunas**: 1

| Colunas |
|----------|
| `Falta de confiabilidade das saídas (alucinação dos modelos` |

### Grupo Incerteza em relação a regulamentação
**Quantidade de colunas**: 1

| Colunas |
|----------|
| `Incerteza em relação a regulamentação` |

### Grupo Preocupações com segurança e privacidade de dados
**Quantidade de colunas**: 1

| Colunas |
|----------|
| `Preocupações com segurança e privacidade de dados` |

### Grupo Retorno sobre investimento (ROI) não comprovado de IA Generativa
**Quantidade de colunas**: 1

| Colunas |
|----------|
| `Retorno sobre investimento (ROI) não comprovado de IA Generativa` |

### Grupo Dados da empresa não estão prontos para uso de IA Generativa
**Quantidade de colunas**: 1

| Colunas |
|----------|
| `Dados da empresa não estão prontos para uso de IA Generativa` |

### Grupo Falta de expertise ou falta de recursos
**Quantidade de colunas**: 1

| Colunas |
|----------|
| `Falta de expertise ou falta de recursos` |

### Grupo Alta direção da empresa não vê valor ou não vê como prioridade
**Quantidade de colunas**: 1

| Colunas |
|----------|
| `Alta direção da empresa não vê valor ou não vê como prioridade` |

### Grupo Preocupações com propriedade intelectual
**Quantidade de colunas**: 1

| Colunas |
|----------|
| `Preocupações com propriedade intelectual` |

### Grupo Mesmo que esse não seja seu cargo formal
**Quantidade de colunas**: 1

| Colunas |
|----------|
| `Mesmo que esse não seja seu cargo formal` |

### Grupo Atuacao
**Quantidade de colunas**: 1

| Colunas |
|----------|
| `Atuacao` |

### Grupo Quais das fontes de dados listadas você já analisou ou processou no trabalho?
**Quantidade de colunas**: 1

| Colunas |
|----------|
| `Quais das fontes de dados listadas você já analisou ou processou no trabalho?` |

### Grupo Dados relacionais (estruturados em bancos SQL
**Quantidade de colunas**: 2

| Colunas |
|----------|
| `Dados relacionais (estruturados em bancos SQL` |
| `Dados relacionais (estruturados em bancos SQL` |

### Grupo Dados armazenados em bancos NoSQL
**Quantidade de colunas**: 2

| Colunas |
|----------|
| `Dados armazenados em bancos NoSQL` |
| `Dados armazenados em bancos NoSQL` |

### Grupo Imagens
**Quantidade de colunas**: 2

| Colunas |
|----------|
| `Imagens` |
| `Imagens` |

### Grupo Textos/Documentos
**Quantidade de colunas**: 2

| Colunas |
|----------|
| `Textos/Documentos` |
| `Textos/Documentos` |

### Grupo Vídeos
**Quantidade de colunas**: 2

| Colunas |
|----------|
| `Vídeos` |
| `Vídeos` |

### Grupo Áudios
**Quantidade de colunas**: 2

| Colunas |
|----------|
| `Áudios` |
| `Áudios` |

### Grupo Planilhas
**Quantidade de colunas**: 2

| Colunas |
|----------|
| `Planilhas` |
| `Planilhas` |

### Grupo Dados georeferenciados
**Quantidade de colunas**: 2

| Colunas |
|----------|
| `Dados georeferenciados` |
| `Dados georeferenciados` |

### Grupo Entre as fontes de dados listadas
**Quantidade de colunas**: 1

| Colunas |
|----------|
| `Entre as fontes de dados listadas` |

### Grupo Quais das linguagens listadas abaixo você utiliza no trabalho?
**Quantidade de colunas**: 1

| Colunas |
|----------|
| `Quais das linguagens listadas abaixo você utiliza no trabalho?` |

### Grupo SQL
**Quantidade de colunas**: 1

| Colunas |
|----------|
| `SQL` |

### Grupo R
**Quantidade de colunas**: 1

| Colunas |
|----------|
| `R` |

### Grupo Python
**Quantidade de colunas**: 1

| Colunas |
|----------|
| `Python` |

### Grupo C/C++/C#
**Quantidade de colunas**: 1

| Colunas |
|----------|
| `C/C++/C#` |

### Grupo .NET
**Quantidade de colunas**: 1

| Colunas |
|----------|
| `.NET` |

### Grupo Java
**Quantidade de colunas**: 1

| Colunas |
|----------|
| `Java` |

### Grupo Julia
**Quantidade de colunas**: 1

| Colunas |
|----------|
| `Julia` |

### Grupo SAS/Stata
**Quantidade de colunas**: 1

| Colunas |
|----------|
| `SAS/Stata` |

### Grupo Visual Basic/VBA
**Quantidade de colunas**: 1

| Colunas |
|----------|
| `Visual Basic/VBA` |

### Grupo Scala
**Quantidade de colunas**: 1

| Colunas |
|----------|
| `Scala` |

### Grupo Matlab
**Quantidade de colunas**: 1

| Colunas |
|----------|
| `Matlab` |

### Grupo Rust
**Quantidade de colunas**: 1

| Colunas |
|----------|
| `Rust` |

### Grupo PHP
**Quantidade de colunas**: 1

| Colunas |
|----------|
| `PHP` |

### Grupo JavaScript
**Quantidade de colunas**: 1

| Colunas |
|----------|
| `JavaScript` |

### Grupo Não utilizo nenhuma linguagem
**Quantidade de colunas**: 1

| Colunas |
|----------|
| `Não utilizo nenhuma linguagem` |

### Grupo Entre as linguagens listadas abaixo
**Quantidade de colunas**: 2

| Colunas |
|----------|
| `Entre as linguagens listadas abaixo` |
| `Entre as linguagens listadas abaixo` |

### Grupo Quais dos bancos de dados/fontes de dados listados abaixo você utiliza no trabalho?
**Quantidade de colunas**: 1

| Colunas |
|----------|
| `Quais dos bancos de dados/fontes de dados listados abaixo você utiliza no trabalho?` |

### Grupo MySQL
**Quantidade de colunas**: 1

| Colunas |
|----------|
| `MySQL` |

### Grupo Oracle
**Quantidade de colunas**: 1

| Colunas |
|----------|
| `Oracle` |

### Grupo SQL SERVER
**Quantidade de colunas**: 1

| Colunas |
|----------|
| `SQL SERVER` |

### Grupo Amazon Aurora ou RDS
**Quantidade de colunas**: 1

| Colunas |
|----------|
| `Amazon Aurora ou RDS` |

### Grupo DynamoDB
**Quantidade de colunas**: 1

| Colunas |
|----------|
| `DynamoDB` |

### Grupo CoachDB
**Quantidade de colunas**: 1

| Colunas |
|----------|
| `CoachDB` |

### Grupo Cassandra
**Quantidade de colunas**: 1

| Colunas |
|----------|
| `Cassandra` |

### Grupo MongoDB
**Quantidade de colunas**: 1

| Colunas |
|----------|
| `MongoDB` |

### Grupo MariaDB
**Quantidade de colunas**: 1

| Colunas |
|----------|
| `MariaDB` |

### Grupo Datomic
**Quantidade de colunas**: 1

| Colunas |
|----------|
| `Datomic` |

### Grupo S3
**Quantidade de colunas**: 1

| Colunas |
|----------|
| `S3` |

### Grupo PostgreSQL
**Quantidade de colunas**: 1

| Colunas |
|----------|
| `PostgreSQL` |

### Grupo ElasticSearch
**Quantidade de colunas**: 1

| Colunas |
|----------|
| `ElasticSearch` |

### Grupo DB2
**Quantidade de colunas**: 1

| Colunas |
|----------|
| `DB2` |

### Grupo Microsoft Access
**Quantidade de colunas**: 1

| Colunas |
|----------|
| `Microsoft Access` |

### Grupo SQLite
**Quantidade de colunas**: 1

| Colunas |
|----------|
| `SQLite` |

### Grupo Sybase
**Quantidade de colunas**: 1

| Colunas |
|----------|
| `Sybase` |

### Grupo Firebase
**Quantidade de colunas**: 1

| Colunas |
|----------|
| `Firebase` |

### Grupo Vertica
**Quantidade de colunas**: 1

| Colunas |
|----------|
| `Vertica` |

### Grupo Redis
**Quantidade de colunas**: 1

| Colunas |
|----------|
| `Redis` |

### Grupo Neo4J
**Quantidade de colunas**: 1

| Colunas |
|----------|
| `Neo4J` |

### Grupo Google BigQuery
**Quantidade de colunas**: 1

| Colunas |
|----------|
| `Google BigQuery` |

### Grupo Google Firestore
**Quantidade de colunas**: 1

| Colunas |
|----------|
| `Google Firestore` |

### Grupo Amazon Redshift
**Quantidade de colunas**: 1

| Colunas |
|----------|
| `Amazon Redshift` |

### Grupo Amazon Athena
**Quantidade de colunas**: 1

| Colunas |
|----------|
| `Amazon Athena` |

### Grupo Snowflake
**Quantidade de colunas**: 1

| Colunas |
|----------|
| `Snowflake` |

### Grupo Databricks
**Quantidade de colunas**: 3

| Colunas |
|----------|
| `Databricks` |
| `Databricks` |
| `Databricks` |

### Grupo HBase
**Quantidade de colunas**: 1

| Colunas |
|----------|
| `HBase` |

### Grupo Presto
**Quantidade de colunas**: 1

| Colunas |
|----------|
| `Presto` |

### Grupo Splunk
**Quantidade de colunas**: 1

| Colunas |
|----------|
| `Splunk` |

### Grupo SAP HANA
**Quantidade de colunas**: 1

| Colunas |
|----------|
| `SAP HANA` |

### Grupo Hive
**Quantidade de colunas**: 1

| Colunas |
|----------|
| `Hive` |

### Grupo Firebird
**Quantidade de colunas**: 1

| Colunas |
|----------|
| `Firebird` |

### Grupo Dentre as opções listadas
**Quantidade de colunas**: 1

| Colunas |
|----------|
| `Dentre as opções listadas` |

### Grupo Azure (Microsoft
**Quantidade de colunas**: 1

| Colunas |
|----------|
| `Azure (Microsoft` |

### Grupo Amazon Web Services (AWS
**Quantidade de colunas**: 1

| Colunas |
|----------|
| `Amazon Web Services (AWS` |

### Grupo Google Cloud (GCP
**Quantidade de colunas**: 1

| Colunas |
|----------|
| `Google Cloud (GCP` |

### Grupo Oracle Cloud
**Quantidade de colunas**: 1

| Colunas |
|----------|
| `Oracle Cloud` |

### Grupo IBM
**Quantidade de colunas**: 1

| Colunas |
|----------|
| `IBM` |

### Grupo Servidores On Premise/Não utilizamos Cloud
**Quantidade de colunas**: 1

| Colunas |
|----------|
| `Servidores On Premise/Não utilizamos Cloud` |

### Grupo Cloud Própria
**Quantidade de colunas**: 1

| Colunas |
|----------|
| `Cloud Própria` |

### Grupo Cloud preferida
**Quantidade de colunas**: 1

| Colunas |
|----------|
| `Cloud preferida` |

### Grupo Ferramenta de BI utilizada no dia a dia
**Quantidade de colunas**: 1

| Colunas |
|----------|
| `Ferramenta de BI utilizada no dia a dia` |

### Grupo Microsoft PowerBI
**Quantidade de colunas**: 1

| Colunas |
|----------|
| `Microsoft PowerBI` |

### Grupo Qlik View/Qlik Sense
**Quantidade de colunas**: 1

| Colunas |
|----------|
| `Qlik View/Qlik Sense` |

### Grupo Tableau
**Quantidade de colunas**: 1

| Colunas |
|----------|
| `Tableau` |

### Grupo Metabase
**Quantidade de colunas**: 1

| Colunas |
|----------|
| `Metabase` |

### Grupo Superset
**Quantidade de colunas**: 1

| Colunas |
|----------|
| `Superset` |

### Grupo Redash
**Quantidade de colunas**: 1

| Colunas |
|----------|
| `Redash` |

### Grupo Looker
**Quantidade de colunas**: 1

| Colunas |
|----------|
| `Looker` |

### Grupo Looker Studio(Google Data Studio
**Quantidade de colunas**: 1

| Colunas |
|----------|
| `Looker Studio(Google Data Studio` |

### Grupo Amazon Quicksight
**Quantidade de colunas**: 1

| Colunas |
|----------|
| `Amazon Quicksight` |

### Grupo Mode
**Quantidade de colunas**: 1

| Colunas |
|----------|
| `Mode` |

### Grupo Alteryx
**Quantidade de colunas**: 3

| Colunas |
|----------|
| `Alteryx` |
| `Alteryx` |
| `Alteryx` |

### Grupo MicroStrategy
**Quantidade de colunas**: 1

| Colunas |
|----------|
| `MicroStrategy` |

### Grupo IBM Analytics/Cognos
**Quantidade de colunas**: 1

| Colunas |
|----------|
| `IBM Analytics/Cognos` |

### Grupo SAP Business Objects/SAP Analytics
**Quantidade de colunas**: 1

| Colunas |
|----------|
| `SAP Business Objects/SAP Analytics` |

### Grupo Oracle Business Intelligence
**Quantidade de colunas**: 1

| Colunas |
|----------|
| `Oracle Business Intelligence` |

### Grupo Salesforce/Einstein Analytics
**Quantidade de colunas**: 1

| Colunas |
|----------|
| `Salesforce/Einstein Analytics` |

### Grupo Birst
**Quantidade de colunas**: 1

| Colunas |
|----------|
| `Birst` |

### Grupo SAS Visual Analytics
**Quantidade de colunas**: 1

| Colunas |
|----------|
| `SAS Visual Analytics` |

### Grupo Grafana
**Quantidade de colunas**: 1

| Colunas |
|----------|
| `Grafana` |

### Grupo TIBCO Spotfire
**Quantidade de colunas**: 1

| Colunas |
|----------|
| `TIBCO Spotfire` |

### Grupo Pentaho
**Quantidade de colunas**: 3

| Colunas |
|----------|
| `Pentaho` |
| `Pentaho` |
| `Pentaho` |

### Grupo Fazemos todas as análises utilizando apenas Excel ou planilhas do google
**Quantidade de colunas**: 1

| Colunas |
|----------|
| `Fazemos todas as análises utilizando apenas Excel ou planilhas do google` |

### Grupo Não utilizo nenhuma ferramenta de BI no trabalho
**Quantidade de colunas**: 1

| Colunas |
|----------|
| `Não utilizo nenhuma ferramenta de BI no trabalho` |

### Grupo Qual sua ferramenta de BI preferida?
**Quantidade de colunas**: 1

| Colunas |
|----------|
| `Qual sua ferramenta de BI preferida?` |

### Grupo Qual o tipo de uso de AI Generativa e LLMs na empresa
**Quantidade de colunas**: 1

| Colunas |
|----------|
| `Qual o tipo de uso de AI Generativa e LLMs na empresa` |

### Grupo AI Generativa e LLMs para melhorar produtos externos para os clientes finais
**Quantidade de colunas**: 1

| Colunas |
|----------|
| `AI Generativa e LLMs para melhorar produtos externos para os clientes finais` |

### Grupo Utiliza ChatGPT ou LLMs no trabalho?
**Quantidade de colunas**: 1

| Colunas |
|----------|
| `Utiliza ChatGPT ou LLMs no trabalho?` |

### Grupo Não uso soluções de AI Generativa com foco em produtividade
**Quantidade de colunas**: 1

| Colunas |
|----------|
| `Não uso soluções de AI Generativa com foco em produtividade` |

### Grupo Uso soluções gratuitas de AI Generativa com foco em produtividade
**Quantidade de colunas**: 1

| Colunas |
|----------|
| `Uso soluções gratuitas de AI Generativa com foco em produtividade` |

### Grupo Uso e pago pelas soluções de AI Generativa com foco em produtividade
**Quantidade de colunas**: 1

| Colunas |
|----------|
| `Uso e pago pelas soluções de AI Generativa com foco em produtividade` |

### Grupo A empresa que trabalho paga pelas soluções de AI Generativa com foco em produtividade
**Quantidade de colunas**: 1

| Colunas |
|----------|
| `A empresa que trabalho paga pelas soluções de AI Generativa com foco em produtividade` |

### Grupo Uso soluções do tipo Copilot
**Quantidade de colunas**: 1

| Colunas |
|----------|
| `Uso soluções do tipo Copilot` |

### Grupo Qual seu objetivo na área de dados?
**Quantidade de colunas**: 1

| Colunas |
|----------|
| `Qual seu objetivo na área de dados?` |

### Grupo Qual oportunidade você está buscando?
**Quantidade de colunas**: 1

| Colunas |
|----------|
| `Qual oportunidade você está buscando?` |

### Grupo Há quanto tempo você busca uma oportunidade na área de dados?
**Quantidade de colunas**: 1

| Colunas |
|----------|
| `Há quanto tempo você busca uma oportunidade na área de dados?` |

### Grupo Como tem sido a busca por um emprego na área de dados?
**Quantidade de colunas**: 1

| Colunas |
|----------|
| `Como tem sido a busca por um emprego na área de dados?` |

### Grupo Quais das opções abaixo fazem parte da sua rotina no trabalho atual como engenheiro de dados?
**Quantidade de colunas**: 1

| Colunas |
|----------|
| `Quais das opções abaixo fazem parte da sua rotina no trabalho atual como engenheiro de dados?` |

### Grupo Desenvolvo pipelines de dados utilizando linguagens de programação como Python
**Quantidade de colunas**: 1

| Colunas |
|----------|
| `Desenvolvo pipelines de dados utilizando linguagens de programação como Python` |

### Grupo Realizo construções de ETLs em ferramentas como Pentaho
**Quantidade de colunas**: 1

| Colunas |
|----------|
| `Realizo construções de ETLs em ferramentas como Pentaho` |

### Grupo Crio consultas através da linguagem SQL para exportar informações e compartilhar com as áreas de negócio.
**Quantidade de colunas**: 2

| Colunas |
|----------|
| `Crio consultas através da linguagem SQL para exportar informações e compartilhar com as áreas de negócio.` |
| `Crio consultas através da linguagem SQL para exportar informações e compartilhar com as áreas de negócio.` |

### Grupo Atuo na integração de diferentes fontes de dados através de plataformas proprietárias como Stitch Data
**Quantidade de colunas**: 1

| Colunas |
|----------|
| `Atuo na integração de diferentes fontes de dados através de plataformas proprietárias como Stitch Data` |

### Grupo Modelo soluções de arquitetura de dados
**Quantidade de colunas**: 1

| Colunas |
|----------|
| `Modelo soluções de arquitetura de dados` |

### Grupo Desenvolvo/cuido da manutenção de repositórios de dados baseados em streaming de eventos como Data Lakes e Data Lakehouses.
**Quantidade de colunas**: 1

| Colunas |
|----------|
| `Desenvolvo/cuido da manutenção de repositórios de dados baseados em streaming de eventos como Data Lakes e Data Lakehouses.` |

### Grupo Atuo na modelagem dos dados
**Quantidade de colunas**: 2

| Colunas |
|----------|
| `Atuo na modelagem dos dados` |
| `Atuo na modelagem dos dados` |

### Grupo Cuido da qualidade dos dados
**Quantidade de colunas**: 1

| Colunas |
|----------|
| `Cuido da qualidade dos dados` |

### Grupo Nenhuma das opções listadas refletem meu dia a dia.
**Quantidade de colunas**: 4

| Colunas |
|----------|
| `Nenhuma das opções listadas refletem meu dia a dia.` |
| `Nenhuma das opções listadas refletem meu dia a dia.` |
| `Nenhuma das opções listadas refletem meu dia a dia.` |
| `Nenhuma das opções listadas refletem meu dia a dia.` |

### Grupo Quais as ferramentas/tecnologias de ETL que você utiliza no trabalho como Data Engineer?
**Quantidade de colunas**: 1

| Colunas |
|----------|
| `Quais as ferramentas/tecnologias de ETL que você utiliza no trabalho como Data Engineer?` |

### Grupo Scripts Python
**Quantidade de colunas**: 2

| Colunas |
|----------|
| `Scripts Python` |
| `Scripts Python` |

### Grupo SQL & Stored Procedures
**Quantidade de colunas**: 2

| Colunas |
|----------|
| `SQL & Stored Procedures` |
| `SQL & Stored Procedures` |

### Grupo Apache Airflow
**Quantidade de colunas**: 2

| Colunas |
|----------|
| `Apache Airflow` |
| `Apache Airflow` |

### Grupo Apache NiFi
**Quantidade de colunas**: 2

| Colunas |
|----------|
| `Apache NiFi` |
| `Apache NiFi` |

### Grupo Luigi
**Quantidade de colunas**: 2

| Colunas |
|----------|
| `Luigi` |
| `Luigi` |

### Grupo AWS Glue
**Quantidade de colunas**: 2

| Colunas |
|----------|
| `AWS Glue` |
| `AWS Glue` |

### Grupo Talend
**Quantidade de colunas**: 2

| Colunas |
|----------|
| `Talend` |
| `Talend` |

### Grupo Stitch
**Quantidade de colunas**: 2

| Colunas |
|----------|
| `Stitch` |
| `Stitch` |

### Grupo Fivetran
**Quantidade de colunas**: 2

| Colunas |
|----------|
| `Fivetran` |
| `Fivetran` |

### Grupo Google Dataflow
**Quantidade de colunas**: 2

| Colunas |
|----------|
| `Google Dataflow` |
| `Google Dataflow` |

### Grupo Oracle Data Integrator
**Quantidade de colunas**: 2

| Colunas |
|----------|
| `Oracle Data Integrator` |
| `Oracle Data Integrator` |

### Grupo IBM DataStage
**Quantidade de colunas**: 2

| Colunas |
|----------|
| `IBM DataStage` |
| `IBM DataStage` |

### Grupo SAP BW ETL
**Quantidade de colunas**: 2

| Colunas |
|----------|
| `SAP BW ETL` |
| `SAP BW ETL` |

### Grupo SQL Server Integration Services (SSIS
**Quantidade de colunas**: 2

| Colunas |
|----------|
| `SQL Server Integration Services (SSIS` |
| `SQL Server Integration Services (SSIS` |

### Grupo SAS Data Integration
**Quantidade de colunas**: 2

| Colunas |
|----------|
| `SAS Data Integration` |
| `SAS Data Integration` |

### Grupo Qlik Sense
**Quantidade de colunas**: 2

| Colunas |
|----------|
| `Qlik Sense` |
| `Qlik Sense` |

### Grupo Knime
**Quantidade de colunas**: 2

| Colunas |
|----------|
| `Knime` |
| `Knime` |

### Grupo Não utilizo ferramentas de ETL
**Quantidade de colunas**: 2

| Colunas |
|----------|
| `Não utilizo ferramentas de ETL` |
| `Não utilizo ferramentas de ETL` |

### Grupo Sua organização possui um Data Lake?
**Quantidade de colunas**: 1

| Colunas |
|----------|
| `Sua organização possui um Data Lake?` |

### Grupo Qual tecnologia utilizada como plataforma do Data Lake?
**Quantidade de colunas**: 1

| Colunas |
|----------|
| `Qual tecnologia utilizada como plataforma do Data Lake?` |

### Grupo Sua organização possui um Data Warehouse?
**Quantidade de colunas**: 1

| Colunas |
|----------|
| `Sua organização possui um Data Warehouse?` |

### Grupo Qual tecnologia utilizada como plataforma do Data Warehouse?
**Quantidade de colunas**: 1

| Colunas |
|----------|
| `Qual tecnologia utilizada como plataforma do Data Warehouse?` |

### Grupo Quais as ferramentas de gestão de Qualidade de dados
**Quantidade de colunas**: 1

| Colunas |
|----------|
| `Quais as ferramentas de gestão de Qualidade de dados` |

### Grupo Em qual das opções abaixo você gasta a maior parte do seu tempo?
**Quantidade de colunas**: 1

| Colunas |
|----------|
| `Em qual das opções abaixo você gasta a maior parte do seu tempo?` |

### Grupo Desenvolvendo pipelines de dados utilizando linguagens de programação como Python
**Quantidade de colunas**: 1

| Colunas |
|----------|
| `Desenvolvendo pipelines de dados utilizando linguagens de programação como Python` |

### Grupo Realizando construções de ETLs em ferramentas como Pentaho
**Quantidade de colunas**: 1

| Colunas |
|----------|
| `Realizando construções de ETLs em ferramentas como Pentaho` |

### Grupo Criando consultas através da linguagem SQL para exportar informações e compartilhar com as áreas de negócio.
**Quantidade de colunas**: 2

| Colunas |
|----------|
| `Criando consultas através da linguagem SQL para exportar informações e compartilhar com as áreas de negócio.` |
| `Criando consultas através da linguagem SQL para exportar informações e compartilhar com as áreas de negócio.` |

### Grupo Atuando na integração de diferentes fontes de dados através de plataformas proprietárias como Stitch Data
**Quantidade de colunas**: 1

| Colunas |
|----------|
| `Atuando na integração de diferentes fontes de dados através de plataformas proprietárias como Stitch Data` |

### Grupo Modelando soluções de arquitetura de dados
**Quantidade de colunas**: 1

| Colunas |
|----------|
| `Modelando soluções de arquitetura de dados` |

### Grupo Desenvolvendo/cuidando da manutenção de repositórios de dados baseados em streaming de eventos como Data Lakes e Data Lakehouses.
**Quantidade de colunas**: 1

| Colunas |
|----------|
| `Desenvolvendo/cuidando da manutenção de repositórios de dados baseados em streaming de eventos como Data Lakes e Data Lakehouses.` |

### Grupo Atuando na modelagem dos dados
**Quantidade de colunas**: 2

| Colunas |
|----------|
| `Atuando na modelagem dos dados` |
| `Atuando na modelagem dos dados` |

### Grupo Cuidando da qualidade dos dados
**Quantidade de colunas**: 1

| Colunas |
|----------|
| `Cuidando da qualidade dos dados` |

### Grupo Quais das opções abaixo fazem parte da sua rotina no trabalho atual com análise de dados?
**Quantidade de colunas**: 1

| Colunas |
|----------|
| `Quais das opções abaixo fazem parte da sua rotina no trabalho atual com análise de dados?` |

### Grupo Processo e analiso dados utilizando linguagens de programação como Python
**Quantidade de colunas**: 1

| Colunas |
|----------|
| `Processo e analiso dados utilizando linguagens de programação como Python` |

### Grupo Realizo construções de dashboards em ferramentas de BI como PowerBI
**Quantidade de colunas**: 2

| Colunas |
|----------|
| `Realizo construções de dashboards em ferramentas de BI como PowerBI` |
| `Realizo construções de dashboards em ferramentas de BI como PowerBI` |

### Grupo Utilizo APIs para extrair dados e complementar minhas análises.
**Quantidade de colunas**: 1

| Colunas |
|----------|
| `Utilizo APIs para extrair dados e complementar minhas análises.` |

### Grupo Realizo experimentos e estudos utilizando metodologias estatísticas como teste de hipótese
**Quantidade de colunas**: 1

| Colunas |
|----------|
| `Realizo experimentos e estudos utilizando metodologias estatísticas como teste de hipótese` |

### Grupo Desenvolvo/cuido da manutenção de ETLs utilizando tecnologias como Talend
**Quantidade de colunas**: 1

| Colunas |
|----------|
| `Desenvolvo/cuido da manutenção de ETLs utilizando tecnologias como Talend` |

### Grupo Desenvolvo/cuido da manutenção de planilhas para atender as áreas de negócio.
**Quantidade de colunas**: 1

| Colunas |
|----------|
| `Desenvolvo/cuido da manutenção de planilhas para atender as áreas de negócio.` |

### Grupo Utilizo ferramentas avançadas de estatística como SASS
**Quantidade de colunas**: 1

| Colunas |
|----------|
| `Utilizo ferramentas avançadas de estatística como SASS` |

### Grupo Quais as ferramentas/tecnologias de ETL que você utiliza no trabalho como Data Analyst?
**Quantidade de colunas**: 1

| Colunas |
|----------|
| `Quais as ferramentas/tecnologias de ETL que você utiliza no trabalho como Data Analyst?` |

### Grupo Sua empresa utiliza alguma das ferramentas listadas para dar mais autonomia em análise de dados para as áreas de negócio?
**Quantidade de colunas**: 1

| Colunas |
|----------|
| `Sua empresa utiliza alguma das ferramentas listadas para dar mais autonomia em análise de dados para as áreas de negócio?` |

### Grupo Ferramentas de AutoML como H2O.ai
**Quantidade de colunas**: 1

| Colunas |
|----------|
| `Ferramentas de AutoML como H2O.ai` |

### Grupo ""Point and Click"" Analytics como Alteryx
**Quantidade de colunas**: 1

| Colunas |
|----------|
| `""Point and Click"" Analytics como Alteryx` |

### Grupo Product metricts & Insights como Mixpanel
**Quantidade de colunas**: 1

| Colunas |
|----------|
| `Product metricts & Insights como Mixpanel` |

### Grupo Ferramentas de análise dentro de ferramentas de CRM como Salesforce Einstein Anaytics ou Zendesk dashboards.
**Quantidade de colunas**: 1

| Colunas |
|----------|
| `Ferramentas de análise dentro de ferramentas de CRM como Salesforce Einstein Anaytics ou Zendesk dashboards.` |

### Grupo Minha empresa não utiliza essas ferramentas.
**Quantidade de colunas**: 1

| Colunas |
|----------|
| `Minha empresa não utiliza essas ferramentas.` |

### Grupo Não sei informar.
**Quantidade de colunas**: 1

| Colunas |
|----------|
| `Não sei informar.` |

### Grupo Em qual das opções abaixo você gasta a maior parte do seu tempo de trabalho?
**Quantidade de colunas**: 1

| Colunas |
|----------|
| `Em qual das opções abaixo você gasta a maior parte do seu tempo de trabalho?` |

### Grupo Processando e analisando dados utilizando linguagens de programação como Python
**Quantidade de colunas**: 1

| Colunas |
|----------|
| `Processando e analisando dados utilizando linguagens de programação como Python` |

### Grupo Realizando construções de dashboards em ferramentas de BI como PowerBI
**Quantidade de colunas**: 2

| Colunas |
|----------|
| `Realizando construções de dashboards em ferramentas de BI como PowerBI` |
| `Realizando construções de dashboards em ferramentas de BI como PowerBI` |

### Grupo Utilizando APIs para extrair dados e complementar minhas análises.
**Quantidade de colunas**: 1

| Colunas |
|----------|
| `Utilizando APIs para extrair dados e complementar minhas análises.` |

### Grupo Realizando experimentos e estudos utilizando metodologias estatísticas como teste de hipótese
**Quantidade de colunas**: 1

| Colunas |
|----------|
| `Realizando experimentos e estudos utilizando metodologias estatísticas como teste de hipótese` |

### Grupo Desenvolvendo/cuidando da manutenção de ETLs utilizando tecnologias como Talend
**Quantidade de colunas**: 1

| Colunas |
|----------|
| `Desenvolvendo/cuidando da manutenção de ETLs utilizando tecnologias como Talend` |

### Grupo Desenvolvendo/cuidando da manutenção de planilhas do Excel ou Google Sheets para atender as áreas de negócio.
**Quantidade de colunas**: 1

| Colunas |
|----------|
| `Desenvolvendo/cuidando da manutenção de planilhas do Excel ou Google Sheets para atender as áreas de negócio.` |

### Grupo Utilizando ferramentas avançadas de estatística como SAS
**Quantidade de colunas**: 2

| Colunas |
|----------|
| `Utilizando ferramentas avançadas de estatística como SAS` |
| `Utilizando ferramentas avançadas de estatística como SAS` |

### Grupo Quais das opções abaixo fazem parte da sua rotina no trabalho atual com ciência de dados?
**Quantidade de colunas**: 1

| Colunas |
|----------|
| `Quais das opções abaixo fazem parte da sua rotina no trabalho atual com ciência de dados?` |

### Grupo Estudos Ad-hoc com o objetivo de confirmar hipóteses
**Quantidade de colunas**: 2

| Colunas |
|----------|
| `Estudos Ad-hoc com o objetivo de confirmar hipóteses` |
| `Estudos Ad-hoc com o objetivo de confirmar hipóteses` |

### Grupo Sou responsável pela coleta e limpeza dos dados que uso para análise e modelagem.
**Quantidade de colunas**: 1

| Colunas |
|----------|
| `Sou responsável pela coleta e limpeza dos dados que uso para análise e modelagem.` |

### Grupo Sou responsável por entrar em contato com os times de negócio para definição do problema
**Quantidade de colunas**: 1

| Colunas |
|----------|
| `Sou responsável por entrar em contato com os times de negócio para definição do problema` |

### Grupo Desenvolvo modelos de Machine Learning com o objetivo de colocar em produção em sistemas (produtos de dados).
**Quantidade de colunas**: 1

| Colunas |
|----------|
| `Desenvolvo modelos de Machine Learning com o objetivo de colocar em produção em sistemas (produtos de dados).` |

### Grupo Sou responsável por colocar modelos em produção
**Quantidade de colunas**: 1

| Colunas |
|----------|
| `Sou responsável por colocar modelos em produção` |

### Grupo Cuido da manutenção de modelos de Machine Learning já em produção
**Quantidade de colunas**: 1

| Colunas |
|----------|
| `Cuido da manutenção de modelos de Machine Learning já em produção` |

### Grupo Utilizo ferramentas avançadas de estatística como SAS
**Quantidade de colunas**: 1

| Colunas |
|----------|
| `Utilizo ferramentas avançadas de estatística como SAS` |

### Grupo Crio e dou manutenção em ETLs
**Quantidade de colunas**: 1

| Colunas |
|----------|
| `Crio e dou manutenção em ETLs` |

### Grupo Crio e gerencio soluções de Feature Store e cultura de MLOps.
**Quantidade de colunas**: 1

| Colunas |
|----------|
| `Crio e gerencio soluções de Feature Store e cultura de MLOps.` |

### Grupo Sou responsável por criar e manter a infra que meus modelos e soluções rodam (clusters
**Quantidade de colunas**: 1

| Colunas |
|----------|
| `Sou responsável por criar e manter a infra que meus modelos e soluções rodam (clusters` |

### Grupo Treino e aplico LLMs para solucionar problemas de negócio.
**Quantidade de colunas**: 1

| Colunas |
|----------|
| `Treino e aplico LLMs para solucionar problemas de negócio.` |

### Grupo Quais as técnicas e métodos listados abaixo você costuma utilizar no trabalho?
**Quantidade de colunas**: 1

| Colunas |
|----------|
| `Quais as técnicas e métodos listados abaixo você costuma utilizar no trabalho?` |

### Grupo Utilizo modelos de regressão (linear
**Quantidade de colunas**: 1

| Colunas |
|----------|
| `Utilizo modelos de regressão (linear` |

### Grupo Utilizo redes neurais ou modelos baseados em árvore para criar modelos de classificação
**Quantidade de colunas**: 1

| Colunas |
|----------|
| `Utilizo redes neurais ou modelos baseados em árvore para criar modelos de classificação` |

### Grupo Desenvolvo sistemas de recomendação (RecSys
**Quantidade de colunas**: 1

| Colunas |
|----------|
| `Desenvolvo sistemas de recomendação (RecSys` |

### Grupo Utilizo métodos estatísticos Bayesianos para analisar dados
**Quantidade de colunas**: 1

| Colunas |
|----------|
| `Utilizo métodos estatísticos Bayesianos para analisar dados` |

### Grupo Utilizo técnicas de NLP (Natural Language Processing) para análisar dados não-estruturados
**Quantidade de colunas**: 1

| Colunas |
|----------|
| `Utilizo técnicas de NLP (Natural Language Processing) para análisar dados não-estruturados` |

### Grupo Utilizo métodos estatísticos clássicos (Testes de hipótese
**Quantidade de colunas**: 1

| Colunas |
|----------|
| `Utilizo métodos estatísticos clássicos (Testes de hipótese` |

### Grupo Utilizo cadeias de Markov ou HMMs para realizar análises de dados
**Quantidade de colunas**: 1

| Colunas |
|----------|
| `Utilizo cadeias de Markov ou HMMs para realizar análises de dados` |

### Grupo Desenvolvo técnicas de Clusterização (K-means
**Quantidade de colunas**: 1

| Colunas |
|----------|
| `Desenvolvo técnicas de Clusterização (K-means` |

### Grupo Realizo previsões através de modelos de Séries Temporais (Time Series
**Quantidade de colunas**: 1

| Colunas |
|----------|
| `Realizo previsões através de modelos de Séries Temporais (Time Series` |

### Grupo Utilizo modelos de Reinforcement Learning (aprendizado por reforço
**Quantidade de colunas**: 1

| Colunas |
|----------|
| `Utilizo modelos de Reinforcement Learning (aprendizado por reforço` |

### Grupo Utilizo modelos de Machine Learning para detecção de fraude
**Quantidade de colunas**: 1

| Colunas |
|----------|
| `Utilizo modelos de Machine Learning para detecção de fraude` |

### Grupo Utilizo métodos de Visão Computacional
**Quantidade de colunas**: 1

| Colunas |
|----------|
| `Utilizo métodos de Visão Computacional` |

### Grupo Utilizo modelos de Detecção de Churn
**Quantidade de colunas**: 1

| Colunas |
|----------|
| `Utilizo modelos de Detecção de Churn` |

### Grupo Utilizo LLMs para solucionar problemas de negócio
**Quantidade de colunas**: 1

| Colunas |
|----------|
| `Utilizo LLMs para solucionar problemas de negócio` |

### Grupo Quais dessas tecnologias fazem parte do seu dia a dia como cientista de dados?
**Quantidade de colunas**: 1

| Colunas |
|----------|
| `Quais dessas tecnologias fazem parte do seu dia a dia como cientista de dados?` |

### Grupo Ferramentas de BI (PowerBI
**Quantidade de colunas**: 1

| Colunas |
|----------|
| `Ferramentas de BI (PowerBI` |

### Grupo Planilhas (Excel
**Quantidade de colunas**: 1

| Colunas |
|----------|
| `Planilhas (Excel` |

### Grupo Ambientes de desenvolvimento local (R-studio
**Quantidade de colunas**: 1

| Colunas |
|----------|
| `Ambientes de desenvolvimento local (R-studio` |

### Grupo Ambientes de desenvolvimento na nuvem (Google Colab
**Quantidade de colunas**: 1

| Colunas |
|----------|
| `Ambientes de desenvolvimento na nuvem (Google Colab` |

### Grupo Ferramentas de AutoML (Datarobot
**Quantidade de colunas**: 1

| Colunas |
|----------|
| `Ferramentas de AutoML (Datarobot` |

### Grupo Ferramentas de ETL (Apache Airflow
**Quantidade de colunas**: 1

| Colunas |
|----------|
| `Ferramentas de ETL (Apache Airflow` |

### Grupo Plataformas de Machine Learning (TensorFlow
**Quantidade de colunas**: 1

| Colunas |
|----------|
| `Plataformas de Machine Learning (TensorFlow` |

### Grupo Feature Store (Feast
**Quantidade de colunas**: 1

| Colunas |
|----------|
| `Feature Store (Feast` |

### Grupo Sistemas de controle de versão (Github
**Quantidade de colunas**: 1

| Colunas |
|----------|
| `Sistemas de controle de versão (Github` |

### Grupo Plataformas de Data Apps (Streamlit
**Quantidade de colunas**: 1

| Colunas |
|----------|
| `Plataformas de Data Apps (Streamlit` |

### Grupo Ferramentas de estatística avançada como SPSS
**Quantidade de colunas**: 1

| Colunas |
|----------|
| `Ferramentas de estatística avançada como SPSS` |

### Grupo Em qual das opções abaixo você gasta a maior parte do seu tempo no trabalho?
**Quantidade de colunas**: 1

| Colunas |
|----------|
| `Em qual das opções abaixo você gasta a maior parte do seu tempo no trabalho?` |

### Grupo Coletando e limpando os dados que uso para análise e modelagem.
**Quantidade de colunas**: 1

| Colunas |
|----------|
| `Coletando e limpando os dados que uso para análise e modelagem.` |

### Grupo Entrando em contato com os times de negócio para definição do problema
**Quantidade de colunas**: 1

| Colunas |
|----------|
| `Entrando em contato com os times de negócio para definição do problema` |

### Grupo Desenvolvendo modelos de Machine Learning com o objetivo de colocar em produção em sistemas (produtos de dados).
**Quantidade de colunas**: 1

| Colunas |
|----------|
| `Desenvolvendo modelos de Machine Learning com o objetivo de colocar em produção em sistemas (produtos de dados).` |

### Grupo Colocando modelos em produção
**Quantidade de colunas**: 1

| Colunas |
|----------|
| `Colocando modelos em produção` |

### Grupo Cuidando da manutenção de modelos de Machine Learning já em produção
**Quantidade de colunas**: 1

| Colunas |
|----------|
| `Cuidando da manutenção de modelos de Machine Learning já em produção` |

### Grupo Criando e dando manutenção em ETLs
**Quantidade de colunas**: 1

| Colunas |
|----------|
| `Criando e dando manutenção em ETLs` |

### Grupo Criando e gerenciando soluções de Feature Store e cultura de MLOps.
**Quantidade de colunas**: 1

| Colunas |
|----------|
| `Criando e gerenciando soluções de Feature Store e cultura de MLOps.` |

### Grupo Criando e mantendo a infra que meus modelos e soluções rodam (clusters
**Quantidade de colunas**: 1

| Colunas |
|----------|
| `Criando e mantendo a infra que meus modelos e soluções rodam (clusters` |

### Grupo Treinando e aplicando LLMs para solucionar problemas de negócio.
**Quantidade de colunas**: 1

| Colunas |
|----------|
| `Treinando e aplicando LLMs para solucionar problemas de negócio.` |

