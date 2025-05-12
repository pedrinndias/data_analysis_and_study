# Relatório Completo da Pesquisa de Dados 2023

## Índice

- [Estrutura Hierárquica](#estrutura-hierárquica)
- [Análise por Coluna](#análise-por-coluna)
- [Estatísticas Gerais](#estatísticas-gerais)
- [Dicionário de Dados](#dicionário-de-dados)

## Estrutura Hierárquica

## Seção P0 
**Descrição:** Id
## Seção P1
├─ **a**: Idade
│  └─ **1**: Faixa Idade
├─ **b**: Genero
├─ **c**: Cor/Raca/Etnia
├─ **d**: Pcd
├─ **e**: Experiencia_Profissional_Prejudicada
│  └─ **1**: Não Acredito Que Minha Experiência Profissional Seja Afetada
│  └─ **2**: Experiencia Prejudicada Devido A Minha Cor Raça Etnia
│  └─ **3**: Experiencia Prejudicada Devido A Minha Identidade De Gênero
│  └─ **4**: Experiencia Prejudicada Devido Ao Fato De Ser Pcd
├─ **f**: Aspectos_Prejudicados
│  └─ **1**: Quantidade De Oportunidades De Emprego/Vagas Recebidas
│  └─ **2**: Senioridade Das Vagas Recebidas Em Relação À Sua Experiência
│  └─ **3**: Aprovação Em Processos Seletivos/Entrevistas
│  └─ **4**: Oportunidades De Progressão De Carreira
│  └─ **5**: Velocidade De Progressão De Carreira
│  └─ **6**: Nível De Cobrança No Trabalho/Stress No Trabalho
│  └─ **7**: Atenção Dada Diante Das Minhas Opiniões E Ideias
│  └─ **8**: Relação Com Outros Membros Da Empresa
│  └─ **9**: Relação Com Outros Membros Da Empresa
├─ **g**: Vive_No_Brasil
├─ **i**: Estado Onde Mora
│  └─ **1**: Uf Onde Mora
│  └─ **2**: Regiao Onde Mora
├─ **j**: Mudou De Estado?
├─ **k**: Regiao De Origem
├─ **l**: Nivel De Ensino
├─ **m**: Área De Formação
## Seção P2
├─ **a**: Qual Sua Situação Atual De Trabalho?
├─ **b**: Setor
├─ **c**: Numero De Funcionarios
├─ **d**: Gestor?
├─ **e**: Cargo Como Gestor
├─ **f**: Cargo Atual
├─ **g**: Nivel
├─ **h**: Faixa Salarial
├─ **i**: Quanto Tempo De Experiência Na Área De Dados Você Tem?
├─ **j**: Quanto Tempo De Experiência Na Área De Ti/Engenharia De Software Você Teve Antes De Começar A Trabalhar Na Área De Dados?
├─ **k**: Você Está Satisfeito Na Sua Empresa Atual?
├─ **l**: Qual O Principal Motivo Da Sua Insatisfação Com A Empresa Atual?
│  └─ **1**: Falta De Oportunidade De Crescimento No Emprego Atual
│  └─ **2**: Salário Atual Não Corresponde Ao Mercado
│  └─ **3**: Não Tenho Uma Boa Relação Com Meu Líder/Gestor
│  └─ **4**: Gostaria De Trabalhar Em Em Outra Área De Atuação
│  └─ **5**: Gostaria De Receber Mais Benefícios
│  └─ **6**: O Clima De Trabalho/Ambiente Não É Bom
│  └─ **7**: Falta De Maturidade Analítica Na Empresa
├─ **m**: Você Participou De Entrevistas De Emprego Nos Últimos 6 Meses?
├─ **n**: Você Pretende Mudar De Emprego Nos Próximos 6 Meses?
├─ **o**: Quais Os Principais Critérios Que Você Leva Em Consideração No Momento De Decidir Onde Trabalhar?
│  └─ **1**: Remuneração/Salário
│  └─ **2**: Benefícios
│  └─ **3**: Propósito Do Trabalho E Da Empresa
│  └─ **4**: Flexibilidade De Trabalho Remoto
│  └─ **5**: Ambiente E Clima De Trabalho
│  └─ **6**: Oportunidade De Aprendizado E Trabalhar Com Referências Na Área
│  └─ **7**: Plano De Carreira E Oportunidades De Crescimento Profissional
│  └─ **8**: Maturidade Da Empresa Em Termos De Tecnologia E Dados
│  └─ **9**: Qualidade Dos Gestores E Líderes
│  └─ **10**: Reputação Que A Empresa Tem No Mercado
├─ **q**: Empresa Que Trabaha Passou Por Layoff Em 2023
├─ **r**: Atualmente Qual A Sua Forma De Trabalho?
├─ **s**: Qual A Forma De Trabalho Ideal Para Você?
├─ **t**: Caso Sua Empresa Decida Pelo Modelo 100% Presencial Qual Será Sua Atitude?
## Seção P3
├─ **a**: Qual O Número Aproximado De Pessoas Que Atuam Com Dados Na Sua Empresa Hoje?
├─ **b**: Quais Desses Papéis/Cargos Fazem Parte Do Time Ou Chapter De Dados Da Sua Empresa?
│  └─ **1**: Analytics Engineer
│  └─ **2**: Engenharia De Dados/Data Engineer
│  └─ **3**: Analista De Dados/Data Analyst
│  └─ **4**: Cientista De Dados/Data Scientist
│  └─ **5**: Database Administrator/Dba
│  └─ **6**: Analista De Business Intelligence/Bi
│  └─ **7**: Arquiteto De Dados/Data Architect
│  └─ **8**: Data Product Manager/Dpm
│  └─ **9**: Business Analyst
├─ **c**: Quais Dessas Responsabilidades Fazem Parte Da Sua Rotina Atual De Trabalho Como Gestor?
│  └─ **1**: Pensar Na Visão De Longo Prazo De Dados Da Empresa E Fortalecimento Da Cultura Analítica Da Companhia.
│  └─ **2**: Organização De Treinamentos E Iniciativas Com O Objetivo De Aumentar A Maturidade Analítica Das Áreas De Negócios.
│  └─ **3**: Atração
│  └─ **4**: Decisão Sobre Contratação De Ferramentas E Tecnologias Relacionadas A Dados.
│  └─ **5**: Sou Gestor Da Equipe Responsável Pela Engenharia De Dados E Por Manter O Data Lake Da Empresa Como Fonte Única Dos Dados
│  └─ **6**: Sou Gestor Da Equipe Responsável Pela Entrega De Dados
│  └─ **7**: Sou Gestor Da Equipe Responsável Por Iniciativas E Projetos Envolvendo Inteligência Artificial E Machine Learning.
│  └─ **8**: Apesar De Ser Gestor Ainda Atuo Na Parte Técnica
│  └─ **9**: Gestão De Projetos De Dados
│  └─ **10**: Gestão De Produtos De Dados
│  └─ **11**: Gestão De Pessoas
├─ **d**: Quais São Os 3 Maiores Desafios Que Você Tem Como Gestor No Atual Momento?
│  └─ **1**: A Contratar Novos Talentos.
│  └─ **2**: B Reter Talentos.
│  └─ **3**: C Convencer A Empresa A Aumentar Os Investimentos Na Área De Dados.
│  └─ **4**: D Gestão De Equipes No Ambiente Remoto.
│  └─ **5**: E Gestão De Projetos Envolvendo Áreas Multidisciplinares Da Empresa.
│  └─ **6**: F Organizar As Informações E Garantir A Qualidade E Confiabilidade.
│  └─ **7**: G Conseguir Processar E Armazenar Um Alto Volume De Dados.
│  └─ **8**: H Conseguir Gerar Valor Para As Áreas De Negócios Através De Estudos E Experimentos.
│  └─ **9**: I Desenvolver E Manter Modelos Machine Learning Em Produção.
│  └─ **10**: J Gerenciar A Expectativa Das Áreas De Negócio Em Relação As Entregas Das Equipes De Dados.
│  └─ **11**: K Garantir A Manutenção Dos Projetos E Modelos Em Produção
│  └─ **12**: Conseguir Levar Inovação Para A Empresa Através Dos Dados.
│  └─ **13**: Garantir Retorno Do Investimento Roi Em Projetos De Dados.
│  └─ **14**: Dividir O Tempo Entre Entregas Técnicas E Gestão.
├─ **e**: Ai Generativa É Uma Prioridade Em Sua Empresa?
├─ **f**: Tipos De Uso De Ai Generativa E Llms Na Empresa
│  └─ **1**: Colaboradores Usando Ai Generativa De Forma Independente E Descentralizada
│  └─ **2**: Direcionamento Centralizado Do Uso De Ai Generativa
│  └─ **3**: Desenvolvedores Utilizando Copilots
│  └─ **4**: Ai Generativa E Llms Para Melhorar Produtos Externos
│  └─ **5**: Ai Generativa E Llms Para Melhorar Produtos Internos Para Os Colaboradores
│  └─ **6**: Ia Generativa E Llms Como Principal Frente Do Negócio
│  └─ **7**: Ia Generativa E Llms Não É Prioridade
│  └─ **8**: Não Sei Opinar Sobre O Uso De Ia Generativa E Llms Na Empresa
├─ **g**: Motivos Que Levam A Empresa A Não Usar Ai Genrativa E Llms
│  └─ **1**: Falta De Compreensão Dos Casos De Uso
│  └─ **2**: Falta De Confiabilidade Das Saídas Alucinação Dos Modelos
│  └─ **3**: Incerteza Em Relação A Regulamentação
│  └─ **4**: Preocupações Com Segurança E Privacidade De Dados
│  └─ **5**: Retorno Sobre Investimento Roi Não Comprovado De Ia Generativa
│  └─ **6**: Dados Da Empresa Não Estão Prontos Para Uso De Ia Generativa
│  └─ **7**: Falta De Expertise Ou Falta De Recursos
│  └─ **8**: Alta Direção Da Empresa Não Vê Valor Ou Não Vê Como Prioridade
│  └─ **9**: Preocupações Com Propriedade Intelectual
## Seção P4
├─ **a**: Mesmo Que Esse Não Seja Seu Cargo Formal
│  └─ **1**: Atuacao
├─ **b**: Quais Das Fontes De Dados Listadas Você Já Analisou Ou Processou No Trabalho?
│  └─ **1**: Dados Relacionais Estruturados Em Bancos Sql
│  └─ **2**: Dados Armazenados Em Bancos Nosql
│  └─ **3**: Imagens
│  └─ **4**: Textos/Documentos
│  └─ **5**: Vídeos
│  └─ **6**: Áudios
│  └─ **7**: Planilhas
│  └─ **8**: Dados Georeferenciados
├─ **c**: Entre As Fontes De Dados Listadas
│  └─ **1**: Dados Relacionais Estruturados Em Bancos Sql
│  └─ **2**: Dados Armazenados Em Bancos Nosql
│  └─ **3**: Imagens
│  └─ **4**: Textos/Documentos
│  └─ **5**: Vídeos
│  └─ **6**: Áudios
│  └─ **7**: Planilhas
│  └─ **8**: Dados Georeferenciados
├─ **d**: Quais Das Linguagens Listadas Abaixo Você Utiliza No Trabalho?
│  └─ **1**: Sql
│  └─ **2**: R
│  └─ **3**: Python
│  └─ **4**: C/C++/C#
│  └─ **5**: .Net
│  └─ **6**: Java
│  └─ **7**: Julia
│  └─ **8**: Sas/Stata
│  └─ **9**: Visual Basic/Vba
│  └─ **10**: Scala
│  └─ **11**: Matlab
│  └─ **12**: Rust
│  └─ **13**: Php
│  └─ **14**: Javascript
│  └─ **15**: Não Utilizo Nenhuma Linguagem
├─ **e**: Entre As Linguagens Listadas Abaixo
├─ **f**: Entre As Linguagens Listadas Abaixo
├─ **g**: Quais Dos Bancos De Dados/Fontes De Dados Listados Abaixo Você Utiliza No Trabalho?
│  └─ **1**: Mysql
│  └─ **2**: Oracle
│  └─ **3**: Sql Server
│  └─ **4**: Amazon Aurora Ou Rds
│  └─ **5**: Dynamodb
│  └─ **6**: Coachdb
│  └─ **7**: Cassandra
│  └─ **8**: Mongodb
│  └─ **9**: Mariadb
│  └─ **10**: Datomic
│  └─ **11**: S3
│  └─ **12**: Postgresql
│  └─ **13**: Elasticsearch
│  └─ **14**: Db2
│  └─ **15**: Microsoft Access
│  └─ **16**: Sqlite
│  └─ **17**: Sybase
│  └─ **18**: Firebase
│  └─ **19**: Vertica
│  └─ **20**: Redis
│  └─ **21**: Neo4J
│  └─ **22**: Google Bigquery
│  └─ **23**: Google Firestore
│  └─ **24**: Amazon Redshift
│  └─ **25**: Amazon Athena
│  └─ **26**: Snowflake
│  └─ **27**: Databricks
│  └─ **28**: Hbase
│  └─ **29**: Presto
│  └─ **30**: Splunk
│  └─ **31**: Sap Hana
│  └─ **32**: Hive
│  └─ **33**: Firebird
├─ **h**: Dentre As Opções Listadas
│  └─ **1**: Azure Microsoft
│  └─ **2**: Amazon Web Services Aws
│  └─ **3**: Google Cloud Gcp
│  └─ **4**: Oracle Cloud
│  └─ **5**: Ibm
│  └─ **6**: Servidores On Premise/Não Utilizamos Cloud
│  └─ **7**: Cloud Própria
├─ **i**: Cloud Preferida
├─ **j**: Ferramenta De Bi Utilizada No Dia A Dia
│  └─ **1**: Microsoft Powerbi
│  └─ **2**: Qlik View/Qlik Sense
│  └─ **3**: Tableau
│  └─ **4**: Metabase
│  └─ **5**: Superset
│  └─ **6**: Redash
│  └─ **7**: Looker
│  └─ **8**: Looker Studiogoogle Data Studio
│  └─ **9**: Amazon Quicksight
│  └─ **10**: Mode
│  └─ **11**: Alteryx
│  └─ **12**: Microstrategy
│  └─ **13**: Ibm Analytics/Cognos
│  └─ **14**: Sap Business Objects/Sap Analytics
│  └─ **15**: Oracle Business Intelligence
│  └─ **16**: Salesforce/Einstein Analytics
│  └─ **17**: Birst
│  └─ **18**: Sas Visual Analytics
│  └─ **19**: Grafana
│  └─ **20**: Tibco Spotfire
│  └─ **21**: Pentaho
│  └─ **22**: Fazemos Todas As Análises Utilizando Apenas Excel Ou Planilhas Do Google
│  └─ **23**: Não Utilizo Nenhuma Ferramenta De Bi No Trabalho
├─ **k**: Qual Sua Ferramenta De Bi Preferida?
├─ **l**: Qual O Tipo De Uso De Ai Generativa E Llms Na Empresa
│  └─ **1**: Colaboradores Usando Ai Generativa De Forma Independente E Descentralizada
│  └─ **2**: Direcionamento Centralizado Do Uso De Ai Generativa
│  └─ **3**: Desenvolvedores Utilizando Copilots
│  └─ **4**: Ai Generativa E Llms Para Melhorar Produtos Externos Para Os Clientes Finais
│  └─ **5**: Ai Generativa E Llms Para Melhorar Produtos Internos Para Os Colaboradores
│  └─ **6**: Ia Generativa E Llms Como Principal Frente Do Negócio
│  └─ **7**: Ia Generativa E Llms Não É Prioridade
│  └─ **8**: Não Sei Opinar Sobre O Uso De Ia Generativa E Llms Na Empresa
├─ **m**: Utiliza Chatgpt Ou Llms No Trabalho?
│  └─ **1**: Não Uso Soluções De Ai Generativa Com Foco Em Produtividade
│  └─ **2**: Uso Soluções Gratuitas De Ai Generativa Com Foco Em Produtividade
│  └─ **3**: Uso E Pago Pelas Soluções De Ai Generativa Com Foco Em Produtividade
│  └─ **4**: A Empresa Que Trabalho Paga Pelas Soluções De Ai Generativa Com Foco Em Produtividade
│  └─ **5**: Uso Soluções Do Tipo Copilot
## Seção P5
├─ **a**: Qual Seu Objetivo Na Área De Dados?
├─ **b**: Qual Oportunidade Você Está Buscando?
├─ **c**: Há Quanto Tempo Você Busca Uma Oportunidade Na Área De Dados?
├─ **d**: Como Tem Sido A Busca Por Um Emprego Na Área De Dados?
## Seção P6
├─ **a**: Quais Das Opções Abaixo Fazem Parte Da Sua Rotina No Trabalho Atual Como Engenheiro De Dados?
│  └─ **1**: Desenvolvo Pipelines De Dados Utilizando Linguagens De Programação Como Python
│  └─ **2**: Realizo Construções De Etls Em Ferramentas Como Pentaho
│  └─ **3**: Crio Consultas Através Da Linguagem Sql Para Exportar Informações E Compartilhar Com As Áreas De Negócio.
│  └─ **4**: Atuo Na Integração De Diferentes Fontes De Dados Através De Plataformas Proprietárias Como Stitch Data
│  └─ **5**: Modelo Soluções De Arquitetura De Dados
│  └─ **6**: Desenvolvo/Cuido Da Manutenção De Repositórios De Dados Baseados Em Streaming De Eventos Como Data Lakes E Data Lakehouses.
│  └─ **7**: Atuo Na Modelagem Dos Dados
│  └─ **8**: Cuido Da Qualidade Dos Dados
│  └─ **9**: Nenhuma Das Opções Listadas Refletem Meu Dia A Dia.
├─ **b**: Quais As Ferramentas/Tecnologias De Etl Que Você Utiliza No Trabalho Como Data Engineer?
│  └─ **1**: Scripts Python
│  └─ **2**: Sql & Stored Procedures
│  └─ **3**: Apache Airflow
│  └─ **4**: Apache Nifi
│  └─ **5**: Luigi
│  └─ **6**: Aws Glue
│  └─ **7**: Talend
│  └─ **8**: Pentaho
│  └─ **9**: Alteryx
│  └─ **10**: Stitch
│  └─ **11**: Fivetran
│  └─ **12**: Google Dataflow
│  └─ **13**: Oracle Data Integrator
│  └─ **14**: Ibm Datastage
│  └─ **15**: Sap Bw Etl
│  └─ **16**: Sql Server Integration Services Ssis
│  └─ **17**: Sas Data Integration
│  └─ **18**: Qlik Sense
│  └─ **19**: Knime
│  └─ **20**: Databricks
│  └─ **21**: Não Utilizo Ferramentas De Etl
├─ **c**: Sua Organização Possui Um Data Lake?
├─ **d**: Qual Tecnologia Utilizada Como Plataforma Do Data Lake?
├─ **e**: Sua Organização Possui Um Data Warehouse?
├─ **f**: Qual Tecnologia Utilizada Como Plataforma Do Data Warehouse?
├─ **g**: Quais As Ferramentas De Gestão De Qualidade De Dados
├─ **h**: Em Qual Das Opções Abaixo Você Gasta A Maior Parte Do Seu Tempo?
│  └─ **1**: Desenvolvendo Pipelines De Dados Utilizando Linguagens De Programação Como Python
│  └─ **2**: Realizando Construções De Etls Em Ferramentas Como Pentaho
│  └─ **3**: Criando Consultas Através Da Linguagem Sql Para Exportar Informações E Compartilhar Com As Áreas De Negócio.
│  └─ **4**: Atuando Na Integração De Diferentes Fontes De Dados Através De Plataformas Proprietárias Como Stitch Data
│  └─ **5**: Modelando Soluções De Arquitetura De Dados
│  └─ **6**: Desenvolvendo/Cuidando Da Manutenção De Repositórios De Dados Baseados Em Streaming De Eventos Como Data Lakes E Data Lakehouses.
│  └─ **7**: Atuando Na Modelagem Dos Dados
│  └─ **8**: Cuidando Da Qualidade Dos Dados
│  └─ **9**: Nenhuma Das Opções Listadas Refletem Meu Dia A Dia.
## Seção P7
├─ **1**: Quais Das Opções Abaixo Fazem Parte Da Sua Rotina No Trabalho Atual Com Análise De Dados?
├─ **a**: 
│  └─ **1**: Processo E Analiso Dados Utilizando Linguagens De Programação Como Python
│  └─ **2**: Realizo Construções De Dashboards Em Ferramentas De Bi Como Powerbi
│  └─ **3**: Crio Consultas Através Da Linguagem Sql Para Exportar Informações E Compartilhar Com As Áreas De Negócio.
│  └─ **4**: Utilizo Apis Para Extrair Dados E Complementar Minhas Análises.
│  └─ **5**: Realizo Experimentos E Estudos Utilizando Metodologias Estatísticas Como Teste De Hipótese
│  └─ **6**: Desenvolvo/Cuido Da Manutenção De Etls Utilizando Tecnologias Como Talend
│  └─ **7**: Atuo Na Modelagem Dos Dados
│  └─ **8**: Desenvolvo/Cuido Da Manutenção De Planilhas Para Atender As Áreas De Negócio.
│  └─ **9**: Utilizo Ferramentas Avançadas De Estatística Como Sass
│  └─ **10**: Nenhuma Das Opções Listadas Refletem Meu Dia A Dia.
├─ **b**: Quais As Ferramentas/Tecnologias De Etl Que Você Utiliza No Trabalho Como Data Analyst?
│  └─ **1**: Scripts Python
│  └─ **2**: Sql & Stored Procedures
│  └─ **3**: Apache Airflow
│  └─ **4**: Apache Nifi
│  └─ **5**: Luigi
│  └─ **6**: Aws Glue
│  └─ **7**: Talend
│  └─ **8**: Pentaho
│  └─ **9**: Alteryx
│  └─ **10**: Stitch
│  └─ **11**: Fivetran
│  └─ **12**: Google Dataflow
│  └─ **13**: Oracle Data Integrator
│  └─ **14**: Ibm Datastage
│  └─ **15**: Sap Bw Etl
│  └─ **16**: Sql Server Integration Services Ssis
│  └─ **17**: Sas Data Integration
│  └─ **18**: Qlik Sense
│  └─ **19**: Knime
│  └─ **20**: Databricks
│  └─ **21**: Não Utilizo Ferramentas De Etl
├─ **c**: Sua Empresa Utiliza Alguma Das Ferramentas Listadas Para Dar Mais Autonomia Em Análise De Dados Para As Áreas De Negócio?
│  └─ **1**: Ferramentas De Automl Como H2O.Ai
│  └─ **2**: ""Point And Click"" Analytics Como Alteryx
│  └─ **3**: Product Metricts & Insights Como Mixpanel
│  └─ **4**: Ferramentas De Análise Dentro De Ferramentas De Crm Como Salesforce Einstein Anaytics Ou Zendesk Dashboards.
│  └─ **5**: Minha Empresa Não Utiliza Essas Ferramentas.
│  └─ **6**: Não Sei Informar.
├─ **d**: Em Qual Das Opções Abaixo Você Gasta A Maior Parte Do Seu Tempo De Trabalho?
│  └─ **1**: Processando E Analisando Dados Utilizando Linguagens De Programação Como Python
│  └─ **2**: Realizando Construções De Dashboards Em Ferramentas De Bi Como Powerbi
│  └─ **3**: Criando Consultas Através Da Linguagem Sql Para Exportar Informações E Compartilhar Com As Áreas De Negócio.
│  └─ **4**: Utilizando Apis Para Extrair Dados E Complementar Minhas Análises.
│  └─ **5**: Realizando Experimentos E Estudos Utilizando Metodologias Estatísticas Como Teste De Hipótese
│  └─ **6**: Desenvolvendo/Cuidando Da Manutenção De Etls Utilizando Tecnologias Como Talend
│  └─ **7**: Atuando Na Modelagem Dos Dados
│  └─ **8**: Desenvolvendo/Cuidando Da Manutenção De Planilhas Do Excel Ou Google Sheets Para Atender As Áreas De Negócio.
│  └─ **9**: Utilizando Ferramentas Avançadas De Estatística Como Sas
│  └─ **10**: Nenhuma Das Opções Listadas Refletem Meu Dia A Dia.
## Seção P8
├─ **a**: Quais Das Opções Abaixo Fazem Parte Da Sua Rotina No Trabalho Atual Com Ciência De Dados?
│  └─ **1**: Estudos Ad-Hoc Com O Objetivo De Confirmar Hipóteses
│  └─ **2**: Sou Responsável Pela Coleta E Limpeza Dos Dados Que Uso Para Análise E Modelagem.
│  └─ **3**: Sou Responsável Por Entrar Em Contato Com Os Times De Negócio Para Definição Do Problema
│  └─ **4**: Desenvolvo Modelos De Machine Learning Com O Objetivo De Colocar Em Produção Em Sistemas Produtos De Dados.
│  └─ **5**: Sou Responsável Por Colocar Modelos Em Produção
│  └─ **6**: Cuido Da Manutenção De Modelos De Machine Learning Já Em Produção
│  └─ **7**: Realizo Construções De Dashboards Em Ferramentas De Bi Como Powerbi
│  └─ **8**: Utilizo Ferramentas Avançadas De Estatística Como Sas
│  └─ **9**: Crio E Dou Manutenção Em Etls
│  └─ **10**: Crio E Gerencio Soluções De Feature Store E Cultura De Mlops.
│  └─ **11**: Sou Responsável Por Criar E Manter A Infra Que Meus Modelos E Soluções Rodam Clusters
│  └─ **12**: Treino E Aplico Llms Para Solucionar Problemas De Negócio.
├─ **b**: Quais As Técnicas E Métodos Listados Abaixo Você Costuma Utilizar No Trabalho?
│  └─ **1**: Utilizo Modelos De Regressão Linear
│  └─ **2**: Utilizo Redes Neurais Ou Modelos Baseados Em Árvore Para Criar Modelos De Classificação
│  └─ **3**: Desenvolvo Sistemas De Recomendação Recsys
│  └─ **4**: Utilizo Métodos Estatísticos Bayesianos Para Analisar Dados
│  └─ **5**: Utilizo Técnicas De Nlp Natural Language Processing Para Análisar Dados Não-Estruturados
│  └─ **6**: Utilizo Métodos Estatísticos Clássicos Testes De Hipótese
│  └─ **7**: Utilizo Cadeias De Markov Ou Hmms Para Realizar Análises De Dados
│  └─ **8**: Desenvolvo Técnicas De Clusterização K-Means
│  └─ **9**: Realizo Previsões Através De Modelos De Séries Temporais Time Series
│  └─ **10**: Utilizo Modelos De Reinforcement Learning Aprendizado Por Reforço
│  └─ **11**: Utilizo Modelos De Machine Learning Para Detecção De Fraude
│  └─ **12**: Utilizo Métodos De Visão Computacional
│  └─ **13**: Utilizo Modelos De Detecção De Churn
│  └─ **14**: Utilizo Llms Para Solucionar Problemas De Negócio
├─ **3**: Quais Dessas Tecnologias Fazem Parte Do Seu Dia A Dia Como Cientista De Dados?
├─ **c**: 
│  └─ **1**: Ferramentas De Bi Powerbi
│  └─ **2**: Planilhas Excel
│  └─ **3**: Ambientes De Desenvolvimento Local R-Studio
│  └─ **4**: Ambientes De Desenvolvimento Na Nuvem Google Colab
│  └─ **5**: Ferramentas De Automl Datarobot
│  └─ **6**: Ferramentas De Etl Apache Airflow
│  └─ **7**: Plataformas De Machine Learning Tensorflow
│  └─ **8**: Feature Store Feast
│  └─ **9**: Sistemas De Controle De Versão Github
│  └─ **10**: Plataformas De Data Apps Streamlit
│  └─ **11**: Ferramentas De Estatística Avançada Como Spss
├─ **d**: Em Qual Das Opções Abaixo Você Gasta A Maior Parte Do Seu Tempo No Trabalho?
│  └─ **1**: Estudos Ad-Hoc Com O Objetivo De Confirmar Hipóteses
│  └─ **2**: Coletando E Limpando Os Dados Que Uso Para Análise E Modelagem.
│  └─ **3**: Entrando Em Contato Com Os Times De Negócio Para Definição Do Problema
│  └─ **4**: Desenvolvendo Modelos De Machine Learning Com O Objetivo De Colocar Em Produção Em Sistemas Produtos De Dados.
│  └─ **5**: Colocando Modelos Em Produção
│  └─ **6**: Cuidando Da Manutenção De Modelos De Machine Learning Já Em Produção
│  └─ **7**: Realizando Construções De Dashboards Em Ferramentas De Bi Como Powerbi
│  └─ **8**: Utilizando Ferramentas Avançadas De Estatística Como Sas
│  └─ **9**: Criando E Dando Manutenção Em Etls
│  └─ **10**: Criando E Gerenciando Soluções De Feature Store E Cultura De Mlops.
│  └─ **11**: Criando E Mantendo A Infra Que Meus Modelos E Soluções Rodam Clusters
│  └─ **12**: Treinando E Aplicando Llms Para Solucionar Problemas De Negócio.

## Análise por Coluna

| Código | Descrição | Tipo | Valores Únicos | Faltantes | Exemplos |
|--------|-----------|------|----------------|-----------|----------|
| p0 | Id | object | 5293 | 0.00% | 3lrxr1us2f1q6umt6heu3lrxr1usz7ww, 69pvhqfrpvzjchky569pvgkoeixqomyg, v9celiw9gbv3tv9c9l41memzhuxk880j |
| p1_a | Idade | int64 | 53 | 0.00% | 27, 28, 31 |
| p1_a_1 | Faixa Idade | object | 9 | 0.00% | 35-39, 25-29, 30-34 |
| p1_b | Genero | object | 4 | 0.00% | Masculino, Masculino, Feminino |
| p1_c | Cor/Raca/Etnia | object | 7 | 0.00% | Preta, Branca, Branca |
| p1_d | Pcd | object | 3 | 0.00% | Não, Não, Não |
| p1_e | Experiencia_Profissional_Prejudicada | object | 17 | 48.63% | Sim, acredito que a minha a experiência profissional seja afetada devido a minha Cor/Raça/Etnia, Não acredito que minha experiência profissional seja afetada devido a esses fatores, Não acredito que minha experiência profissional seja afetada devido a esses fatores |
| p1_e_1 | Não Acredito Que Minha Experiência Profissional Seja Afetada | float64 | 2 | 48.63% | 0.0, 0.0, 0.0 |
| p1_e_2 | Experiencia Prejudicada Devido A Minha Cor Raça Etnia | float64 | 2 | 48.63% | 0.0, 0.0, 1.0 |
| p1_e_3 | Experiencia Prejudicada Devido A Minha Identidade De Gênero | float64 | 2 | 48.63% | 0.0, 0.0, 0.0 |
| p1_e_4 | Experiencia Prejudicada Devido Ao Fato De Ser Pcd | float64 | 2 | 48.63% | 0.0, 0.0, 0.0 |
| p1_f | Aspectos_Prejudicados | object | 602 | 76.50% | Quantidade de oportunidades de emprego/vagas recebidas, Atenção dada pelas pessoas diante das minhas opiniões e ideias, Atenção dada pelas pessoas diante das minhas opiniões e ideias, Relação com outros membros da empresa, em momentos de trabalho, Relação com outros membros da empresa, em momentos de integração e outros momentos fora do trabalho, Oportunidades de progressão de carreira, Velocidade de progressão de carreira, Atenção dada pelas pessoas diante das minhas opiniões e ideias, Nível de cobrança no trabalho / Stress no trabalho |
| p1_f_1 | Quantidade De Oportunidades De Emprego/Vagas Recebidas | float64 | 2 | 76.48% | 1.0, 0.0, 1.0 |
| p1_f_2 | Senioridade Das Vagas Recebidas Em Relação À Sua Experiência | float64 | 2 | 76.48% | 0.0, 0.0, 0.0 |
| p1_f_3 | Aprovação Em Processos Seletivos/Entrevistas | float64 | 2 | 76.48% | 0.0, 0.0, 0.0 |
| p1_f_4 | Oportunidades De Progressão De Carreira | float64 | 2 | 76.48% | 1.0, 0.0, 0.0 |
| p1_f_5 | Velocidade De Progressão De Carreira | float64 | 2 | 76.48% | 0.0, 1.0, 1.0 |
| p1_f_6 | Nível De Cobrança No Trabalho/Stress No Trabalho | float64 | 2 | 76.48% | 1.0, 0.0, 1.0 |
| p1_f_7 | Atenção Dada Diante Das Minhas Opiniões E Ideias | float64 | 2 | 76.48% | 0.0, 0.0, 1.0 |
| p1_f_8 | Relação Com Outros Membros Da Empresa | float64 | 2 | 76.48% | 0.0, 0.0, 1.0 |
| p1_f_9 | Relação Com Outros Membros Da Empresa | float64 | 2 | 76.48% | 0.0, 0.0, 0.0 |
| p1_g | Vive_No_Brasil | int64 | 2 | 0.00% | 1, 1, 1 |
| p1_i | Estado Onde Mora | object | 26 | 2.29% | Distrito Federal (DF), São Paulo (SP), Piauí (PI) |
| p1_i_1 | Uf Onde Mora | object | 25 | 2.34% | BA, SP, ES |
| p1_i_2 | Regiao Onde Mora | object | 5 | 2.34% | Sudeste, Sul, Sul |
| p1_j | Mudou De Estado? | float64 | 2 | 2.29% | 1.0, 0.0, 1.0 |
| p1_k | Regiao De Origem | object | 28 | 79.90% | Nasci/me formei fora do Brasil, Bahia (BA), Minas Gerais (MG) |
| p1_l | Nivel De Ensino | object | 7 | 0.00% | Pós-graduação, Estudante de Graduação, Pós-graduação |
| p1_m | Área De Formação | object | 9 | 2.13% | Marketing / Publicidade / Comunicação / Jornalismo, Outras Engenharias, Outras Engenharias |
| p2_a | Qual Sua Situação Atual De Trabalho? | object | 13 | 0.00% | Empregado (CLT), Empregado (CLT), Empregado (CLT) |
| p2_b | Setor | object | 21 | 10.20% | Tecnologia/Fábrica de Software, Área da Saúde, Área de Consultoria |
| p2_c | Numero De Funcionarios | object | 9 | 10.20% | Acima de 3.000, de 1.001 a 3.000, de 11 a 50 |
| p2_d | Gestor? | float64 | 2 | 10.20% | 0.0, 0.0, 0.0 |
| p2_e | Cargo Como Gestor | object | 5 | 83.07% | Team Leader/Tech Leader, Gerente/Head, Supervisor/Coordenador |
| p2_f | Cargo Atual | object | 17 | 27.13% | Engenheiro de Dados/Arquiteto de Dados/Data Engineer/Data Architect, Engenheiro de Machine Learning/ML Engineer/AI Engineer, Cientista de Dados/Data Scientist |
| p2_g | Nivel | object | 3 | 27.13% | Pleno, Júnior, Pleno |
| p2_h | Faixa Salarial | object | 14 | 10.20% | Menos de R$ 1.000/mês, de R$ 8.001/mês a R$ 12.000/mês, de R$ 3.001/mês a R$ 4.000/mês |
| p2_i | Quanto Tempo De Experiência Na Área De Dados Você Tem? | object | 8 | 10.20% | de 7 a 10 anos, de 3 a 4 anos, de 1 a 2 anos |
| p2_j | Quanto Tempo De Experiência Na Área De Ti/Engenharia De Software Você Teve Antes De Começar A Trabalhar Na Área De Dados? | object | 7 | 10.20% | de 3 a 4 anos, de 5 a 6 anos, Não tive experiência na área de TI/Engenharia de Software antes de começar a trabalhar na área de dados |
| p2_k | Você Está Satisfeito Na Sua Empresa Atual? | float64 | 2 | 10.20% | 1.0, 1.0, 1.0 |
| p2_l | Qual O Principal Motivo Da Sua Insatisfação Com A Empresa Atual? | object | 259 | 75.10% | Salário atual não corresponde ao mercado, Falta de oportunidade de crescimento no emprego atual, Gostaria de trabalhar em em outra área de atuação, Falta de oportunidade de crescimento no emprego atual, O clima de trabalho/ambiente não é bom, Falta de maturidade analítica na empresa, Falta de maturidade analítica na empresa, Falta de oportunidade de crescimento no emprego atual, Salário atual não corresponde ao mercado |
| p2_l_1 | Falta De Oportunidade De Crescimento No Emprego Atual | float64 | 2 | 75.10% | 1.0, 1.0, 0.0 |
| p2_l_2 | Salário Atual Não Corresponde Ao Mercado | float64 | 2 | 75.10% | 1.0, 0.0, 1.0 |
| p2_l_3 | Não Tenho Uma Boa Relação Com Meu Líder/Gestor | float64 | 2 | 75.10% | 0.0, 0.0, 0.0 |
| p2_l_4 | Gostaria De Trabalhar Em Em Outra Área De Atuação | float64 | 2 | 75.10% | 0.0, 0.0, 1.0 |
| p2_l_5 | Gostaria De Receber Mais Benefícios | float64 | 2 | 75.10% | 0.0, 1.0, 1.0 |
| p2_l_6 | O Clima De Trabalho/Ambiente Não É Bom | float64 | 2 | 75.10% | 1.0, 0.0, 0.0 |
| p2_l_7 | Falta De Maturidade Analítica Na Empresa | float64 | 2 | 75.10% | 1.0, 0.0, 0.0 |
| p2_m | Você Participou De Entrevistas De Emprego Nos Últimos 6 Meses? | object | 6 | 10.20% | Não participei de entrevistas de emprego/processos seletivos nos últimos 6 meses, Sim, fiz entrevistas mas não fui aprovado (ou ainda aguardo resposta), Sim, fui aprovado no meu primeiro emprego (ou estava sem emprego) |
| p2_n | Você Pretende Mudar De Emprego Nos Próximos 6 Meses? | object | 4 | 10.20% | Não estou buscando e não pretendo mudar de emprego nos próximos 6 meses, Não estou buscando, mas me considero aberto a outras oportunidades, Estou em busca de oportunidades dentro ou fora do Brasil |
| p2_o | Quais Os Principais Critérios Que Você Leva Em Consideração No Momento De Decidir Onde Trabalhar? | object | 466 | 10.69% | Remuneração/Salário, Flexibilidade de trabalho remoto, Plano de carreira e oportunidades de crescimento profissional, Flexibilidade de trabalho remoto, Plano de carreira e oportunidades de crescimento profissional, Remuneração/Salário, Flexibilidade de trabalho remoto, Ambiente e clima de trabalho |
| p2_o_1 | Remuneração/Salário | float64 | 2 | 10.69% | 1.0, 1.0, 1.0 |
| p2_o_2 | Benefícios | float64 | 2 | 10.69% | 0.0, 1.0, 0.0 |
| p2_o_3 | Propósito Do Trabalho E Da Empresa | float64 | 2 | 10.69% | 0.0, 0.0, 1.0 |
| p2_o_4 | Flexibilidade De Trabalho Remoto | float64 | 2 | 10.69% | 1.0, 1.0, 0.0 |
| p2_o_5 | Ambiente E Clima De Trabalho | float64 | 2 | 10.69% | 0.0, 1.0, 0.0 |
| p2_o_6 | Oportunidade De Aprendizado E Trabalhar Com Referências Na Área | float64 | 2 | 10.69% | 0.0, 1.0, 1.0 |
| p2_o_7 | Plano De Carreira E Oportunidades De Crescimento Profissional | float64 | 2 | 10.69% | 0.0, 0.0, 0.0 |
| p2_o_8 | Maturidade Da Empresa Em Termos De Tecnologia E Dados | float64 | 2 | 10.69% | 0.0, 1.0, 0.0 |
| p2_o_9 | Qualidade Dos Gestores E Líderes | float64 | 2 | 10.69% | 0.0, 0.0, 1.0 |
| p2_o_10 | Reputação Que A Empresa Tem No Mercado | float64 | 2 | 10.69% | 0.0, 0.0, 0.0 |
| p2_q | Empresa Que Trabaha Passou Por Layoff Em 2023 | object | 3 | 10.20% | Não ocorreram layoffs/demissões em massa na empresa em que trabalho, Não ocorreram layoffs/demissões em massa na empresa em que trabalho, Sim, ocorreram layoffs/demissões em massa na empresa em que trabalho mas não fui afetado |
| p2_r | Atualmente Qual A Sua Forma De Trabalho? | object | 4 | 10.20% | Modelo híbrido flexível (o funcionário tem liberdade para escolher quando estar no escritório presencialmente), Modelo 100% remoto, Modelo 100% presencial |
| p2_s | Qual A Forma De Trabalho Ideal Para Você? | object | 4 | 10.20% | Modelo híbrido flexível (o funcionário tem liberdade para escolher quando estar no escritório presencialmente), Modelo híbrido com dias fixos de trabalho presencial, Modelo híbrido com dias fixos de trabalho presencial |
| p2_t | Caso Sua Empresa Decida Pelo Modelo 100% Presencial Qual Será Sua Atitude? | object | 3 | 10.20% | Vou procurar outra oportunidade no modelo híbrido ou remoto, Vou procurar outra oportunidade no modelo 100% remoto, Vou procurar outra oportunidade no modelo híbrido ou remoto |
| p3_a | Qual O Número Aproximado De Pessoas Que Atuam Com Dados Na Sua Empresa Hoje? | object | 8 | 83.07% | 4 - 10, Acima de 300 pessoas, Acima de 300 pessoas |
| p3_b | Quais Desses Papéis/Cargos Fazem Parte Do Time Ou Chapter De Dados Da Sua Empresa? | object | 647 | 83.77% | Business Analyst, Analista de Dados/Data Analyst, Analista de Dados/Data Analyst, Analytics Engineer, Engenharia de Dados/Data Engineer, Cientista de Dados/Data Scientist, Data Product Manager/DPM, Engenharia de Dados/Data Engineer, Cientista de Dados/Data Scientist, Analista de Business Intelligence/BI, Machine Learning Engineer/AI Engineer, Business Analyst |
| p3_b_1 | Analytics Engineer | float64 | 2 | 83.77% | 0.0, 0.0, 0.0 |
| p3_b_2 | Engenharia De Dados/Data Engineer | float64 | 2 | 83.77% | 0.0, 0.0, 0.0 |
| p3_b_3 | Analista De Dados/Data Analyst | float64 | 2 | 83.77% | 1.0, 1.0, 0.0 |
| p3_b_4 | Cientista De Dados/Data Scientist | float64 | 2 | 83.77% | 0.0, 0.0, 1.0 |
| p3_b_5 | Database Administrator/Dba | float64 | 2 | 83.77% | 1.0, 1.0, 0.0 |
| p3_b_6 | Analista De Business Intelligence/Bi | float64 | 2 | 83.77% | 1.0, 1.0, 0.0 |
| p3_b_7 | Arquiteto De Dados/Data Architect | float64 | 2 | 83.77% | 1.0, 0.0, 0.0 |
| p3_b_8 | Data Product Manager/Dpm | float64 | 2 | 83.77% | 0.0, 0.0, 1.0 |
| p3_b_9 | Business Analyst | float64 | 2 | 83.77% | 1.0, 1.0, 0.0 |
| p3_c | Quais Dessas Responsabilidades Fazem Parte Da Sua Rotina Atual De Trabalho Como Gestor? | object | 611 | 83.51% | Gestão de pessoas, apoio no desenvolvimento das pessoas, evolução de carreira,, Atração, seleção e contratação de talentos para o time de dados., Sou gestor da equipe responsável pela entrega de dados, estudos, relatórios e dashboards para as áreas de negócio da empresa., Apesar de ser gestor ainda atuo na parte técnica, construindo soluções/análises/modelos etc., Pensar na visão de longo prazo de dados da empresa e fortalecimento da cultura analítica da companhia., Atração, seleção e contratação de talentos para o time de dados., Decisão sobre contratação de ferramentas e tecnologias relacionadas a dados., Sou gestor da equipe responsável pela entrega de dados, estudos, relatórios e dashboards para as áreas de negócio da empresa., Sou gestor da equipe responsável por iniciativas e projetos envolvendo Inteligência Artificial e Machine Learning., Gestão de produtos de dados, cuidando da visão dos produtos, backlog, feedback de usuários etc., Gestão de projetos de dados, cuidando das etapas, equipes envolvidas, atingimento dos objetivos etc., Gestão de pessoas, apoio no desenvolvimento das pessoas, evolução de carreira, |
| p3_c_1 | Pensar Na Visão De Longo Prazo De Dados Da Empresa E Fortalecimento Da Cultura Analítica Da Companhia. | float64 | 2 | 83.49% | 1.0, 1.0, 1.0 |
| p3_c_2 | Organização De Treinamentos E Iniciativas Com O Objetivo De Aumentar A Maturidade Analítica Das Áreas De Negócios. | float64 | 2 | 83.49% | 0.0, 1.0, 0.0 |
| p3_c_3 | Atração | float64 | 2 | 83.49% | 1.0, 1.0, 0.0 |
| p3_c_4 | Decisão Sobre Contratação De Ferramentas E Tecnologias Relacionadas A Dados. | float64 | 2 | 83.49% | 1.0, 0.0, 0.0 |
| p3_c_5 | Sou Gestor Da Equipe Responsável Pela Engenharia De Dados E Por Manter O Data Lake Da Empresa Como Fonte Única Dos Dados | float64 | 2 | 83.49% | 0.0, 0.0, 1.0 |
| p3_c_6 | Sou Gestor Da Equipe Responsável Pela Entrega De Dados | float64 | 2 | 83.49% | 0.0, 0.0, 0.0 |
| p3_c_7 | Sou Gestor Da Equipe Responsável Por Iniciativas E Projetos Envolvendo Inteligência Artificial E Machine Learning. | float64 | 2 | 83.49% | 0.0, 0.0, 0.0 |
| p3_c_8 | Apesar De Ser Gestor Ainda Atuo Na Parte Técnica | float64 | 2 | 83.49% | 0.0, 1.0, 1.0 |
| p3_c_9 | Gestão De Projetos De Dados | float64 | 2 | 83.49% | 0.0, 1.0, 1.0 |
| p3_c_10 | Gestão De Produtos De Dados | float64 | 2 | 83.49% | 1.0, 0.0, 0.0 |
| p3_c_11 | Gestão De Pessoas | float64 | 2 | 83.49% | 0.0, 0.0, 0.0 |
| p3_d | Quais São Os 3 Maiores Desafios Que Você Tem Como Gestor No Atual Momento? | object | 601 | 83.53% | Garantir retorno do investimento (ROI) em projetos de dados., Conseguir gerar valor para as áreas de negócios através de estudos e experimentos., Gerenciar a expectativa das áreas de negócio em relação as entregas das equipes de dados., Conseguir gerar valor para as áreas de negócios através de estudos e experimentos., Organizar as informações e garantir a qualidade e confiabilidade., Dividir o tempo entre entregas técnicas e gestão de pessoas., Gerenciar a expectativa das áreas de negócio em relação as entregas das equipes de dados., Garantir a manutenção dos projetos e modelos em produção, em meio ao crescimento da empresa. |
| p3_d_1 | A Contratar Novos Talentos. | float64 | 2 | 83.49% | 1.0, 0.0, 1.0 |
| p3_d_2 | B Reter Talentos. | float64 | 2 | 83.49% | 0.0, 0.0, 0.0 |
| p3_d_3 | C Convencer A Empresa A Aumentar Os Investimentos Na Área De Dados. | float64 | 2 | 83.49% | 0.0, 0.0, 0.0 |
| p3_d_4 | D Gestão De Equipes No Ambiente Remoto. | float64 | 2 | 83.49% | 0.0, 0.0, 0.0 |
| p3_d_5 | E Gestão De Projetos Envolvendo Áreas Multidisciplinares Da Empresa. | float64 | 2 | 83.49% | 0.0, 0.0, 0.0 |
| p3_d_6 | F Organizar As Informações E Garantir A Qualidade E Confiabilidade. | float64 | 2 | 83.49% | 1.0, 1.0, 0.0 |
| p3_d_7 | G Conseguir Processar E Armazenar Um Alto Volume De Dados. | float64 | 2 | 83.49% | 0.0, 0.0, 0.0 |
| p3_d_8 | H Conseguir Gerar Valor Para As Áreas De Negócios Através De Estudos E Experimentos. | float64 | 2 | 83.49% | 1.0, 1.0, 0.0 |
| p3_d_9 | I Desenvolver E Manter Modelos Machine Learning Em Produção. | float64 | 2 | 83.49% | 0.0, 0.0, 0.0 |
| p3_d_10 | J Gerenciar A Expectativa Das Áreas De Negócio Em Relação As Entregas Das Equipes De Dados. | float64 | 2 | 83.49% | 1.0, 1.0, 1.0 |
| p3_d_11 | K Garantir A Manutenção Dos Projetos E Modelos Em Produção | float64 | 2 | 83.49% | 0.0, 0.0, 0.0 |
| p3_d_12 | Conseguir Levar Inovação Para A Empresa Através Dos Dados. | float64 | 2 | 83.49% | 0.0, 0.0, 0.0 |
| p3_d_13 | Garantir Retorno Do Investimento Roi Em Projetos De Dados. | float64 | 2 | 83.49% | 0.0, 0.0, 0.0 |
| p3_d_14 | Dividir O Tempo Entre Entregas Técnicas E Gestão. | float64 | 2 | 83.49% | 0.0, 0.0, 0.0 |
| p3_e | Ai Generativa É Uma Prioridade Em Sua Empresa? | object | 5 | 83.07% | Não é uma iniciativa que estamos focando e não tem sido uma prioridade., Mais ou menos... É uma das várias iniciativas que estamos impulsionando, mas não é uma prioridade (iniciativas isoladas e pouco foco)., Mais ou menos... É uma das várias iniciativas que estamos impulsionando, mas não é uma prioridade (iniciativas isoladas e pouco foco). |
| p3_f | Tipos De Uso De Ai Generativa E Llms Na Empresa | object | 152 | 83.71% | Não tenho visto soluções de IA Generatica e LLMs sendo tradadas como prioridade pela empresa e pessoas, os poucos casos de uso são isolados ou ainda estão muito no início., Uma ou mais equipes testando e aplicando soluções de AI Generativa e LLMs, com o objetivo de aumentar a eficiencia de processos internos (como produtividade das equipes internas, ou melhoria de processos existentes)., Uma ou mais equipes testando e aplicando soluções de AI Generativa e LLMs, com o objetivo de propor melhorias e inovações para impulsionar a diferenciação de produtos oferecidos para os clientes finais (exemplo: novos recursos, produtos, serviços etc)., Colaboradores utilizando soluções baseadas em AI Generativa (como o ChatGPT por exemplo) de forma independente, com o objetivo de melhorar sua produtividade no dia a dia, sem um direcionamento centralizado., Existe um direcionamento centralizado para que colaboradores utilizem soluções baseadas em AI Generativa (como o ChatGPT por exemplo), incluindo apoio nos custos das ferramentas., Colaboradores utilizando soluções baseadas em AI Generativa (como o ChatGPT por exemplo) de forma independente, com o objetivo de melhorar sua produtividade no dia a dia, sem um direcionamento centralizado. |
| p3_f_1 | Colaboradores Usando Ai Generativa De Forma Independente E Descentralizada | float64 | 2 | 83.71% | 1.0, 0.0, 0.0 |
| p3_f_2 | Direcionamento Centralizado Do Uso De Ai Generativa | float64 | 2 | 83.71% | 0.0, 0.0, 0.0 |
| p3_f_3 | Desenvolvedores Utilizando Copilots | float64 | 2 | 83.71% | 0.0, 0.0, 0.0 |
| p3_f_4 | Ai Generativa E Llms Para Melhorar Produtos Externos | float64 | 2 | 83.71% | 0.0, 1.0, 1.0 |
| p3_f_5 | Ai Generativa E Llms Para Melhorar Produtos Internos Para Os Colaboradores | float64 | 2 | 83.71% | 1.0, 1.0, 0.0 |
| p3_f_6 | Ia Generativa E Llms Como Principal Frente Do Negócio | float64 | 2 | 83.71% | 0.0, 0.0, 0.0 |
| p3_f_7 | Ia Generativa E Llms Não É Prioridade | float64 | 2 | 83.71% | 1.0, 0.0, 0.0 |
| p3_f_8 | Não Sei Opinar Sobre O Uso De Ia Generativa E Llms Na Empresa | float64 | 2 | 83.71% | 0.0, 0.0, 0.0 |
| p3_g | Motivos Que Levam A Empresa A Não Usar Ai Genrativa E Llms | object | 269 | 84.47% | Dados da empresa não estão prontos para uso de IA Generativa., Falta de compreensão dos casos de uso., Falta de compreensão dos casos de uso., Dados da empresa não estão prontos para uso de IA Generativa., Falta de expertise das equipes técnicas ou falta de recursos internos. |
| p3_g_1 | Falta De Compreensão Dos Casos De Uso | float64 | 2 | 84.45% | 0.0, 0.0, 0.0 |
| p3_g_2 | Falta De Confiabilidade Das Saídas Alucinação Dos Modelos | float64 | 2 | 84.45% | 1.0, 0.0, 0.0 |
| p3_g_3 | Incerteza Em Relação A Regulamentação | float64 | 2 | 84.45% | 0.0, 1.0, 0.0 |
| p3_g_4 | Preocupações Com Segurança E Privacidade De Dados | float64 | 2 | 84.45% | 1.0, 1.0, 0.0 |
| p3_g_5 | Retorno Sobre Investimento Roi Não Comprovado De Ia Generativa | float64 | 2 | 84.45% | 0.0, 0.0, 0.0 |
| p3_g_6 | Dados Da Empresa Não Estão Prontos Para Uso De Ia Generativa | float64 | 2 | 84.45% | 0.0, 0.0, 0.0 |
| p3_g_7 | Falta De Expertise Ou Falta De Recursos | float64 | 2 | 84.45% | 0.0, 0.0, 0.0 |
| p3_g_8 | Alta Direção Da Empresa Não Vê Valor Ou Não Vê Como Prioridade | float64 | 2 | 84.45% | 0.0, 0.0, 0.0 |
| p3_g_9 | Preocupações Com Propriedade Intelectual | float64 | 2 | 84.45% | 0.0, 0.0, 0.0 |
| p4_a | Mesmo Que Esse Não Seja Seu Cargo Formal | object | 4 | 29.13% | Não atuo em nenhuma das frentes citadas., *Ciência de Dados/Machine Learning/AI: *Desenha e executa experimentos com o objetivo de responder perguntas do negócio; desenvolve modelos preditivos e algoritmos de Machine Learning com o objetivo de otimizar e automatizar a tomada de decisão., *Análise de Dados/BI:* Extrai e cruza dados unindo diferentes fontes da informação; analisa dados visando identificar padrões, gerar insights e levantar perguntas; desenvolve dashboards, relatórios e visualizações de dados em ferramentas de BI. |
| p4_a_1 | Atuacao | object | 6 | 0.00% | Engenharia de Dados, Análise de Dados, Gestor |
| p4_b | Quais Das Fontes De Dados Listadas Você Já Analisou Ou Processou No Trabalho? | object | 544 | 28.74% | Dados relacionais (estruturados em bancos SQL), Planilhas, Planilhas, Dados relacionais (estruturados em bancos SQL), Planilhas |
| p4_b_1 | Dados Relacionais Estruturados Em Bancos Sql | float64 | 2 | 28.74% | 1.0, 1.0, 1.0 |
| p4_b_2 | Dados Armazenados Em Bancos Nosql | float64 | 2 | 28.74% | 1.0, 0.0, 0.0 |
| p4_b_3 | Imagens | float64 | 2 | 28.74% | 0.0, 0.0, 0.0 |
| p4_b_4 | Textos/Documentos | float64 | 2 | 28.74% | 1.0, 1.0, 0.0 |
| p4_b_5 | Vídeos | float64 | 2 | 28.74% | 0.0, 0.0, 0.0 |
| p4_b_6 | Áudios | float64 | 2 | 28.74% | 0.0, 0.0, 0.0 |
| p4_b_7 | Planilhas | float64 | 2 | 28.74% | 1.0, 1.0, 1.0 |
| p4_b_8 | Dados Georeferenciados | float64 | 2 | 28.74% | 0.0, 0.0, 1.0 |
| p4_c | Entre As Fontes De Dados Listadas | object | 104 | 28.75% | Dados relacionais (estruturados em bancos SQL), Dados armazenados em bancos NoSQL, Ingestão direta de eventos, Dados relacionais (estruturados em bancos SQL), Planilhas |
| p4_c_1 | Dados Relacionais Estruturados Em Bancos Sql | float64 | 2 | 28.74% | 1.0, 1.0, 1.0 |
| p4_c_2 | Dados Armazenados Em Bancos Nosql | float64 | 2 | 28.74% | 0.0, 0.0, 0.0 |
| p4_c_3 | Imagens | float64 | 2 | 28.74% | 0.0, 0.0, 0.0 |
| p4_c_4 | Textos/Documentos | float64 | 2 | 28.74% | 0.0, 1.0, 0.0 |
| p4_c_5 | Vídeos | float64 | 2 | 28.74% | 0.0, 0.0, 0.0 |
| p4_c_6 | Áudios | float64 | 2 | 28.74% | 0.0, 0.0, 0.0 |
| p4_c_7 | Planilhas | float64 | 2 | 28.74% | 1.0, 0.0, 0.0 |
| p4_c_8 | Dados Georeferenciados | float64 | 2 | 28.74% | 0.0, 0.0, 0.0 |
| p4_d | Quais Das Linguagens Listadas Abaixo Você Utiliza No Trabalho? | object | 271 | 28.74% | SQL, Python, SQL, Python, SQL |
| p4_d_1 | Sql | float64 | 2 | 28.74% | 1.0, 1.0, 0.0 |
| p4_d_2 | R | float64 | 2 | 28.74% | 0.0, 0.0, 0.0 |
| p4_d_3 | Python | float64 | 2 | 28.74% | 1.0, 1.0, 1.0 |
| p4_d_4 | C/C++/C# | float64 | 2 | 28.74% | 0.0, 0.0, 0.0 |
| p4_d_5 | .Net | float64 | 2 | 28.74% | 0.0, 0.0, 0.0 |
| p4_d_6 | Java | float64 | 2 | 28.74% | 0.0, 0.0, 0.0 |
| p4_d_7 | Julia | float64 | 2 | 28.74% | 0.0, 0.0, 0.0 |
| p4_d_8 | Sas/Stata | float64 | 2 | 28.74% | 0.0, 0.0, 0.0 |
| p4_d_9 | Visual Basic/Vba | float64 | 2 | 28.74% | 0.0, 0.0, 0.0 |
| p4_d_10 | Scala | float64 | 2 | 28.74% | 0.0, 0.0, 0.0 |
| p4_d_11 | Matlab | float64 | 2 | 28.74% | 0.0, 0.0, 0.0 |
| p4_d_12 | Rust | float64 | 2 | 28.74% | 0.0, 0.0, 0.0 |
| p4_d_13 | Php | float64 | 2 | 28.74% | 0.0, 0.0, 0.0 |
| p4_d_14 | Javascript | float64 | 2 | 28.74% | 0.0, 0.0, 0.0 |
| p4_d_15 | Não Utilizo Nenhuma Linguagem | float64 | 2 | 28.74% | 0.0, 1.0, 0.0 |
| p4_e | Entre As Linguagens Listadas Abaixo | object | 14 | 28.74% | Python, R, SQL |
| p4_f | Entre As Linguagens Listadas Abaixo | object | 16 | 29.15% | Python, Python, Rust |
| p4_g | Quais Dos Bancos De Dados/Fontes De Dados Listados Abaixo Você Utiliza No Trabalho? | object | 1838 | 28.77% | S3, MySQL, SQL SERVER, Google BigQuery, Amazon Athena, Amazon Redshift, S3, Neo4J, Amazon Aurora ou RDS |
| p4_g_1 | Mysql | float64 | 2 | 28.74% | 0.0, 1.0, 1.0 |
| p4_g_2 | Oracle | float64 | 2 | 28.74% | 0.0, 1.0, 0.0 |
| p4_g_3 | Sql Server | float64 | 2 | 28.74% | 0.0, 1.0, 0.0 |
| p4_g_4 | Amazon Aurora Ou Rds | float64 | 2 | 28.74% | 0.0, 0.0, 0.0 |
| p4_g_5 | Dynamodb | float64 | 2 | 28.74% | 0.0, 0.0, 0.0 |
| p4_g_6 | Coachdb | float64 | 2 | 28.74% | 0.0, 0.0, 0.0 |
| p4_g_7 | Cassandra | float64 | 2 | 28.74% | 0.0, 0.0, 0.0 |
| p4_g_8 | Mongodb | float64 | 2 | 28.74% | 0.0, 1.0, 0.0 |
| p4_g_9 | Mariadb | float64 | 2 | 28.74% | 0.0, 0.0, 0.0 |
| p4_g_10 | Datomic | float64 | 2 | 28.74% | 0.0, 0.0, 0.0 |
| p4_g_11 | S3 | float64 | 2 | 28.74% | 1.0, 0.0, 0.0 |
| p4_g_12 | Postgresql | float64 | 2 | 28.74% | 0.0, 0.0, 0.0 |
| p4_g_13 | Elasticsearch | float64 | 2 | 28.74% | 0.0, 0.0, 0.0 |
| p4_g_14 | Db2 | float64 | 2 | 28.74% | 0.0, 0.0, 0.0 |
| p4_g_15 | Microsoft Access | float64 | 2 | 28.74% | 0.0, 0.0, 0.0 |
| p4_g_16 | Sqlite | float64 | 2 | 28.74% | 0.0, 0.0, 0.0 |
| p4_g_17 | Sybase | float64 | 2 | 28.74% | 0.0, 0.0, 0.0 |
| p4_g_18 | Firebase | float64 | 2 | 28.74% | 0.0, 0.0, 0.0 |
| p4_g_19 | Vertica | float64 | 2 | 28.74% | 0.0, 0.0, 0.0 |
| p4_g_20 | Redis | float64 | 2 | 28.74% | 0.0, 0.0, 0.0 |
| p4_g_21 | Neo4J | float64 | 2 | 28.74% | 0.0, 0.0, 0.0 |
| p4_g_22 | Google Bigquery | float64 | 2 | 28.74% | 0.0, 1.0, 0.0 |
| p4_g_23 | Google Firestore | float64 | 2 | 28.74% | 0.0, 0.0, 0.0 |
| p4_g_24 | Amazon Redshift | float64 | 2 | 28.74% | 0.0, 0.0, 0.0 |
| p4_g_25 | Amazon Athena | float64 | 2 | 28.74% | 1.0, 0.0, 0.0 |
| p4_g_26 | Snowflake | float64 | 2 | 28.74% | 0.0, 0.0, 0.0 |
| p4_g_27 | Databricks | float64 | 2 | 28.74% | 0.0, 1.0, 0.0 |
| p4_g_28 | Hbase | float64 | 2 | 28.74% | 0.0, 0.0, 0.0 |
| p4_g_29 | Presto | float64 | 2 | 28.74% | 1.0, 0.0, 0.0 |
| p4_g_30 | Splunk | float64 | 2 | 28.74% | 0.0, 0.0, 0.0 |
| p4_g_31 | Sap Hana | float64 | 2 | 28.74% | 0.0, 0.0, 0.0 |
| p4_g_32 | Hive | float64 | 2 | 28.74% | 0.0, 0.0, 0.0 |
| p4_g_33 | Firebird | float64 | 2 | 28.74% | 1.0, 0.0, 0.0 |
| p4_h | Dentre As Opções Listadas | object | 175 | 31.74% | Servidores On Premise/Não utilizamos Cloud, Azure (Microsoft), Azure (Microsoft), Servidores On Premise/Não utilizamos Cloud |
| p4_h_1 | Azure Microsoft | float64 | 2 | 31.74% | 0.0, 0.0, 0.0 |
| p4_h_2 | Amazon Web Services Aws | float64 | 2 | 31.74% | 1.0, 0.0, 0.0 |
| p4_h_3 | Google Cloud Gcp | float64 | 2 | 31.74% | 0.0, 0.0, 1.0 |
| p4_h_4 | Oracle Cloud | float64 | 2 | 31.74% | 0.0, 0.0, 0.0 |
| p4_h_5 | Ibm | float64 | 2 | 31.74% | 0.0, 0.0, 0.0 |
| p4_h_6 | Servidores On Premise/Não Utilizamos Cloud | float64 | 2 | 31.74% | 0.0, 0.0, 1.0 |
| p4_h_7 | Cloud Própria | float64 | 2 | 31.74% | 0.0, 0.0, 0.0 |
| p4_i | Cloud Preferida | object | 44 | 28.75% | Azure (Microsoft), Azure (Microsoft), Amazon Web Services (AWS) |
| p4_j | Ferramenta De Bi Utilizada No Dia A Dia | object | 764 | 28.74% | Não utilizo nenhuma ferramenta de BI no trabalho, Grafana, Microsoft PowerBI, Fazemos todas as análises utilizando apenas Excel ou planilhas do google, Microsoft PowerBI |
| p4_j_1 | Microsoft Powerbi | float64 | 2 | 28.74% | 0.0, 1.0, 1.0 |
| p4_j_2 | Qlik View/Qlik Sense | float64 | 2 | 28.74% | 0.0, 0.0, 0.0 |
| p4_j_3 | Tableau | float64 | 2 | 28.74% | 0.0, 0.0, 0.0 |
| p4_j_4 | Metabase | float64 | 2 | 28.74% | 0.0, 0.0, 0.0 |
| p4_j_5 | Superset | float64 | 2 | 28.74% | 0.0, 0.0, 0.0 |
| p4_j_6 | Redash | float64 | 2 | 28.74% | 0.0, 0.0, 0.0 |
| p4_j_7 | Looker | float64 | 2 | 28.74% | 1.0, 0.0, 0.0 |
| p4_j_8 | Looker Studiogoogle Data Studio | float64 | 2 | 28.74% | 0.0, 0.0, 0.0 |
| p4_j_9 | Amazon Quicksight | float64 | 2 | 28.74% | 0.0, 0.0, 0.0 |
| p4_j_10 | Mode | float64 | 2 | 28.74% | 0.0, 0.0, 0.0 |
| p4_j_11 | Alteryx | float64 | 2 | 28.74% | 0.0, 0.0, 0.0 |
| p4_j_12 | Microstrategy | float64 | 2 | 28.74% | 0.0, 0.0, 0.0 |
| p4_j_13 | Ibm Analytics/Cognos | float64 | 2 | 28.74% | 0.0, 0.0, 0.0 |
| p4_j_14 | Sap Business Objects/Sap Analytics | float64 | 2 | 28.74% | 0.0, 0.0, 0.0 |
| p4_j_15 | Oracle Business Intelligence | float64 | 2 | 28.74% | 0.0, 0.0, 0.0 |
| p4_j_16 | Salesforce/Einstein Analytics | float64 | 2 | 28.74% | 0.0, 0.0, 0.0 |
| p4_j_17 | Birst | float64 | 2 | 28.74% | 0.0, 0.0, 0.0 |
| p4_j_18 | Sas Visual Analytics | float64 | 2 | 28.74% | 0.0, 1.0, 0.0 |
| p4_j_19 | Grafana | float64 | 2 | 28.74% | 0.0, 0.0, 0.0 |
| p4_j_20 | Tibco Spotfire | float64 | 2 | 28.74% | 0.0, 0.0, 0.0 |
| p4_j_21 | Pentaho | float64 | 2 | 28.74% | 0.0, 0.0, 0.0 |
| p4_j_22 | Fazemos Todas As Análises Utilizando Apenas Excel Ou Planilhas Do Google | float64 | 2 | 28.74% | 0.0, 0.0, 0.0 |
| p4_j_23 | Não Utilizo Nenhuma Ferramenta De Bi No Trabalho | float64 | 2 | 28.74% | 0.0, 0.0, 0.0 |
| p4_k | Qual Sua Ferramenta De Bi Preferida? | object | 91 | 28.81% | Tableau, Looker Studio, Plotly Dash |
| p4_l | Qual O Tipo De Uso De Ai Generativa E Llms Na Empresa | object | 199 | 28.74% | Não sei opinar., Não tenho visto soluções de IA Generatica e LLMs sendo tradadas como prioridade pela empresa e pessoas, os poucos casos de uso são isolados ou ainda estão muito no início., Colaboradores utilizando soluções baseadas em AI Generativa (como o ChatGPT por exemplo) de forma independente, com o objetivo de melhorar sua produtividade no dia a dia, sem um direcionamento centralizado. |
| p4_l_1 | Colaboradores Usando Ai Generativa De Forma Independente E Descentralizada | float64 | 2 | 28.74% | 1.0, 0.0, 0.0 |
| p4_l_2 | Direcionamento Centralizado Do Uso De Ai Generativa | float64 | 2 | 28.74% | 0.0, 0.0, 0.0 |
| p4_l_3 | Desenvolvedores Utilizando Copilots | float64 | 2 | 28.74% | 0.0, 0.0, 1.0 |
| p4_l_4 | Ai Generativa E Llms Para Melhorar Produtos Externos Para Os Clientes Finais | float64 | 2 | 28.74% | 1.0, 0.0, 0.0 |
| p4_l_5 | Ai Generativa E Llms Para Melhorar Produtos Internos Para Os Colaboradores | float64 | 2 | 28.74% | 0.0, 1.0, 0.0 |
| p4_l_6 | Ia Generativa E Llms Como Principal Frente Do Negócio | float64 | 2 | 28.74% | 0.0, 0.0, 1.0 |
| p4_l_7 | Ia Generativa E Llms Não É Prioridade | float64 | 2 | 28.74% | 0.0, 0.0, 0.0 |
| p4_l_8 | Não Sei Opinar Sobre O Uso De Ia Generativa E Llms Na Empresa | float64 | 2 | 28.74% | 0.0, 0.0, 0.0 |
| p4_m | Utiliza Chatgpt Ou Llms No Trabalho? | object | 22 | 28.74% | Não utilizo nenhum tipo de solução de IA Generativa para melhorar a produtividade no dia a dia., Utilizo soluções pagas de AI Generativa (como por exemplo ChatGPT plus, MidJourney etc) e pago do meu próprio bolso., Utilizo soluções no estilo "Copilot" (exemplo: Github Copilot, Amazon CodeWhisperer ou ChatGPT Plus) para ter mais produtividade no dia a dia., Utilizo apenas soluções gratuitas (como por exemplo o ChatGPT), para me ajudar a ser mais produtivo no dia a dia. |
| p4_m_1 | Não Uso Soluções De Ai Generativa Com Foco Em Produtividade | float64 | 2 | 28.74% | 0.0, 0.0, 0.0 |
| p4_m_2 | Uso Soluções Gratuitas De Ai Generativa Com Foco Em Produtividade | float64 | 2 | 28.74% | 0.0, 1.0, 1.0 |
| p4_m_3 | Uso E Pago Pelas Soluções De Ai Generativa Com Foco Em Produtividade | float64 | 2 | 28.74% | 0.0, 0.0, 0.0 |
| p4_m_4 | A Empresa Que Trabalho Paga Pelas Soluções De Ai Generativa Com Foco Em Produtividade | float64 | 2 | 28.74% | 0.0, 0.0, 0.0 |
| p4_m_5 | Uso Soluções Do Tipo Copilot | float64 | 2 | 28.74% | 1.0, 0.0, 0.0 |
| p5_a | Qual Seu Objetivo Na Área De Dados? | object | 52 | 90.08% | Primeiro emprego: Estou tentando encontrar a primeira oportunidade na área de dados, Primeiro emprego: Estou tentando encontrar a primeira oportunidade na área de dados, Preparação profissional: Estou buscando conhecimentos técnicos para no futuro assumir algum cargo na área de dados |
| p5_b | Qual Oportunidade Você Está Buscando? | object | 13 | 94.58% | Analista de Dados/Data Analyst, Analista de Dados/Data Analyst, Cientista de Dados/Data Scientist |
| p5_c | Há Quanto Tempo Você Busca Uma Oportunidade Na Área De Dados? | object | 4 | 94.58% | 0 - 6 meses, 0 - 6 meses, acima de 2 anos |
| p5_d | Como Tem Sido A Busca Por Um Emprego Na Área De Dados? | object | 6 | 94.60% | Já me candidatei, mas nunca fui chamado para entrevistas, Já me candidatei, mas nunca fui chamado para entrevistas, Ainda não me candidatei a nenhuma vaga na área |
| p6_a | Quais Das Opções Abaixo Fazem Parte Da Sua Rotina No Trabalho Atual Como Engenheiro De Dados? | object | 311 | 82.77% | Desenvolvo pipelines de dados utilizando linguagens de programação como Python, Scala, Java etc., Crio consultas através da linguagem SQL para exportar informações e compartilhar com as áreas de negócio., Modelo soluções de arquitetura de dados, criando componentes de ingestão de dados, transformação e recuperação da informação., Cuido da qualidade dos dados, metadados e dicionário de dados., Atuo na modelagem dos dados, com o objetivo de criar conjuntos de dados como Data Warehouses, Data Marts, Datasets etc., Desenvolvo pipelines de dados utilizando linguagens de programação como Python, Scala, Java etc., Realizo construções de ETL's em ferramentas como Pentaho, Talend, Dataflow etc., Modelo soluções de arquitetura de dados, criando componentes de ingestão de dados, transformação e recuperação da informação., Desenvolvo pipelines de dados utilizando linguagens de programação como Python, Scala, Java etc., Crio consultas através da linguagem SQL para exportar informações e compartilhar com as áreas de negócio., Atuo na integração de diferentes fontes de dados através de plataformas proprietárias como Stitch Data, Fivetran etc., Cuido da qualidade dos dados, metadados e dicionário de dados., Atuo na modelagem dos dados, com o objetivo de criar conjuntos de dados como Data Warehouses, Data Marts, Datasets etc., Desenvolvo/cuido da manutenção de repositórios de dados baseados em streaming de eventos como Data Lakes e Data Lakehouses., Modelo soluções de arquitetura de dados, criando componentes de ingestão de dados, transformação e recuperação da informação. |
| p6_a_1 | Desenvolvo Pipelines De Dados Utilizando Linguagens De Programação Como Python | float64 | 2 | 82.77% | 1.0, 1.0, 1.0 |
| p6_a_2 | Realizo Construções De Etls Em Ferramentas Como Pentaho | float64 | 2 | 82.77% | 0.0, 0.0, 0.0 |
| p6_a_3 | Crio Consultas Através Da Linguagem Sql Para Exportar Informações E Compartilhar Com As Áreas De Negócio. | float64 | 2 | 82.77% | 0.0, 1.0, 1.0 |
| p6_a_4 | Atuo Na Integração De Diferentes Fontes De Dados Através De Plataformas Proprietárias Como Stitch Data | float64 | 2 | 82.77% | 0.0, 0.0, 0.0 |
| p6_a_5 | Modelo Soluções De Arquitetura De Dados | float64 | 2 | 82.77% | 0.0, 0.0, 1.0 |
| p6_a_6 | Desenvolvo/Cuido Da Manutenção De Repositórios De Dados Baseados Em Streaming De Eventos Como Data Lakes E Data Lakehouses. | float64 | 2 | 82.77% | 0.0, 0.0, 0.0 |
| p6_a_7 | Atuo Na Modelagem Dos Dados | float64 | 2 | 82.77% | 1.0, 1.0, 1.0 |
| p6_a_8 | Cuido Da Qualidade Dos Dados | float64 | 2 | 82.77% | 1.0, 1.0, 1.0 |
| p6_a_9 | Nenhuma Das Opções Listadas Refletem Meu Dia A Dia. | float64 | 2 | 82.77% | 0.0, 0.0, 0.0 |
| p6_b | Quais As Ferramentas/Tecnologias De Etl Que Você Utiliza No Trabalho Como Data Engineer? | object | 357 | 82.77% | Apache Airflow, Scripts Python, Google Dataflow, SQL Server Integration Services (SSIS), Databricks, Scripts Python, Apache Airflow, Google Dataflow, Scripts Python, SQL & Stored Procedures, Apache Airflow, Fivetran, Databricks, Scripts Scala |
| p6_b_1 | Scripts Python | float64 | 2 | 82.77% | 0.0, 0.0, 1.0 |
| p6_b_2 | Sql & Stored Procedures | float64 | 2 | 82.77% | 0.0, 1.0, 1.0 |
| p6_b_3 | Apache Airflow | float64 | 2 | 82.77% | 0.0, 0.0, 0.0 |
| p6_b_4 | Apache Nifi | float64 | 2 | 82.77% | 0.0, 0.0, 0.0 |
| p6_b_5 | Luigi | float64 | 2 | 82.77% | 0.0, 0.0, 0.0 |
| p6_b_6 | Aws Glue | float64 | 2 | 82.77% | 1.0, 1.0, 0.0 |
| p6_b_7 | Talend | float64 | 2 | 82.77% | 0.0, 0.0, 0.0 |
| p6_b_8 | Pentaho | float64 | 2 | 82.77% | 0.0, 0.0, 0.0 |
| p6_b_9 | Alteryx | float64 | 2 | 82.77% | 0.0, 0.0, 0.0 |
| p6_b_10 | Stitch | float64 | 2 | 82.77% | 0.0, 0.0, 0.0 |
| p6_b_11 | Fivetran | float64 | 2 | 82.77% | 0.0, 0.0, 0.0 |
| p6_b_12 | Google Dataflow | float64 | 2 | 82.77% | 0.0, 0.0, 0.0 |
| p6_b_13 | Oracle Data Integrator | float64 | 2 | 82.77% | 0.0, 0.0, 0.0 |
| p6_b_14 | Ibm Datastage | float64 | 2 | 82.77% | 0.0, 0.0, 0.0 |
| p6_b_15 | Sap Bw Etl | float64 | 2 | 82.77% | 0.0, 0.0, 0.0 |
| p6_b_16 | Sql Server Integration Services Ssis | float64 | 2 | 82.77% | 0.0, 0.0, 0.0 |
| p6_b_17 | Sas Data Integration | float64 | 2 | 82.77% | 0.0, 0.0, 0.0 |
| p6_b_18 | Qlik Sense | float64 | 2 | 82.77% | 0.0, 0.0, 0.0 |
| p6_b_19 | Knime | float64 | 2 | 82.77% | 0.0, 0.0, 0.0 |
| p6_b_20 | Databricks | float64 | 2 | 82.77% | 0.0, 0.0, 0.0 |
| p6_b_21 | Não Utilizo Ferramentas De Etl | float64 | 2 | 82.77% | 0.0, 0.0, 0.0 |
| p6_c | Sua Organização Possui Um Data Lake? | float64 | 2 | 82.79% | 1.0, 1.0, 1.0 |
| p6_d | Qual Tecnologia Utilizada Como Plataforma Do Data Lake? | object | 7 | 85.98% | Snowflake, Google FS + BigQuery, Google FS + BigQuery |
| p6_e | Sua Organização Possui Um Data Warehouse? | float64 | 2 | 82.83% | 1.0, 1.0, 1.0 |
| p6_f | Qual Tecnologia Utilizada Como Plataforma Do Data Warehouse? | object | 10 | 86.04% | Google BigQuery, AWS Redshift, Azure |
| p6_g | Quais As Ferramentas De Gestão De Qualidade De Dados | object | 13 | 89.51% | great\_expectations, great\_expectations, dbt |
| p6_h | Em Qual Das Opções Abaixo Você Gasta A Maior Parte Do Seu Tempo? | object | 59 | 82.77% | Modelando soluções de arquitetura de dados, criando componentes de ingestão de dados, transformação e recuperação da informação., Desenvolvendo pipelines de dados utilizando linguagens de programação como Python, Scala, Java etc., Atuando na modelagem dos dados, com o objetivo de criar conjuntos de dados como Data Warehouses, Data Marts, Datasets etc., Modelando soluções de arquitetura de dados, criando componentes de ingestão de dados, transformação e recuperação da informação. |
| p6_h_1 | Desenvolvendo Pipelines De Dados Utilizando Linguagens De Programação Como Python | float64 | 2 | 82.77% | 0.0, 1.0, 0.0 |
| p6_h_2 | Realizando Construções De Etls Em Ferramentas Como Pentaho | float64 | 2 | 82.77% | 0.0, 0.0, 0.0 |
| p6_h_3 | Criando Consultas Através Da Linguagem Sql Para Exportar Informações E Compartilhar Com As Áreas De Negócio. | float64 | 2 | 82.77% | 1.0, 0.0, 0.0 |
| p6_h_4 | Atuando Na Integração De Diferentes Fontes De Dados Através De Plataformas Proprietárias Como Stitch Data | float64 | 2 | 82.77% | 0.0, 0.0, 0.0 |
| p6_h_5 | Modelando Soluções De Arquitetura De Dados | float64 | 2 | 82.77% | 0.0, 0.0, 0.0 |
| p6_h_6 | Desenvolvendo/Cuidando Da Manutenção De Repositórios De Dados Baseados Em Streaming De Eventos Como Data Lakes E Data Lakehouses. | float64 | 2 | 82.77% | 0.0, 0.0, 0.0 |
| p6_h_7 | Atuando Na Modelagem Dos Dados | float64 | 2 | 82.77% | 1.0, 0.0, 0.0 |
| p6_h_8 | Cuidando Da Qualidade Dos Dados | float64 | 2 | 82.77% | 1.0, 0.0, 0.0 |
| p6_h_9 | Nenhuma Das Opções Listadas Refletem Meu Dia A Dia. | float64 | 2 | 82.77% | 0.0, 0.0, 0.0 |
| p7_1 | Quais Das Opções Abaixo Fazem Parte Da Sua Rotina No Trabalho Atual Com Análise De Dados? | object | 415 | 66.09% | Processo e analiso dados utilizando linguagens de programação como Python, R etc., Realizo construções de dashboards em ferramentas de BI como PowerBI, Tableau, Looker, Qlik etc., Crio consultas através da linguagem SQL para exportar informações e compartilhar com as áreas de negócio., Utilizo API's para extrair dados e complementar minhas análises., Realizo construções de dashboards em ferramentas de BI como PowerBI, Tableau, Looker, Qlik etc., Crio consultas através da linguagem SQL para exportar informações e compartilhar com as áreas de negócio., Realizo construções de dashboards em ferramentas de BI como PowerBI, Tableau, Looker, Qlik etc., Crio consultas através da linguagem SQL para exportar informações e compartilhar com as áreas de negócio. |
| p7_a_1 | Processo E Analiso Dados Utilizando Linguagens De Programação Como Python | float64 | 2 | 66.09% | 0.0, 1.0, 1.0 |
| p7_a_2 | Realizo Construções De Dashboards Em Ferramentas De Bi Como Powerbi | float64 | 2 | 66.09% | 1.0, 1.0, 1.0 |
| p7_a_3 | Crio Consultas Através Da Linguagem Sql Para Exportar Informações E Compartilhar Com As Áreas De Negócio. | float64 | 2 | 66.09% | 1.0, 1.0, 0.0 |
| p7_a_4 | Utilizo Apis Para Extrair Dados E Complementar Minhas Análises. | float64 | 2 | 66.09% | 1.0, 0.0, 1.0 |
| p7_a_5 | Realizo Experimentos E Estudos Utilizando Metodologias Estatísticas Como Teste De Hipótese | float64 | 2 | 66.09% | 0.0, 0.0, 0.0 |
| p7_a_6 | Desenvolvo/Cuido Da Manutenção De Etls Utilizando Tecnologias Como Talend | float64 | 2 | 66.09% | 0.0, 0.0, 0.0 |
| p7_a_7 | Atuo Na Modelagem Dos Dados | float64 | 2 | 66.09% | 1.0, 0.0, 0.0 |
| p7_a_8 | Desenvolvo/Cuido Da Manutenção De Planilhas Para Atender As Áreas De Negócio. | float64 | 2 | 66.09% | 1.0, 0.0, 0.0 |
| p7_a_9 | Utilizo Ferramentas Avançadas De Estatística Como Sass | float64 | 2 | 66.09% | 0.0, 0.0, 0.0 |
| p7_a_10 | Nenhuma Das Opções Listadas Refletem Meu Dia A Dia. | float64 | 2 | 66.09% | 0.0, 0.0, 0.0 |
| p7_b | Quais As Ferramentas/Tecnologias De Etl Que Você Utiliza No Trabalho Como Data Analyst? | object | 372 | 66.09% | Scripts Python, Scripts Python, Google Dataflow, Não utilizo ferramentas de ETL |
| p7_b_1 | Scripts Python | float64 | 2 | 66.09% | 0.0, 0.0, 0.0 |
| p7_b_2 | Sql & Stored Procedures | float64 | 2 | 66.09% | 0.0, 1.0, 1.0 |
| p7_b_3 | Apache Airflow | float64 | 2 | 66.09% | 0.0, 0.0, 0.0 |
| p7_b_4 | Apache Nifi | float64 | 2 | 66.09% | 0.0, 0.0, 0.0 |
| p7_b_5 | Luigi | float64 | 2 | 66.09% | 0.0, 0.0, 0.0 |
| p7_b_6 | Aws Glue | float64 | 2 | 66.09% | 0.0, 0.0, 0.0 |
| p7_b_7 | Talend | float64 | 2 | 66.09% | 0.0, 0.0, 0.0 |
| p7_b_8 | Pentaho | float64 | 2 | 66.09% | 0.0, 0.0, 0.0 |
| p7_b_9 | Alteryx | float64 | 2 | 66.09% | 0.0, 0.0, 0.0 |
| p7_b_10 | Stitch | float64 | 2 | 66.09% | 0.0, 0.0, 0.0 |
| p7_b_11 | Fivetran | float64 | 2 | 66.09% | 0.0, 0.0, 0.0 |
| p7_b_12 | Google Dataflow | float64 | 2 | 66.09% | 0.0, 0.0, 0.0 |
| p7_b_13 | Oracle Data Integrator | float64 | 2 | 66.09% | 0.0, 0.0, 0.0 |
| p7_b_14 | Ibm Datastage | float64 | 2 | 66.09% | 0.0, 0.0, 0.0 |
| p7_b_15 | Sap Bw Etl | float64 | 2 | 66.09% | 0.0, 0.0, 0.0 |
| p7_b_16 | Sql Server Integration Services Ssis | float64 | 2 | 66.09% | 0.0, 0.0, 0.0 |
| p7_b_17 | Sas Data Integration | float64 | 2 | 66.09% | 0.0, 0.0, 0.0 |
| p7_b_18 | Qlik Sense | float64 | 2 | 66.09% | 0.0, 0.0, 0.0 |
| p7_b_19 | Knime | float64 | 2 | 66.09% | 0.0, 0.0, 0.0 |
| p7_b_20 | Databricks | float64 | 2 | 66.09% | 0.0, 0.0, 0.0 |
| p7_b_21 | Não Utilizo Ferramentas De Etl | float64 | 2 | 66.09% | 0.0, 0.0, 0.0 |
| p7_c | Sua Empresa Utiliza Alguma Das Ferramentas Listadas Para Dar Mais Autonomia Em Análise De Dados Para As Áreas De Negócio? | object | 32 | 66.09% | Ferramentas de análise dentro de ferramentas de CRM como Salesforce Einstein Anaytics ou Zendesk dashboards., "Point and Click" Analytics como Alteryx, Knime, Rapidminer etc., Minha empresa não utiliza essas ferramentas., Minha empresa não utiliza essas ferramentas. |
| p7_c_1 | Ferramentas De Automl Como H2O.Ai | float64 | 2 | 66.09% | 0.0, 0.0, 0.0 |
| p7_c_2 | ""Point And Click"" Analytics Como Alteryx | float64 | 2 | 66.09% | 0.0, 0.0, 1.0 |
| p7_c_3 | Product Metricts & Insights Como Mixpanel | float64 | 2 | 66.09% | 0.0, 1.0, 0.0 |
| p7_c_4 | Ferramentas De Análise Dentro De Ferramentas De Crm Como Salesforce Einstein Anaytics Ou Zendesk Dashboards. | float64 | 2 | 66.09% | 0.0, 0.0, 0.0 |
| p7_c_5 | Minha Empresa Não Utiliza Essas Ferramentas. | float64 | 2 | 66.09% | 1.0, 0.0, 0.0 |
| p7_c_6 | Não Sei Informar. | float64 | 2 | 66.09% | 0.0, 0.0, 0.0 |
| p7_d | Em Qual Das Opções Abaixo Você Gasta A Maior Parte Do Seu Tempo De Trabalho? | object | 66 | 66.09% | Realizando construções de dashboards em ferramentas de BI como PowerBI, Tableau, Looker, Qlik etc., Criando consultas através da linguagem SQL para exportar informações e compartilhar com as áreas de negócio., Realizando construções de dashboards em ferramentas de BI como PowerBI, Tableau, Looker, Qlik etc., Desenvolvendo/cuidando da manutenção de planilhas para atender as áreas de negócio. |
| p7_d_1 | Processando E Analisando Dados Utilizando Linguagens De Programação Como Python | float64 | 2 | 66.09% | 0.0, 0.0, 0.0 |
| p7_d_2 | Realizando Construções De Dashboards Em Ferramentas De Bi Como Powerbi | float64 | 2 | 66.09% | 1.0, 0.0, 1.0 |
| p7_d_3 | Criando Consultas Através Da Linguagem Sql Para Exportar Informações E Compartilhar Com As Áreas De Negócio. | float64 | 2 | 66.09% | 1.0, 1.0, 1.0 |
| p7_d_4 | Utilizando Apis Para Extrair Dados E Complementar Minhas Análises. | float64 | 2 | 66.09% | 0.0, 0.0, 0.0 |
| p7_d_5 | Realizando Experimentos E Estudos Utilizando Metodologias Estatísticas Como Teste De Hipótese | float64 | 2 | 66.09% | 0.0, 0.0, 0.0 |
| p7_d_6 | Desenvolvendo/Cuidando Da Manutenção De Etls Utilizando Tecnologias Como Talend | float64 | 2 | 66.09% | 0.0, 0.0, 0.0 |
| p7_d_7 | Atuando Na Modelagem Dos Dados | float64 | 2 | 66.09% | 0.0, 0.0, 0.0 |
| p7_d_8 | Desenvolvendo/Cuidando Da Manutenção De Planilhas Do Excel Ou Google Sheets Para Atender As Áreas De Negócio. | float64 | 2 | 66.09% | 0.0, 0.0, 1.0 |
| p7_d_9 | Utilizando Ferramentas Avançadas De Estatística Como Sas | float64 | 2 | 66.09% | 0.0, 0.0, 0.0 |
| p7_d_10 | Nenhuma Das Opções Listadas Refletem Meu Dia A Dia. | float64 | 2 | 66.09% | 0.0, 0.0, 0.0 |
| p8_a | Quais Das Opções Abaixo Fazem Parte Da Sua Rotina No Trabalho Atual Com Ciência De Dados? | object | 438 | 85.87% | Estudos Ad-hoc com o objetivo de confirmar hipóteses, realizar modelos preditivos, forecasts, análise de cluster para resolver problemas pontuais e responder perguntas das áreas de negócio., Sou responsável por entrar em contato com os times de negócio para definição do problema, identificar a solução e apresentação de resultados., Desenvolvo modelos de Machine Learning com o objetivo de colocar em produção em sistemas (produtos de dados)., Treinando e aplicando LLM's para solucionar problemas de negócio., Cuido da manutenção de modelos de Machine Learning já em produção, atuando no monitoramento, ajustes e refatoração quando necessário., Desenvolvo modelos de Machine Learning com o objetivo de colocar em produção em sistemas (produtos de dados)., Estudos Ad-hoc com o objetivo de confirmar hipóteses, realizar modelos preditivos, forecasts, análise de cluster para resolver problemas pontuais e responder perguntas das áreas de negócio., Realizo construções de dashboards em ferramentas de BI como PowerBI, Tableau, Looker, Qlik, etc., Desenvolvo modelos de Machine Learning com o objetivo de colocar em produção em sistemas (produtos de dados)., Sou responsável pela coleta e limpeza dos dados que uso para análise e modelagem., Sou responsável por entrar em contato com os times de negócio para definição do problema, identificar a solução e apresentação de resultados., Estudos Ad-hoc com o objetivo de confirmar hipóteses, realizar modelos preditivos, forecasts, análise de cluster para resolver problemas pontuais e responder perguntas das áreas de negócio. |
| p8_a_1 | Estudos Ad-Hoc Com O Objetivo De Confirmar Hipóteses | float64 | 2 | 85.87% | 1.0, 0.0, 1.0 |
| p8_a_2 | Sou Responsável Pela Coleta E Limpeza Dos Dados Que Uso Para Análise E Modelagem. | float64 | 2 | 85.87% | 1.0, 1.0, 0.0 |
| p8_a_3 | Sou Responsável Por Entrar Em Contato Com Os Times De Negócio Para Definição Do Problema | float64 | 2 | 85.87% | 1.0, 0.0, 1.0 |
| p8_a_4 | Desenvolvo Modelos De Machine Learning Com O Objetivo De Colocar Em Produção Em Sistemas Produtos De Dados. | float64 | 2 | 85.87% | 0.0, 1.0, 1.0 |
| p8_a_5 | Sou Responsável Por Colocar Modelos Em Produção | float64 | 2 | 85.87% | 1.0, 1.0, 0.0 |
| p8_a_6 | Cuido Da Manutenção De Modelos De Machine Learning Já Em Produção | float64 | 2 | 85.87% | 0.0, 1.0, 0.0 |
| p8_a_7 | Realizo Construções De Dashboards Em Ferramentas De Bi Como Powerbi | float64 | 2 | 85.87% | 0.0, 0.0, 1.0 |
| p8_a_8 | Utilizo Ferramentas Avançadas De Estatística Como Sas | float64 | 2 | 85.87% | 0.0, 0.0, 0.0 |
| p8_a_9 | Crio E Dou Manutenção Em Etls | float64 | 2 | 85.87% | 0.0, 1.0, 1.0 |
| p8_a_10 | Crio E Gerencio Soluções De Feature Store E Cultura De Mlops. | float64 | 2 | 85.87% | 0.0, 0.0, 0.0 |
| p8_a_11 | Sou Responsável Por Criar E Manter A Infra Que Meus Modelos E Soluções Rodam Clusters | float64 | 2 | 85.87% | 1.0, 0.0, 0.0 |
| p8_a_12 | Treino E Aplico Llms Para Solucionar Problemas De Negócio. | float64 | 2 | 85.87% | 0.0, 0.0, 0.0 |
| p8_b | Quais As Técnicas E Métodos Listados Abaixo Você Costuma Utilizar No Trabalho? | object | 470 | 85.87% | Utilizo modelos de regressão (linear, logística, GLM)., Utilizo redes neurais ou modelos baseados em árvore para criar modelos de classificação., Utilizo métodos estatísticos clássicos (Testes de hipótese, análise multivariada, sobrevivência, dados longitudinais, inferência estatística) para analisar dados., Utilizo modelos de regressão (linear, logística, GLM)., Utilizo redes neurais ou modelos baseados em árvore para criar modelos de classificação., Utilizo métodos de Visão Computacional., Utilizo redes neurais ou modelos baseados em árvore para criar modelos de classificação., Desenvolvo sistemas de recomendação (RecSys)., Utilizo métodos estatísticos clássicos (Testes de hipótese, análise multivariada, sobrevivência, dados longitudinais, inferência estatística) para analisar dados. |
| p8_b_1 | Utilizo Modelos De Regressão Linear | float64 | 2 | 85.87% | 1.0, 1.0, 0.0 |
| p8_b_2 | Utilizo Redes Neurais Ou Modelos Baseados Em Árvore Para Criar Modelos De Classificação | float64 | 2 | 85.87% | 0.0, 1.0, 1.0 |
| p8_b_3 | Desenvolvo Sistemas De Recomendação Recsys | float64 | 2 | 85.87% | 0.0, 0.0, 0.0 |
| p8_b_4 | Utilizo Métodos Estatísticos Bayesianos Para Analisar Dados | float64 | 2 | 85.87% | 0.0, 0.0, 0.0 |
| p8_b_5 | Utilizo Técnicas De Nlp Natural Language Processing Para Análisar Dados Não-Estruturados | float64 | 2 | 85.87% | 0.0, 1.0, 1.0 |
| p8_b_6 | Utilizo Métodos Estatísticos Clássicos Testes De Hipótese | float64 | 2 | 85.87% | 0.0, 1.0, 1.0 |
| p8_b_7 | Utilizo Cadeias De Markov Ou Hmms Para Realizar Análises De Dados | float64 | 2 | 85.87% | 0.0, 0.0, 0.0 |
| p8_b_8 | Desenvolvo Técnicas De Clusterização K-Means | float64 | 2 | 85.87% | 1.0, 1.0, 0.0 |
| p8_b_9 | Realizo Previsões Através De Modelos De Séries Temporais Time Series | float64 | 2 | 85.87% | 1.0, 0.0, 0.0 |
| p8_b_10 | Utilizo Modelos De Reinforcement Learning Aprendizado Por Reforço | float64 | 2 | 85.87% | 0.0, 0.0, 0.0 |
| p8_b_11 | Utilizo Modelos De Machine Learning Para Detecção De Fraude | float64 | 2 | 85.87% | 0.0, 0.0, 1.0 |
| p8_b_12 | Utilizo Métodos De Visão Computacional | float64 | 2 | 85.87% | 0.0, 0.0, 1.0 |
| p8_b_13 | Utilizo Modelos De Detecção De Churn | float64 | 2 | 85.87% | 1.0, 0.0, 0.0 |
| p8_b_14 | Utilizo Llms Para Solucionar Problemas De Negócio | float64 | 2 | 85.87% | 0.0, 0.0, 1.0 |
| p8_3 | Quais Dessas Tecnologias Fazem Parte Do Seu Dia A Dia Como Cientista De Dados? | object | 403 | 85.87% | Feature Store (Feast, Hopsworks, AWS Feature Store, Databricks Feature Store etc)., Planilhas (Excel, Google Sheets etc)., Ambientes de desenvolvimento local (R-studio, JupyterLab, Anaconda)., Ambientes de desenvolvimento na nuvem (Google Colab, AWS Sagemaker, Kaggle Notebooks etc)., Sistemas de controle de versão (Github, DVC, Neptune, Gitlab etc)., Sistemas de controle de versão (Github, DVC, Neptune, Gitlab etc). |
| p8_c_1 | Ferramentas De Bi Powerbi | float64 | 2 | 85.87% | 0.0, 0.0, 0.0 |
| p8_c_2 | Planilhas Excel | float64 | 2 | 85.87% | 1.0, 0.0, 1.0 |
| p8_c_3 | Ambientes De Desenvolvimento Local R-Studio | float64 | 2 | 85.87% | 1.0, 1.0, 1.0 |
| p8_c_4 | Ambientes De Desenvolvimento Na Nuvem Google Colab | float64 | 2 | 85.87% | 0.0, 1.0, 1.0 |
| p8_c_5 | Ferramentas De Automl Datarobot | float64 | 2 | 85.87% | 0.0, 0.0, 1.0 |
| p8_c_6 | Ferramentas De Etl Apache Airflow | float64 | 2 | 85.87% | 0.0, 1.0, 0.0 |
| p8_c_7 | Plataformas De Machine Learning Tensorflow | float64 | 2 | 85.87% | 0.0, 0.0, 0.0 |
| p8_c_8 | Feature Store Feast | float64 | 2 | 85.87% | 0.0, 0.0, 0.0 |
| p8_c_9 | Sistemas De Controle De Versão Github | float64 | 2 | 85.87% | 0.0, 1.0, 0.0 |
| p8_c_10 | Plataformas De Data Apps Streamlit | float64 | 2 | 85.87% | 0.0, 1.0, 0.0 |
| p8_c_11 | Ferramentas De Estatística Avançada Como Spss | float64 | 2 | 85.87% | 0.0, 0.0, 0.0 |
| p8_d | Em Qual Das Opções Abaixo Você Gasta A Maior Parte Do Seu Tempo No Trabalho? | object | 87 | 85.87% | Coletando e limpando dos dados que uso para análise e modelagem., Treinando e aplicando LLM's para solucionar problemas de negócio., Coletando e limpando dos dados que uso para análise e modelagem., Coletando e limpando dos dados que uso para análise e modelagem., Entrando em contato com os times de negócio para definição do problema, identificar a solução e apresentação de resultados. |
| p8_d_1 | Estudos Ad-Hoc Com O Objetivo De Confirmar Hipóteses | float64 | 2 | 85.87% | 0.0, 1.0, 1.0 |
| p8_d_2 | Coletando E Limpando Os Dados Que Uso Para Análise E Modelagem. | float64 | 2 | 85.87% | 0.0, 1.0, 1.0 |
| p8_d_3 | Entrando Em Contato Com Os Times De Negócio Para Definição Do Problema | float64 | 2 | 85.87% | 0.0, 0.0, 0.0 |
| p8_d_4 | Desenvolvendo Modelos De Machine Learning Com O Objetivo De Colocar Em Produção Em Sistemas Produtos De Dados. | float64 | 2 | 85.87% | 0.0, 0.0, 0.0 |
| p8_d_5 | Colocando Modelos Em Produção | float64 | 2 | 85.87% | 0.0, 1.0, 0.0 |
| p8_d_6 | Cuidando Da Manutenção De Modelos De Machine Learning Já Em Produção | float64 | 2 | 85.87% | 0.0, 0.0, 0.0 |
| p8_d_7 | Realizando Construções De Dashboards Em Ferramentas De Bi Como Powerbi | float64 | 2 | 85.87% | 0.0, 0.0, 0.0 |
| p8_d_8 | Utilizando Ferramentas Avançadas De Estatística Como Sas | float64 | 2 | 85.87% | 0.0, 0.0, 1.0 |
| p8_d_9 | Criando E Dando Manutenção Em Etls | float64 | 2 | 85.87% | 0.0, 0.0, 0.0 |
| p8_d_10 | Criando E Gerenciando Soluções De Feature Store E Cultura De Mlops. | float64 | 2 | 85.87% | 0.0, 0.0, 0.0 |
| p8_d_11 | Criando E Mantendo A Infra Que Meus Modelos E Soluções Rodam Clusters | float64 | 2 | 85.87% | 0.0, 0.0, 0.0 |
| p8_d_12 | Treinando E Aplicando Llms Para Solucionar Problemas De Negócio. | float64 | 2 | 85.87% | 0.0, 0.0, 0.0 |

## Estatísticas Gerais

- **Total de Colunas**: 399
- **Total de Registros**: 5293
- **Colunas Categóricas**: 69
- **Colunas Numéricas**: 330
- **Colunas com >50% Faltantes**: 233

## Dicionário de Dados

| Código Completo | Descrição Detalhada |
|------------------|---------------------|
| p0 | Id |
| p1_a | Idade |
| p1_a_1 | Faixa Idade |
| p1_b | Genero |
| p1_c | Cor/Raca/Etnia |
| p1_d | Pcd |
| p1_e | Experiencia_Profissional_Prejudicada |
| p1_e_1 | Não Acredito Que Minha Experiência Profissional Seja Afetada |
| p1_e_2 | Experiencia Prejudicada Devido A Minha Cor Raça Etnia |
| p1_e_3 | Experiencia Prejudicada Devido A Minha Identidade De Gênero |
| p1_e_4 | Experiencia Prejudicada Devido Ao Fato De Ser Pcd |
| p1_f | Aspectos_Prejudicados |
| p1_f_1 | Quantidade De Oportunidades De Emprego/Vagas Recebidas |
| p1_f_2 | Senioridade Das Vagas Recebidas Em Relação À Sua Experiência |
| p1_f_3 | Aprovação Em Processos Seletivos/Entrevistas |
| p1_f_4 | Oportunidades De Progressão De Carreira |
| p1_f_5 | Velocidade De Progressão De Carreira |
| p1_f_6 | Nível De Cobrança No Trabalho/Stress No Trabalho |
| p1_f_7 | Atenção Dada Diante Das Minhas Opiniões E Ideias |
| p1_f_8 | Relação Com Outros Membros Da Empresa |
| p1_f_9 | Relação Com Outros Membros Da Empresa |
| p1_g | Vive_No_Brasil |
| p1_i | Estado Onde Mora |
| p1_i_1 | Uf Onde Mora |
| p1_i_2 | Regiao Onde Mora |
| p1_j | Mudou De Estado? |
| p1_k | Regiao De Origem |
| p1_l | Nivel De Ensino |
| p1_m | Área De Formação |
| p2_a | Qual Sua Situação Atual De Trabalho? |
| p2_b | Setor |
| p2_c | Numero De Funcionarios |
| p2_d | Gestor? |
| p2_e | Cargo Como Gestor |
| p2_f | Cargo Atual |
| p2_g | Nivel |
| p2_h | Faixa Salarial |
| p2_i | Quanto Tempo De Experiência Na Área De Dados Você Tem? |
| p2_j | Quanto Tempo De Experiência Na Área De Ti/Engenharia De Software Você Teve Antes De Começar A Trabalhar Na Área De Dados? |
| p2_k | Você Está Satisfeito Na Sua Empresa Atual? |
| p2_l | Qual O Principal Motivo Da Sua Insatisfação Com A Empresa Atual? |
| p2_l_1 | Falta De Oportunidade De Crescimento No Emprego Atual |
| p2_l_2 | Salário Atual Não Corresponde Ao Mercado |
| p2_l_3 | Não Tenho Uma Boa Relação Com Meu Líder/Gestor |
| p2_l_4 | Gostaria De Trabalhar Em Em Outra Área De Atuação |
| p2_l_5 | Gostaria De Receber Mais Benefícios |
| p2_l_6 | O Clima De Trabalho/Ambiente Não É Bom |
| p2_l_7 | Falta De Maturidade Analítica Na Empresa |
| p2_m | Você Participou De Entrevistas De Emprego Nos Últimos 6 Meses? |
| p2_n | Você Pretende Mudar De Emprego Nos Próximos 6 Meses? |
| p2_o | Quais Os Principais Critérios Que Você Leva Em Consideração No Momento De Decidir Onde Trabalhar? |
| p2_o_1 | Remuneração/Salário |
| p2_o_10 | Reputação Que A Empresa Tem No Mercado |
| p2_o_2 | Benefícios |
| p2_o_3 | Propósito Do Trabalho E Da Empresa |
| p2_o_4 | Flexibilidade De Trabalho Remoto |
| p2_o_5 | Ambiente E Clima De Trabalho |
| p2_o_6 | Oportunidade De Aprendizado E Trabalhar Com Referências Na Área |
| p2_o_7 | Plano De Carreira E Oportunidades De Crescimento Profissional |
| p2_o_8 | Maturidade Da Empresa Em Termos De Tecnologia E Dados |
| p2_o_9 | Qualidade Dos Gestores E Líderes |
| p2_q | Empresa Que Trabaha Passou Por Layoff Em 2023 |
| p2_r | Atualmente Qual A Sua Forma De Trabalho? |
| p2_s | Qual A Forma De Trabalho Ideal Para Você? |
| p2_t | Caso Sua Empresa Decida Pelo Modelo 100% Presencial Qual Será Sua Atitude? |
| p3_a | Qual O Número Aproximado De Pessoas Que Atuam Com Dados Na Sua Empresa Hoje? |
| p3_b | Quais Desses Papéis/Cargos Fazem Parte Do Time Ou Chapter De Dados Da Sua Empresa? |
| p3_b_1 | Analytics Engineer |
| p3_b_2 | Engenharia De Dados/Data Engineer |
| p3_b_3 | Analista De Dados/Data Analyst |
| p3_b_4 | Cientista De Dados/Data Scientist |
| p3_b_5 | Database Administrator/Dba |
| p3_b_6 | Analista De Business Intelligence/Bi |
| p3_b_7 | Arquiteto De Dados/Data Architect |
| p3_b_8 | Data Product Manager/Dpm |
| p3_b_9 | Business Analyst |
| p3_c | Quais Dessas Responsabilidades Fazem Parte Da Sua Rotina Atual De Trabalho Como Gestor? |
| p3_c_1 | Pensar Na Visão De Longo Prazo De Dados Da Empresa E Fortalecimento Da Cultura Analítica Da Companhia. |
| p3_c_10 | Gestão De Produtos De Dados |
| p3_c_11 | Gestão De Pessoas |
| p3_c_2 | Organização De Treinamentos E Iniciativas Com O Objetivo De Aumentar A Maturidade Analítica Das Áreas De Negócios. |
| p3_c_3 | Atração |
| p3_c_4 | Decisão Sobre Contratação De Ferramentas E Tecnologias Relacionadas A Dados. |
| p3_c_5 | Sou Gestor Da Equipe Responsável Pela Engenharia De Dados E Por Manter O Data Lake Da Empresa Como Fonte Única Dos Dados |
| p3_c_6 | Sou Gestor Da Equipe Responsável Pela Entrega De Dados |
| p3_c_7 | Sou Gestor Da Equipe Responsável Por Iniciativas E Projetos Envolvendo Inteligência Artificial E Machine Learning. |
| p3_c_8 | Apesar De Ser Gestor Ainda Atuo Na Parte Técnica |
| p3_c_9 | Gestão De Projetos De Dados |
| p3_d | Quais São Os 3 Maiores Desafios Que Você Tem Como Gestor No Atual Momento? |
| p3_d_1 | A Contratar Novos Talentos. |
| p3_d_10 | J Gerenciar A Expectativa Das Áreas De Negócio Em Relação As Entregas Das Equipes De Dados. |
| p3_d_11 | K Garantir A Manutenção Dos Projetos E Modelos Em Produção |
| p3_d_12 | Conseguir Levar Inovação Para A Empresa Através Dos Dados. |
| p3_d_13 | Garantir Retorno Do Investimento Roi Em Projetos De Dados. |
| p3_d_14 | Dividir O Tempo Entre Entregas Técnicas E Gestão. |
| p3_d_2 | B Reter Talentos. |
| p3_d_3 | C Convencer A Empresa A Aumentar Os Investimentos Na Área De Dados. |
| p3_d_4 | D Gestão De Equipes No Ambiente Remoto. |
| p3_d_5 | E Gestão De Projetos Envolvendo Áreas Multidisciplinares Da Empresa. |
| p3_d_6 | F Organizar As Informações E Garantir A Qualidade E Confiabilidade. |
| p3_d_7 | G Conseguir Processar E Armazenar Um Alto Volume De Dados. |
| p3_d_8 | H Conseguir Gerar Valor Para As Áreas De Negócios Através De Estudos E Experimentos. |
| p3_d_9 | I Desenvolver E Manter Modelos Machine Learning Em Produção. |
| p3_e | Ai Generativa É Uma Prioridade Em Sua Empresa? |
| p3_f | Tipos De Uso De Ai Generativa E Llms Na Empresa |
| p3_f_1 | Colaboradores Usando Ai Generativa De Forma Independente E Descentralizada |
| p3_f_2 | Direcionamento Centralizado Do Uso De Ai Generativa |
| p3_f_3 | Desenvolvedores Utilizando Copilots |
| p3_f_4 | Ai Generativa E Llms Para Melhorar Produtos Externos |
| p3_f_5 | Ai Generativa E Llms Para Melhorar Produtos Internos Para Os Colaboradores |
| p3_f_6 | Ia Generativa E Llms Como Principal Frente Do Negócio |
| p3_f_7 | Ia Generativa E Llms Não É Prioridade |
| p3_f_8 | Não Sei Opinar Sobre O Uso De Ia Generativa E Llms Na Empresa |
| p3_g | Motivos Que Levam A Empresa A Não Usar Ai Genrativa E Llms |
| p3_g_1 | Falta De Compreensão Dos Casos De Uso |
| p3_g_2 | Falta De Confiabilidade Das Saídas Alucinação Dos Modelos |
| p3_g_3 | Incerteza Em Relação A Regulamentação |
| p3_g_4 | Preocupações Com Segurança E Privacidade De Dados |
| p3_g_5 | Retorno Sobre Investimento Roi Não Comprovado De Ia Generativa |
| p3_g_6 | Dados Da Empresa Não Estão Prontos Para Uso De Ia Generativa |
| p3_g_7 | Falta De Expertise Ou Falta De Recursos |
| p3_g_8 | Alta Direção Da Empresa Não Vê Valor Ou Não Vê Como Prioridade |
| p3_g_9 | Preocupações Com Propriedade Intelectual |
| p4_a | Mesmo Que Esse Não Seja Seu Cargo Formal |
| p4_a_1 | Atuacao |
| p4_b | Quais Das Fontes De Dados Listadas Você Já Analisou Ou Processou No Trabalho? |
| p4_b_1 | Dados Relacionais Estruturados Em Bancos Sql |
| p4_b_2 | Dados Armazenados Em Bancos Nosql |
| p4_b_3 | Imagens |
| p4_b_4 | Textos/Documentos |
| p4_b_5 | Vídeos |
| p4_b_6 | Áudios |
| p4_b_7 | Planilhas |
| p4_b_8 | Dados Georeferenciados |
| p4_c | Entre As Fontes De Dados Listadas |
| p4_c_1 | Dados Relacionais Estruturados Em Bancos Sql |
| p4_c_2 | Dados Armazenados Em Bancos Nosql |
| p4_c_3 | Imagens |
| p4_c_4 | Textos/Documentos |
| p4_c_5 | Vídeos |
| p4_c_6 | Áudios |
| p4_c_7 | Planilhas |
| p4_c_8 | Dados Georeferenciados |
| p4_d | Quais Das Linguagens Listadas Abaixo Você Utiliza No Trabalho? |
| p4_d_1 | Sql |
| p4_d_10 | Scala |
| p4_d_11 | Matlab |
| p4_d_12 | Rust |
| p4_d_13 | Php |
| p4_d_14 | Javascript |
| p4_d_15 | Não Utilizo Nenhuma Linguagem |
| p4_d_2 | R |
| p4_d_3 | Python |
| p4_d_4 | C/C++/C# |
| p4_d_5 | .Net |
| p4_d_6 | Java |
| p4_d_7 | Julia |
| p4_d_8 | Sas/Stata |
| p4_d_9 | Visual Basic/Vba |
| p4_e | Entre As Linguagens Listadas Abaixo |
| p4_f | Entre As Linguagens Listadas Abaixo |
| p4_g | Quais Dos Bancos De Dados/Fontes De Dados Listados Abaixo Você Utiliza No Trabalho? |
| p4_g_1 | Mysql |
| p4_g_10 | Datomic |
| p4_g_11 | S3 |
| p4_g_12 | Postgresql |
| p4_g_13 | Elasticsearch |
| p4_g_14 | Db2 |
| p4_g_15 | Microsoft Access |
| p4_g_16 | Sqlite |
| p4_g_17 | Sybase |
| p4_g_18 | Firebase |
| p4_g_19 | Vertica |
| p4_g_2 | Oracle |
| p4_g_20 | Redis |
| p4_g_21 | Neo4J |
| p4_g_22 | Google Bigquery |
| p4_g_23 | Google Firestore |
| p4_g_24 | Amazon Redshift |
| p4_g_25 | Amazon Athena |
| p4_g_26 | Snowflake |
| p4_g_27 | Databricks |
| p4_g_28 | Hbase |
| p4_g_29 | Presto |
| p4_g_3 | Sql Server |
| p4_g_30 | Splunk |
| p4_g_31 | Sap Hana |
| p4_g_32 | Hive |
| p4_g_33 | Firebird |
| p4_g_4 | Amazon Aurora Ou Rds |
| p4_g_5 | Dynamodb |
| p4_g_6 | Coachdb |
| p4_g_7 | Cassandra |
| p4_g_8 | Mongodb |
| p4_g_9 | Mariadb |
| p4_h | Dentre As Opções Listadas |
| p4_h_1 | Azure Microsoft |
| p4_h_2 | Amazon Web Services Aws |
| p4_h_3 | Google Cloud Gcp |
| p4_h_4 | Oracle Cloud |
| p4_h_5 | Ibm |
| p4_h_6 | Servidores On Premise/Não Utilizamos Cloud |
| p4_h_7 | Cloud Própria |
| p4_i | Cloud Preferida |
| p4_j | Ferramenta De Bi Utilizada No Dia A Dia |
| p4_j_1 | Microsoft Powerbi |
| p4_j_10 | Mode |
| p4_j_11 | Alteryx |
| p4_j_12 | Microstrategy |
| p4_j_13 | Ibm Analytics/Cognos |
| p4_j_14 | Sap Business Objects/Sap Analytics |
| p4_j_15 | Oracle Business Intelligence |
| p4_j_16 | Salesforce/Einstein Analytics |
| p4_j_17 | Birst |
| p4_j_18 | Sas Visual Analytics |
| p4_j_19 | Grafana |
| p4_j_2 | Qlik View/Qlik Sense |
| p4_j_20 | Tibco Spotfire |
| p4_j_21 | Pentaho |
| p4_j_22 | Fazemos Todas As Análises Utilizando Apenas Excel Ou Planilhas Do Google |
| p4_j_23 | Não Utilizo Nenhuma Ferramenta De Bi No Trabalho |
| p4_j_3 | Tableau |
| p4_j_4 | Metabase |
| p4_j_5 | Superset |
| p4_j_6 | Redash |
| p4_j_7 | Looker |
| p4_j_8 | Looker Studiogoogle Data Studio |
| p4_j_9 | Amazon Quicksight |
| p4_k | Qual Sua Ferramenta De Bi Preferida? |
| p4_l | Qual O Tipo De Uso De Ai Generativa E Llms Na Empresa |
| p4_l_1 | Colaboradores Usando Ai Generativa De Forma Independente E Descentralizada |
| p4_l_2 | Direcionamento Centralizado Do Uso De Ai Generativa |
| p4_l_3 | Desenvolvedores Utilizando Copilots |
| p4_l_4 | Ai Generativa E Llms Para Melhorar Produtos Externos Para Os Clientes Finais |
| p4_l_5 | Ai Generativa E Llms Para Melhorar Produtos Internos Para Os Colaboradores |
| p4_l_6 | Ia Generativa E Llms Como Principal Frente Do Negócio |
| p4_l_7 | Ia Generativa E Llms Não É Prioridade |
| p4_l_8 | Não Sei Opinar Sobre O Uso De Ia Generativa E Llms Na Empresa |
| p4_m | Utiliza Chatgpt Ou Llms No Trabalho? |
| p4_m_1 | Não Uso Soluções De Ai Generativa Com Foco Em Produtividade |
| p4_m_2 | Uso Soluções Gratuitas De Ai Generativa Com Foco Em Produtividade |
| p4_m_3 | Uso E Pago Pelas Soluções De Ai Generativa Com Foco Em Produtividade |
| p4_m_4 | A Empresa Que Trabalho Paga Pelas Soluções De Ai Generativa Com Foco Em Produtividade |
| p4_m_5 | Uso Soluções Do Tipo Copilot |
| p5_a | Qual Seu Objetivo Na Área De Dados? |
| p5_b | Qual Oportunidade Você Está Buscando? |
| p5_c | Há Quanto Tempo Você Busca Uma Oportunidade Na Área De Dados? |
| p5_d | Como Tem Sido A Busca Por Um Emprego Na Área De Dados? |
| p6_a | Quais Das Opções Abaixo Fazem Parte Da Sua Rotina No Trabalho Atual Como Engenheiro De Dados? |
| p6_a_1 | Desenvolvo Pipelines De Dados Utilizando Linguagens De Programação Como Python |
| p6_a_2 | Realizo Construções De Etls Em Ferramentas Como Pentaho |
| p6_a_3 | Crio Consultas Através Da Linguagem Sql Para Exportar Informações E Compartilhar Com As Áreas De Negócio. |
| p6_a_4 | Atuo Na Integração De Diferentes Fontes De Dados Através De Plataformas Proprietárias Como Stitch Data |
| p6_a_5 | Modelo Soluções De Arquitetura De Dados |
| p6_a_6 | Desenvolvo/Cuido Da Manutenção De Repositórios De Dados Baseados Em Streaming De Eventos Como Data Lakes E Data Lakehouses. |
| p6_a_7 | Atuo Na Modelagem Dos Dados |
| p6_a_8 | Cuido Da Qualidade Dos Dados |
| p6_a_9 | Nenhuma Das Opções Listadas Refletem Meu Dia A Dia. |
| p6_b | Quais As Ferramentas/Tecnologias De Etl Que Você Utiliza No Trabalho Como Data Engineer? |
| p6_b_1 | Scripts Python |
| p6_b_10 | Stitch |
| p6_b_11 | Fivetran |
| p6_b_12 | Google Dataflow |
| p6_b_13 | Oracle Data Integrator |
| p6_b_14 | Ibm Datastage |
| p6_b_15 | Sap Bw Etl |
| p6_b_16 | Sql Server Integration Services Ssis |
| p6_b_17 | Sas Data Integration |
| p6_b_18 | Qlik Sense |
| p6_b_19 | Knime |
| p6_b_2 | Sql & Stored Procedures |
| p6_b_20 | Databricks |
| p6_b_21 | Não Utilizo Ferramentas De Etl |
| p6_b_3 | Apache Airflow |
| p6_b_4 | Apache Nifi |
| p6_b_5 | Luigi |
| p6_b_6 | Aws Glue |
| p6_b_7 | Talend |
| p6_b_8 | Pentaho |
| p6_b_9 | Alteryx |
| p6_c | Sua Organização Possui Um Data Lake? |
| p6_d | Qual Tecnologia Utilizada Como Plataforma Do Data Lake? |
| p6_e | Sua Organização Possui Um Data Warehouse? |
| p6_f | Qual Tecnologia Utilizada Como Plataforma Do Data Warehouse? |
| p6_g | Quais As Ferramentas De Gestão De Qualidade De Dados |
| p6_h | Em Qual Das Opções Abaixo Você Gasta A Maior Parte Do Seu Tempo? |
| p6_h_1 | Desenvolvendo Pipelines De Dados Utilizando Linguagens De Programação Como Python |
| p6_h_2 | Realizando Construções De Etls Em Ferramentas Como Pentaho |
| p6_h_3 | Criando Consultas Através Da Linguagem Sql Para Exportar Informações E Compartilhar Com As Áreas De Negócio. |
| p6_h_4 | Atuando Na Integração De Diferentes Fontes De Dados Através De Plataformas Proprietárias Como Stitch Data |
| p6_h_5 | Modelando Soluções De Arquitetura De Dados |
| p6_h_6 | Desenvolvendo/Cuidando Da Manutenção De Repositórios De Dados Baseados Em Streaming De Eventos Como Data Lakes E Data Lakehouses. |
| p6_h_7 | Atuando Na Modelagem Dos Dados |
| p6_h_8 | Cuidando Da Qualidade Dos Dados |
| p6_h_9 | Nenhuma Das Opções Listadas Refletem Meu Dia A Dia. |
| p7_1 | Quais Das Opções Abaixo Fazem Parte Da Sua Rotina No Trabalho Atual Com Análise De Dados? |
| p7_a_1 | Processo E Analiso Dados Utilizando Linguagens De Programação Como Python |
| p7_a_10 | Nenhuma Das Opções Listadas Refletem Meu Dia A Dia. |
| p7_a_2 | Realizo Construções De Dashboards Em Ferramentas De Bi Como Powerbi |
| p7_a_3 | Crio Consultas Através Da Linguagem Sql Para Exportar Informações E Compartilhar Com As Áreas De Negócio. |
| p7_a_4 | Utilizo Apis Para Extrair Dados E Complementar Minhas Análises. |
| p7_a_5 | Realizo Experimentos E Estudos Utilizando Metodologias Estatísticas Como Teste De Hipótese |
| p7_a_6 | Desenvolvo/Cuido Da Manutenção De Etls Utilizando Tecnologias Como Talend |
| p7_a_7 | Atuo Na Modelagem Dos Dados |
| p7_a_8 | Desenvolvo/Cuido Da Manutenção De Planilhas Para Atender As Áreas De Negócio. |
| p7_a_9 | Utilizo Ferramentas Avançadas De Estatística Como Sass |
| p7_b | Quais As Ferramentas/Tecnologias De Etl Que Você Utiliza No Trabalho Como Data Analyst? |
| p7_b_1 | Scripts Python |
| p7_b_10 | Stitch |
| p7_b_11 | Fivetran |
| p7_b_12 | Google Dataflow |
| p7_b_13 | Oracle Data Integrator |
| p7_b_14 | Ibm Datastage |
| p7_b_15 | Sap Bw Etl |
| p7_b_16 | Sql Server Integration Services Ssis |
| p7_b_17 | Sas Data Integration |
| p7_b_18 | Qlik Sense |
| p7_b_19 | Knime |
| p7_b_2 | Sql & Stored Procedures |
| p7_b_20 | Databricks |
| p7_b_21 | Não Utilizo Ferramentas De Etl |
| p7_b_3 | Apache Airflow |
| p7_b_4 | Apache Nifi |
| p7_b_5 | Luigi |
| p7_b_6 | Aws Glue |
| p7_b_7 | Talend |
| p7_b_8 | Pentaho |
| p7_b_9 | Alteryx |
| p7_c | Sua Empresa Utiliza Alguma Das Ferramentas Listadas Para Dar Mais Autonomia Em Análise De Dados Para As Áreas De Negócio? |
| p7_c_1 | Ferramentas De Automl Como H2O.Ai |
| p7_c_2 | ""Point And Click"" Analytics Como Alteryx |
| p7_c_3 | Product Metricts & Insights Como Mixpanel |
| p7_c_4 | Ferramentas De Análise Dentro De Ferramentas De Crm Como Salesforce Einstein Anaytics Ou Zendesk Dashboards. |
| p7_c_5 | Minha Empresa Não Utiliza Essas Ferramentas. |
| p7_c_6 | Não Sei Informar. |
| p7_d | Em Qual Das Opções Abaixo Você Gasta A Maior Parte Do Seu Tempo De Trabalho? |
| p7_d_1 | Processando E Analisando Dados Utilizando Linguagens De Programação Como Python |
| p7_d_10 | Nenhuma Das Opções Listadas Refletem Meu Dia A Dia. |
| p7_d_2 | Realizando Construções De Dashboards Em Ferramentas De Bi Como Powerbi |
| p7_d_3 | Criando Consultas Através Da Linguagem Sql Para Exportar Informações E Compartilhar Com As Áreas De Negócio. |
| p7_d_4 | Utilizando Apis Para Extrair Dados E Complementar Minhas Análises. |
| p7_d_5 | Realizando Experimentos E Estudos Utilizando Metodologias Estatísticas Como Teste De Hipótese |
| p7_d_6 | Desenvolvendo/Cuidando Da Manutenção De Etls Utilizando Tecnologias Como Talend |
| p7_d_7 | Atuando Na Modelagem Dos Dados |
| p7_d_8 | Desenvolvendo/Cuidando Da Manutenção De Planilhas Do Excel Ou Google Sheets Para Atender As Áreas De Negócio. |
| p7_d_9 | Utilizando Ferramentas Avançadas De Estatística Como Sas |
| p8_3 | Quais Dessas Tecnologias Fazem Parte Do Seu Dia A Dia Como Cientista De Dados? |
| p8_a | Quais Das Opções Abaixo Fazem Parte Da Sua Rotina No Trabalho Atual Com Ciência De Dados? |
| p8_a_1 | Estudos Ad-Hoc Com O Objetivo De Confirmar Hipóteses |
| p8_a_10 | Crio E Gerencio Soluções De Feature Store E Cultura De Mlops. |
| p8_a_11 | Sou Responsável Por Criar E Manter A Infra Que Meus Modelos E Soluções Rodam Clusters |
| p8_a_12 | Treino E Aplico Llms Para Solucionar Problemas De Negócio. |
| p8_a_2 | Sou Responsável Pela Coleta E Limpeza Dos Dados Que Uso Para Análise E Modelagem. |
| p8_a_3 | Sou Responsável Por Entrar Em Contato Com Os Times De Negócio Para Definição Do Problema |
| p8_a_4 | Desenvolvo Modelos De Machine Learning Com O Objetivo De Colocar Em Produção Em Sistemas Produtos De Dados. |
| p8_a_5 | Sou Responsável Por Colocar Modelos Em Produção |
| p8_a_6 | Cuido Da Manutenção De Modelos De Machine Learning Já Em Produção |
| p8_a_7 | Realizo Construções De Dashboards Em Ferramentas De Bi Como Powerbi |
| p8_a_8 | Utilizo Ferramentas Avançadas De Estatística Como Sas |
| p8_a_9 | Crio E Dou Manutenção Em Etls |
| p8_b | Quais As Técnicas E Métodos Listados Abaixo Você Costuma Utilizar No Trabalho? |
| p8_b_1 | Utilizo Modelos De Regressão Linear |
| p8_b_10 | Utilizo Modelos De Reinforcement Learning Aprendizado Por Reforço |
| p8_b_11 | Utilizo Modelos De Machine Learning Para Detecção De Fraude |
| p8_b_12 | Utilizo Métodos De Visão Computacional |
| p8_b_13 | Utilizo Modelos De Detecção De Churn |
| p8_b_14 | Utilizo Llms Para Solucionar Problemas De Negócio |
| p8_b_2 | Utilizo Redes Neurais Ou Modelos Baseados Em Árvore Para Criar Modelos De Classificação |
| p8_b_3 | Desenvolvo Sistemas De Recomendação Recsys |
| p8_b_4 | Utilizo Métodos Estatísticos Bayesianos Para Analisar Dados |
| p8_b_5 | Utilizo Técnicas De Nlp Natural Language Processing Para Análisar Dados Não-Estruturados |
| p8_b_6 | Utilizo Métodos Estatísticos Clássicos Testes De Hipótese |
| p8_b_7 | Utilizo Cadeias De Markov Ou Hmms Para Realizar Análises De Dados |
| p8_b_8 | Desenvolvo Técnicas De Clusterização K-Means |
| p8_b_9 | Realizo Previsões Através De Modelos De Séries Temporais Time Series |
| p8_c_1 | Ferramentas De Bi Powerbi |
| p8_c_10 | Plataformas De Data Apps Streamlit |
| p8_c_11 | Ferramentas De Estatística Avançada Como Spss |
| p8_c_2 | Planilhas Excel |
| p8_c_3 | Ambientes De Desenvolvimento Local R-Studio |
| p8_c_4 | Ambientes De Desenvolvimento Na Nuvem Google Colab |
| p8_c_5 | Ferramentas De Automl Datarobot |
| p8_c_6 | Ferramentas De Etl Apache Airflow |
| p8_c_7 | Plataformas De Machine Learning Tensorflow |
| p8_c_8 | Feature Store Feast |
| p8_c_9 | Sistemas De Controle De Versão Github |
| p8_d | Em Qual Das Opções Abaixo Você Gasta A Maior Parte Do Seu Tempo No Trabalho? |
| p8_d_1 | Estudos Ad-Hoc Com O Objetivo De Confirmar Hipóteses |
| p8_d_10 | Criando E Gerenciando Soluções De Feature Store E Cultura De Mlops. |
| p8_d_11 | Criando E Mantendo A Infra Que Meus Modelos E Soluções Rodam Clusters |
| p8_d_12 | Treinando E Aplicando Llms Para Solucionar Problemas De Negócio. |
| p8_d_2 | Coletando E Limpando Os Dados Que Uso Para Análise E Modelagem. |
| p8_d_3 | Entrando Em Contato Com Os Times De Negócio Para Definição Do Problema |
| p8_d_4 | Desenvolvendo Modelos De Machine Learning Com O Objetivo De Colocar Em Produção Em Sistemas Produtos De Dados. |
| p8_d_5 | Colocando Modelos Em Produção |
| p8_d_6 | Cuidando Da Manutenção De Modelos De Machine Learning Já Em Produção |
| p8_d_7 | Realizando Construções De Dashboards Em Ferramentas De Bi Como Powerbi |
| p8_d_8 | Utilizando Ferramentas Avançadas De Estatística Como Sas |
| p8_d_9 | Criando E Dando Manutenção Em Etls |