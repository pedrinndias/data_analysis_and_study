# Disparidade Salarial dos Profissionais de Dados no Brasil

**Pedro Dias Soares, [pdsoares@sga.pucminas.br]** 

---

Professores:

**Hugo Bastos de Paula**

**Hayala Nepomuceno Curto**


---
---

_Curso de Ciência de Dados, Unidade Praça da Liberdade_

_Instituto de Informática e Ciências Exatas – Pontifícia Universidade de Minas Gerais (PUC MINAS), Belo Horizonte – MG – Brasil_

---
## Sumário

*   [Resumo](#resumo)
*   [Introdução](#introdução)
    *   [Contextualização](#contextualização)
    *   [Problema](#problema)
    *   [Objetivo geral](#objetivo-geral)
    *   [Justificativas](#justificativas)
*   [Público alvo](#público-alvo)
*   [Dicionário de dados](#dicionário-de-dados)
*   [Descrição de dados](#descrição-de-dados)
*   [Preparação dos dados](#preparação-dos-dados)
*   [Enriquecimento de dados](#enriquecimento-de-dados)
*   [Analises exploratorias de dados](#analises-exploratorias-de-dados) 
    *   [1º Pergunta Orientada a Dados](#1º-pergunta-orientada-a-dados)
*   [Indução de modelos](#indução-de-modelos)
    *   [Modelos 1° pergunta orietada a dados](#modelos-1º-pergunta-orietada-a-dados)
*   [Resultados](#resultados)
    *   [Resultados obtidos com os Modelos 1º pergunta orietada a dados](#resultados-obtidos-com-os-modelos-1º-pergunta-orietada-a-dados)
*   [Interpretação do modelo](#interpretação-dos-modelos)
    *   [Interpretação dos Modelos 1° pergunta orietada a dados](#interpretação-dos-modelo-1º-pergunta-orientada-a-dados)
*   [Análise comparativa dos modelos](#análise-comparativa-dos-modelos)
*   [Conclusão](#8-conclusão)
*   [REFERÊNCIAS](#referências)
*   [APÊNDICES](#apêndices)


---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

# Resumo

A disparidade salarial entre profissionais de dados no Brasil é influenciada por diversos fatores pessoais, educacionais e de mercado. Este estudo busca identificar quais variáveis impactam a remuneração desses profissionais, analisando dados da pesquisa State of Data Brazil 2023 e de bases auxiliares. Para isso, são exploradas características como experiência, formação acadêmica, setor de atuação, localização e habilidades técnicas. Através de modelagem preditiva, os resultados indicam que experiência, nível de senioridade e setor da empresa são os fatores com maior impacto na variação salarial. Esses insights podem auxiliar profissionais e empresas na tomada de decisões estratégicas sobre carreira e políticas de remuneração.

---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

## Introdução

O Brasil experimentou um crescimento exponencial na indústria de dados devido à transformação digital do país e à crescente necessidade de trabalhadores qualificados. Embora as oportunidades sejam abundantes, os salários variam amplamente entre os trabalhadores, com fatores como experiência, gênero, educação, localização geográfica e tipo de empresa influenciando essa disparidade.

O objetivo deste estudo é identificar os principais fatores associados à disparidade na remuneração dos profissionais de dados no Brasil, utilizando informações coletadas de uma ampla pesquisa setorial.

As disparidades salariais entre os profissionais de dados no Brasil são influenciadas por diversos fatores como idade, gênero dos profissionais de dados, do setor de emprego ou modelo de contratação e ainda o seu histórico educacional e experiência profissional.

Este estudo investiga os principais elementos que estão associados à variação de salários no campo de dados ao utilizar o conjunto de dados State of Data Brazil 2023 e outras bases para complementar a pesquisa. Empregando métodos da ciência de dados, busca-se identificar padrões salariais e oferecer insights relevantes para profissionais e empresas. Espera-se que os resultados tragam um maior entendimento das disparidades salariais no campo, ajudando a desenvolver estratégias que incentivem a igualdade no mercado de tecnologia e ciência de dados.

---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

###    Contextualização

A desigualdade salarial é um desafio enfrentado no mercado de trabalho brasileiro, impactando diversos setores da economia.

Estudos do IBGE apontam que gênero, etnia e escolaridade são fatores cruciais na determinação dos salários. De acordo com as pesquisas de 2022 do instituto, o rendimento médio por hora dos trabalhadores brancos foi de R$ 20,00, enquanto para pretos ou pardos foi de R$ 12,40, representando uma diferença de 61,4%. Além disso, pesquisas do mesmo em 2021 indicam que as taxas de desocupação foram de 11,3% para brancos, 16,5% para pretos e 16,2% para pardos, evidenciando a influência desses aspectos na disparidade salarial na atualidade.

No setor de tecnologia, essas disparidades têm características particulares, especialmente devido ao desenvolvimento acelerado da área e à necessidade contínua de atualização profissional. Na ciência de dados, as diferenças salariais são significativas e influenciadas por fatores como a experiência, formação acadêmica, setor de atuação e habilidades técnicas.

De acordo com o relatório State of Data Brazil 2023, profissionais que possuem certificações específicas em grandes empresas costumam receber remunerações mais altas, enquanto mulheres e grupos minoritários ainda encontram barreiras para alcançar igualdade salarial. 

Diante do exposto, buscamos por meio desta análise de dados, investigar os fatores determinantes para a variação salarial entre os profissionais de dados no Brasil, visando compreender melhor as desigualdades no setor e identificar caminhos para um mercado mais equitativo.

---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

###    Problema

O agente em questão busca estabelecer quais são os fatores determinantes para a variação salarial entre profissionais de dados no Brasil. Constantemente, empresas brasileiras enfrentam dificuldades em determinar um salário justo ao profissional de dados por não considerarem os requisitos e as variáveis necessárias para isso. Nesse contexto, a análise busca entender o papel de fatores como experiência e nível educacional nas diferenças salariais, visando fornecer um padrão para que o mercado profissional da área seja mais equilibrado no país.

---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

###    Objetivo geral

**Desenvolver um sistema inteligente para compreender os fatores que influenciam a variação salarial dos profissionais de dados no Brasil, e para auxiliar na equiparação salarial desses, utilizando técnicas de ciência de dados para identificar padrões e tendências.**

####    Objetivos específicos

1. **Exploração e Análise dos Dados:**
    - Extrair da base de dados State of Data Brazil 2023 e bases auxiliares, dados suficientes para identificar variáveis relevantes associadas aos salários.
      
2. **Identificação de Fatores Relevantes:**
    - Analisar variáveis e compreender o papel de cada uma na carreira profissional do cientista de dados brasileiro, como o nível de experiência, o setor de atuação, o nível educacional, as habilidades técnicas, o gênero e a etnia.
      
3. **Aplicação de Modelos Preditivos:**
    - Aplicar por meio de algoritmos de aprendizado de máquina, a previsão da variação salarial com base nos fatores identificados.
      
4. **Interpretação dos Resultados:**
    - Aplicar por meio de algoritmos de aprendizado de máquina, a previsão da variação salarial com base nos fatores identificados.
      
5. **Geração de Insights para o Mercado:**
    - Fornecer recomendações baseadas nos achados, para auxiliar profissionais de dados e empresas na atribuição de salários aos profissionais da área.

---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

###    Justificativas

A desigualdade salarial na área de dados é um tema relevante, impactando profissionais e empresas. Este estudo busca identificar os principais fatores associados aos salários, com foco na experiência, senioridade e setor de atuação. O estudo se destina a profissionais da área que podem utilizar os resultados para planejar suas carreiras, e às empresas, que podem aprimorar suas políticas salariais com base em dados concretos. A pesquisa se apoia em bases de dados reconhecidas, como a State of Data Brazil 2023 da Data Hackers, garantindo a validade e confiabilidade das análises realizadas.

---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

##    Público alvo

Os principais perfis de usuários da aplicação são:

Profissionais de dados: Os quais possuem conhecimento técnico variado. Estão familiarizados com ferramentas de análise e visualização de dados, além de linguagens como Python e SQL. No ambiente corporativo, ocupam cargos que vão de analistas a cientistas de dados sêniores.

Gestores e recrutadores de RH: Estes utilizam plataformas de análise salarial para embasar decisões estratégicas. Eles ocupam posições hierárquicas que incluem gerentes, diretores e especialistas em aquisição de talentos.

Pesquisadores e acadêmicos: Aqueles que têm conhecimento analítico e estatístico. Utilizam tecnologias para explorar padrões e tendências em dados salariais e estão inseridos em universidades, centros de pesquisa e órgãos governamentais.

Órgãos governamentais e associações da indústria: Esses utilizam a aplicação para obter informações detalhadas sobre o mercado de trabalho e salários, visando formular políticas públicas, regulamentações e padrões da indústria. Estão envolvidos com dados que ajudam a orientar legislações e relatórios sobre tendências econômicas e de emprego.

A aplicação será útil para esses grupos ao oferecer maneiras de visualizar intuitivas, comparações salariais e insights baseados em machine learning.

## 🎯 Público-alvo da aplicação

A aplicação tem como objetivo fornecer insights sobre disparidade salarial na área de dados no Brasil, ajudando diferentes perfis de usuários a tomar decisões estratégicas. 

## 🏢 Stakeholders e seus papéis

| **Stakeholder**                 | **Nível de Interesse** | **Influência** | **Objetivos** |
|---------------------------------|----------------------|--------------|--------------|
| **Profissionais de Dados**          | Alto                 | Média        | Avaliar sua posição no mercado e planejar crescimento. |
| **Gestores e Recrutadores de RH**   | Alto                 | Alta         | Ajustar faixas salariais e estruturar políticas de retenção. |
| **Pesquisadores e Acadêmicos**      | Médio                | Média        | Explorar padrões e desigualdades no mercado. |
| **Órgãos Governamentais**           | Médio                | Alta         | Criar regulamentações e políticas de inclusão. |

## 👥 Perfis de usuários (Personas)

### **1️⃣ Persona: Analista de Dados Júnior**
- **Nome:** Lucas Mendes  
- **Idade:** 25 anos  
- **Objetivo:** Comparar sua faixa salarial com o mercado para planejar seu crescimento profissional.  
- **Desafios:** Não sabe quais habilidades influenciam no aumento salarial.  

### **2️⃣ Persona: Gerente de RH em Tecnologia**
- **Nome:** Mariana Costa  
- **Idade:** 38 anos  
- **Objetivo:** Definir pacotes salariais competitivos para atrair talentos na área de dados.  
- **Desafios:** Falta de dados estruturados sobre o mercado e diferenças regionais.  

### **3️⃣ Persona: Pesquisador de Mercado de Trabalho**
- **Nome:** Dr. João Ribeiro  
- **Idade:** 45 anos  
- **Objetivo:** Estudar desigualdades salariais no setor de tecnologia.  
- **Desafios:** Precisa de dados confiáveis e ferramentas estatísticas para análise.  

### **4️⃣ Persona: Regulador de Políticas Públicas**
- **Nome:** Ana Beatriz Oliveira  
- **Idade:** 50 anos  
- **Objetivo:** Criar diretrizes para reduzir a disparidade salarial na tecnologia.  
- **Desafios:** Necessita de informações claras e de fácil interpretação.

---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

###    Dicionário de dados

O banco de dados "State of Data Brazil 2023" é o resultado de uma pesquisa conduzida pela comunidade Data Hackers em parceria com a Bain & Company, que visa mapear o mercado brasileiro de dados. A pesquisa contou com a participação de mais de 5.200 profissionais da área, que responderam a perguntas sobre diversos temas, por exemplo:

- **Fatores Pessoais e Demográficos:** Idade, gênero; Perfil racial e diversidade dentro do setor de dados; Contexto social e fatores que podem influenciar a carreira na área de dados.

- **Experiência profissional prejudicada (discriminação):** 

- **Experiência e Carreira:** Tempo de atuação no mercado de dados; Cargos ocupados e progressão na carreira; Transições de carreira para a área de dados.

- **Empresa e Ambiente de Trabalho:**  Tipo e porte da empresa em que os profissionais trabalham; Modelo de trabalho (remoto, híbrido ou presencial); Cultura organizacional e satisfação no ambiente de trabalho.

---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

###    Descrição de dados
1. State_of_Data_BR_2023
A pesquisa State_of_Data_BR_2023 é realizada anualmente com o objetivo de mapear o perfil dos profissionais de dados no Brasil. Ela abrange informações como salários, ferramentas utilizadas, nível de experiência, formação acadêmica e outros aspectos relevantes.

**Salários Médio por Gênero:**  
gênero  
Feminino           R$ 7.000,00  
Masculino         R$ 10.000,00  
Não Informado      R$ 7.000,00  
Nome: `salary_midpoint`, `dtype: object`  

**Salários Médio por Etnia:**  
etnia  
Asiático          R$ 10.000,00  
Negro              R$ 7.000,00  
Indígena           R$ 5.000,00  
Pardo              R$ 7.000,00  
Não Informado      R$ 7.000,00  
Branco            R$ 10.000,00  
Nome: `salary_midpoint`, `dtype: object`  

**Salários Médio por Nível de Educação:**  
nível_educacional  
Graduação                  R$ 7.000,00  
Mestrado                  R$ 10.000,00  
Sem Educação Formal        R$ 5.000,00  
Doutorado                 R$ 14.000,00  
Pós-graduação             R$ 10.000,00  
Estudante de Graduação     R$ 3.500,00  
Nome: `salary_midpoint`, `dtype: object`  

**Salários Médio por Senioridade:**  
senioridade  
Júnior         R$ 3.500,00  
Pleno          R$ 7.000,00  
Sênior        R$ 10.000,00  
Nome: `salary_midpoint`, `dtype: object`  

**Salários Médio por Função:**  
função_atual  
Engenheiro de Analytics       R$ 10.000,00  
Engenheiro/Arquiteto de Dados R$ 10.000,00  
Professor/Pesquisador         R$ 10.000,00  
Economista                    R$ 10.000,00  
Cientista de Dados            R$ 10.000,00  
Analista de Negócios           R$ 7.000,00  
Analista de Dados              R$ 7.000,00  
Desenvolvedor de Software      R$ 7.000,00  
Analista de BI                 R$ 5.000,00  
Nome: `salary_midpoint`, `dtype: object`  

**Salários Médio por Indústria:**  
indústria  
Finanças/Bancos          R$ 10.000,00  
Indústria                R$ 10.000,00  
Internet/E-commerce      R$ 10.000,00  
Tecnologia/Software      R$ 10.000,00  
Varejo                   R$ 10.000,00  
Educação                  R$ 7.000,00  
Setor Público             R$ 7.000,00  
Marketing                 R$ 5.000,00  
Nome: `salary_midpoint`, `dtype: object`  

**Salários Médio por Região:**  
região  
Centro-oeste    R$ 10.000,00  
Sudeste         R$ 10.000,00  
Nordeste         R$ 7.000,00  
Norte            R$ 7.000,00  
Sul              R$ 7.000,00  
Nome: `salary_midpoint`, `dtype: object`  

**Diferença Salarial por Gênero:** 42,86% (Mediana Masculino: R$ 10.000,00; Mediana Feminino: R$ 7.000,00)  

**Diferença Salarial Branco-Negro:** 42,86% (Mediana Branco: R$ 10.000,00; Mediana Negro: R$ 7.000,00)   
**Diferença Salarial Branco-Pardo:** 42,86% (Mediana Branco: R$ 10.000,00; Mediana Pardo: R$ 7.000,00)  

**Correlação entre Experiência Total e Salário:** 0,54   
**Correlação entre Nível Educacional e Salário:** 0,32

---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------


## Preparação dos dados



### Atributos relevantes da base de dados principal para 1ºpergunta orientada
**Pergunta orientada a dados:** *Como fatores como formação acadêmica e experiência profissional interagem para influenciar a disparidade salarial entre profissionais de dados no Brasil?*


| Atributo                                         | Nome                                      | Tipo         | Subtipo                             | Descrição                                                                                     | Relevância |
|--------------------------------------------------|-------------------------------------------|--------------|-------------------------------------|-----------------------------------------------------------------------------------------------|------------|
| P0                                               | id                 		       | Qualitativo  | Nominal                             | Para identificação da resposta                                    		            | Alta       |
| P1l                                              | Nível de ensino alcançado                 | Qualitativo  | Ordinal                             | Nível de ensino do respondente (graduação, mestrado, etc.)                                    | Alta       |
| P1m                                              | Área de formação acadêmica                | Qualitativo  | Nominal (Multivalorado)             | Área de formação acadêmica do respondente (TI, Economia, etc.)                                | Alta       |
| P2h                                              | Faixa salarial mensal                     | Qualitativo  | Ordinal                             | Faixa salarial mensal do respondente                                                          | Alta       |
| P2i                                              | Tempo de experiência na área de dados     | Quantitativo | Discreto                            | Tempo de experiência do respondente na área de dados (em anos)                                | Alta       |
| P2g                                              | Nível de senioridade                      | Qualitativo  | Ordinal                             | Nível de senioridade do respondente (Júnior, Pleno, Sênior)                                   | Alta       |
| P1b                                              | Gênero do profissional                    | Qualitativo  | Nominal (Multivalorado)             | Identidade de gênero do respondente                                                           | Alta       |
| P1c                                              | Cor/Raça/Etnia                            | Qualitativo  | Nominal (Multivalorado)             | Cor ou raça do respondente                                                                    | Alta       |
| P2b                                              | Setor de atuação da empresa               | Qualitativo  | Nominal (Multivalorado)             | Setor em que a empresa do respondente atua (Tecnologia, Finanças, etc.)                       | Alta       |
| P1i1                                             | UF onde mora                              | Qualitativo  | Nominal (Multivalorado)             | Unidade Federativa onde o respondente reside                                                  | Alta       |
| P2f                                              | Cargo atual                               | Qualitativo  | Nominal (Multivalorado)             | Cargo atual ocupado pelo respondente                                                          | Alta       |
| P2o6                                             | Oportunidade de aprendizado               | Qualitativo  | Nominal (Multivalorado)             | Valorização das oportunidades de aprendizado e crescimento profissional                       | Alta       |
| P2o10                                            | Reputação da empresa                      | Qualitativo  | Nominal (Multivalorado)             | Valorização da reputação que a empresa tem no mercado                                         | Alta       |

---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

## Enriquecimento de dados

### Base de dados auxiliar para 1º pergunta orientada a dados
**Pergunta orientada a dados:** *Como fatores como formação acadêmica e experiência profissional interagem para influenciar a disparidade salarial entre profissionais de dados no Brasil?*
- Microdados do Censo da Educação Superior
- Link: https://www.gov.br/inep/pt-br/acesso-a-informacao/dados-abertos/microdados/censo-da-educacao-superior
  
- [Base de dados](/assets/data/bases_principais/bases_auxiliar/1_pergunta_orientada_a_dados/MICRODADOS_ED_SUP_IES_2023.CSV)

---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

# Analises exploratorias de dados

*   [1º Pergunta orientada a dados ](#1º-pergunta-orientada-a-dados)
  
	*   [Analise exploratoria de dados base de dados State of Data 2023](#analise-exploratoria-de-dados-base-de-dados-state-of-data-2023) 
		   *    [Grafico Distribuição de Salários Mensais](#grafico-distribuição-de-salários-mensais) 
		   *   	[Grafico Relação entre Salário e Tempo de Experiência](#grafico-relação-entre-salário-e-tempo-de-experiência) 
		   *   	[Grafico Distribuição Salarial por Nível de Ensino](#grafico-distribuição-salarial-por-nível-de-ensino) 
		   *   	[Grafico Interação entre Escolaridade, Experiência e Salário](#grafico-interação-entre-escolaridade-experiência-e-salário) 
		   *   	[Grafico Mapa de Calor de Correlações](#grafico-mapa-de-calor-de-correlações) 
		   *   	[Grafico Distribuição por Gênero e Raça-Etnia](#grafico-distribuição-por-gênero-e-raça-etnia) 
		   *   	[Grafico Distribuição Geográfica dos Profissionais](#grafico-distribuição-geográfica-dos-profissionais) 
		   *   	[Grafico Salário por Nível de Senioridade](#grafico-salário-por-nível-de-senioridade) 
		   *   	[Grafico Análise Multivariada das Relações entre Variáveis Selecionadas](#grafico-análise-multivariada-das-relações-entre-variáveis-selecionadas) 
		   *   	[Grafico Sunburst da Distribuição de Profissionais de Dados](#grafico-sunburst-da-distribuição-de-profissionais-de-dados) 


	*   [Analise exploratoria de dados base de dados Microdados](#analise-exploratoria-de-dados-base-de-dados-microdados) 
		   *   	[Grafico Distribuição Nacional de Níveis de Formação dos Docentes](#grafico-distribuição-nacional-de-níveis-de-formação-dos-docentes) 
		   *   	[Grafico Top 10 Estados por Nível de Formação de Docentes](#grafico-top-10-estados-por-nível-de-formação-de-docentes) 
		   *   	[Grafico Distribuição Etária Nacional dos Docentes](#grafico-distribuição-etária-nacional-dos-docentes) 
		   *   	[Grafico Matriz de Correlação entre Formação e Faixa Etária](#grafico-matriz-de-correlação-entre-formação-e-faixa-etária) 
		   *   	[Grafico Mapa Interativo de Bolhas - Distribuição de Docentes por Nível de Formação e UF](#grafico-mapa-interativo-de-bolhas---distribuição-de-docentes-por-nível-de-formação-e-uf) 
		   *   	[Gráfico de Dispersão 3D Interativo - Mestrado, Doutorado e Média de Idade dos Docentes por UF](#grafico-gráfico-de-dispersão-3d-interativo---mestrado-doutorado-e-média-de-idade-dos-docentes-por-uf) 


	*   [Analise exploratoria de dados bases integradas](#analise-exploratoria-de-dados-bases-integradas) 
		   *   	[Grafico Salário Médio Estimado e Total de Docentes por UF](#grafico-salário-médio-estimado-e-total-de-docentes-por-uf) 
		   *   	[Grafico Salário Estimado por Área de Formação - Top 5](#grafico-salário-estimado-por-área-de-formação---top-5) 
		   *   	[Grafico Salário Estimado por Tempo de Experiência](#grafico-salário-estimado-por-tempo-de-experiência) 
		   *   	[Grafico Salário Estimado por Tempo de Experiência em Dados](#grafico-salário-estimado-por-tempo-de-experiência-em-dados)
		   *   	[Grafico Salário Estimado por Nível de Ensino](#grafico-salário-estimado-por-nível-de-ensino) 
		   *   	[Grafico Salário Estimado por Experiência, Agrupado por Nível de Ensino](#grafico-salário-estimado-por-experiência-agrupado-por-nível-de-ensino) 
		   *   	[Grafico Distribuição de Profissionais por Área de Formação Acadêmica](#grafico-distribuição-de-profissionais-por-área-de-formação-acadêmica) 
		   *   	[Grafico Distribuição de Profissionais por Faixa Salarial Mensal](#grafico-distribuição-de-profissionais-por-faixa-salarial-mensal) 
		   *   	[Grafico Distribuição de Profissionais por Nível de Ensino](#grafico-distribuição-de-profissionais-por-nível-de-ensino) 
		   *   	[Grafico Distribuição do Salário Estimado](#grafico-distribuição-do-salário-estimado) 
		   *   	[Grafico Distribuição de Profissionais por Tempo de Experiência em Dados](#grafico-distribuição-de-profissionais-por-tempo-de-experiência-em-dados)
		   *   	[Grafico Top 10 UF de Residência dos Profissionais de Dados](#grafico-top-10-uf-de-residência-dos-profissionais-de-dados)
		   *   	[Grafico Heatmap de Correlação entre Salário, Experiência e Nível de Ensino](#grafico-heatmap-de-correlação-entre-salário-experiência-e-nível-de-ensino)
		   *   	[Grafico Salário Médio Estimado vs. Anos de Experiência por Nível de Ensino](#grafico-salário-médio-estimado-vs-anos-de-experiência-por-nível-de-ensino)
		   *   	[Grafico Relação 3D entre Salário, Experiência e Nível de Ensino](#grafico-relação-3d-entre-salário-experiência-e-nível-de-ensino)
		   *   	[Grafico Salário Estimado vs. Proporção de Docentes com Doutorado na UF de Residência](#grafico-salário-estimado-vs-proporção-de-docentes-com-doutorado-na-uf-de-residência)
		   *   	[Gráfico Relação 3D entre Salário, Experiência e Nível de Ensino](#gráfico-relação-3d-entre-salário-experiência-e-nível-de-ensino)
 

  # 1º Pergunta orientada a dados 
**Pergunta Orientada a Dados:** *Como fatores como formação acadêmica e experiência profissional interagem para influenciar a disparidade salarial entre profissionais de dados no Brasil?*

## Analise exploratoria de dados base de dados State of Data 2023

---

### Grafico Distribuição de Salários Mensais
![__results___0_1](https://github.com/user-attachments/assets/6204cac8-9875-4db3-b6d7-6bf52b038d49)
## Explicação do Gráfico: Distribuição de Salários Mensais

O gráfico apresentado é um histograma que ilustra a **Distribuição de Salários Mensais** de profissionais de dados no Brasil, com uma curva de estimativa de densidade do kernel (KDE) sobreposta para suavizar a representação da distribuição.

**Eixos do Gráfico:**
*   **Eixo X (Horizontal):** Representa o "Salário Médio (R$)", indicando as faixas salariais mensais em Reais. A escala varia de R$ 0 até valores próximos ou superiores a R$ 40.000.
*   **Eixo Y (Vertical):** Indica a "Contagem", ou seja, o número de profissionais que se enquadram em cada faixa salarial representada pelas barras do histograma. A contagem máxima observada no gráfico aproxima-se de 800 profissionais em uma determinada faixa salarial.

**Interpretação da Distribuição:**
*   **Concentração de Salários:** A maior concentração de profissionais encontra-se nas faixas salariais mais baixas. Observa-se um pico principal (a barra mais alta) na faixa de aproximadamente R$ 9.000 a R$ 10.000, onde cerca de 800 profissionais estão localizados.
*   **Múltiplos Picos (Multimodalidade):** A distribuição aparenta ser multimodal, sugerida pela curva KDE e pelas barras do histograma. Além do pico principal, há outras concentrações notáveis:
    *   Uma concentração significativa entre R$ 4.000 e R$ 6.000, com mais de 600 profissionais.
    *   Outro pico menor ao redor de R$ 13.000 a R$ 14.000, com quase 300 profissionais.
    *   Pequenas elevações em faixas salariais mais altas, como em torno de R$ 17.000-R$18.000 e R$ 22.000-R$23.000, indicando grupos menores de profissionais nesses níveis salariais.
*   **Assimetria à Direita (Right-Skewed):** A distribuição é assimétrica à direita. Isso significa que, embora a maioria dos salários esteja concentrada nas faixas mais baixas e médias, existe uma "cauda" longa para a direita, indicando que um número menor de profissionais recebe salários consideravelmente mais altos (acima de R$ 20.000, R$ 30.000, e chegando a R$ 40.000 ou mais). Essa assimetria é comum em distribuições de renda e salário.
*   **Dispersão:** Há uma grande dispersão nos salários, variando desde valores abaixo de R$ 5.000 até mais de R$ 40.000, o que reflete a diversidade de remuneração na área de dados no Brasil.

Em resumo, o gráfico mostra que a maioria dos profissionais de dados no Brasil, conforme o dataset analisado, possui salários concentrados nas faixas inferiores a R$ 15.000, com picos importantes em torno de R$ 4.000-R$6.000 e R$ 9.000-R$10.000. No entanto, existe uma parcela de profissionais que alcança remunerações significativamente mais elevadas, estendendo a distribuição para a direita.

## Grafico Relação entre Salário e Tempo de Experiência
![__results___0_2](https://github.com/user-attachments/assets/5b842f17-cbc8-46af-8bf5-7c8bf30bc7e7)
## Explicação do Gráfico: Relação entre Salário e Tempo de Experiência

O gráfico de boxplot intitulado "Relação entre Salário e Tempo de Experiência" ilustra como a faixa salarial numérica ("Faixa_salarial_num") varia conforme o "Tempo de experiência na área de dados" no Brasil.

**Como ler este gráfico de Boxplot:**
*   **Caixa (Box):** Representa o intervalo interquartil (IQR), onde se concentram 50% dos salários. A linha inferior da caixa é o primeiro quartil (Q1 - 25º percentil), e a linha superior é o terceiro quartil (Q3 - 75º percentil).
*   **Linha dentro da Caixa:** Indica a mediana (Q2 - 50º percentil), que é o valor salarial central para cada grupo de experiência.
*   **Hastess/"Bigodes" (Whiskers):** As linhas que se estendem a partir da caixa mostram o alcance dos dados, geralmente até 1,5 vezes o IQR. Pontos além dessas hastes são considerados outliers.
*   **Outliers:** São pontos individuais (losangos no gráfico) que representam salários atípicos, muito acima ou abaixo da maioria dos salários para aquele grupo de experiência.
*   **Eixo Y (Vertical):** "Faixa\_salarial\_num" representa os salários em Reais (R$), variando de R$ 0 a R$ 40.000.
*   **Eixo X (Horizontal):** "Tempo de experiência na área de dados" categoriza os profissionais em diferentes faixas de anos de experiência: "Menos de 1 ano", "de 1 a 2 anos", "de 3 a 4 anos", "de 4 a 6 anos", "de 5 a 6 anos", e "de 7 a 10 anos". As categorias no eixo X do gráfico original não estão em ordem crescente de experiência.

**Interpretação das Tendências Observadas:**

Ao analisar os boxplots para cada faixa de experiência (considerando-os em ordem crescente de experiência):

*   **Tendência Geral de Aumento Salarial com a Experiência:**
    *   **Menos de 1 ano:** Este grupo apresenta a menor mediana salarial, situando-se em torno de R$ 3.500 - R$ 4.000. A maioria dos salários (IQR) está entre aproximadamente R$ 2.000 e R$ 5.000.
    *   **De 1 a 2 anos:** A mediana salarial sobe para cerca de R$ 5.000. O IQR varia de R$ 3.500 a R$ 7.000.
    *   **De 3 a 4 anos:** Observa-se um aumento mais significativo na mediana, que se localiza em torno de R$ 8.000 - R$ 8.500. O IQR está entre R$ 5.000 e R$ 10.000.
    *   **De 4 a 6 anos / De 5 a 6 anos / De 7 a 10 anos:** Estes grupos com maior experiência apresentam medianas salariais consideravelmente mais altas e bastante próximas entre si.
        *   A mediana para "de 4 a 6 anos" e "de 5 a 6 anos" (que parecem muito similares no gráfico) está em torno de R$ 11.000 - R$ 12.000, com IQR entre R$ 10.000 e R$ 14.000.
        *   Para "de 7 a 10 anos", a mediana é ligeiramente superior, em torno de R$ 12.000 - R$ 13.000, com um IQR similar (R$ 10.000 a R$ 14.000).

*   **Variabilidade Salarial (Dispersão):**
    *   A dispersão salarial (representada pela altura da caixa e o comprimento das hastes) tende a aumentar com a experiência. Profissionais nos níveis iniciais de carreira ("Menos de 1 ano") apresentam uma faixa salarial mais concentrada em comparação com aqueles com mais experiência, onde a variabilidade é maior.
    *   Os grupos com mais experiência ("de 4 a 6 anos" em diante) mostram uma dispersão salarial maior, indicando que, embora a média seja mais alta, há uma gama mais ampla de salários sendo pagos.

*   **Outliers:**
    *   Outliers (salários muito acima do comum para o grupo) são observados em todas as categorias de experiência.
    *   Nos grupos com mais experiência (a partir de "de 3 a 4 anos"), alguns profissionais atingem salários de até R$ 40.000, indicando um potencial de alta remuneração para os mais experientes ou em posições de destaque.
    *   Mesmo no grupo com "Menos de 1 ano", existe um outlier próximo a R$ 14.000.

**Conclusão do Gráfico:**
O gráfico demonstra uma clara correlação positiva entre o tempo de experiência na área de dados e o nível salarial. Profissionais com mais anos de atuação tendem a ter salários medianos mais altos e também uma maior variabilidade salarial, com alguns indivíduos alcançando remunerações substancialmente elevadas. A progressão salarial parece ser mais acentuada nos primeiros anos de carreira, estabilizando-se em um patamar mais elevado para profissionais com 4 ou mais anos de experiência.

## Grafico Distribuição Salarial por Nível de Ensino
![__results___0_3](https://github.com/user-attachments/assets/45da8bf1-dfcc-4fac-911f-96af9f6a8b34)
## Explicação do Gráfico: Distribuição Salarial por Nível de Ensino

O gráfico de violino apresentado, intitulado "Distribuição Salarial por Nível de Ensino", exibe como a faixa salarial numérica ("Faixa\_salarial\_num") se distribui entre diferentes níveis de escolaridade alcançados por profissionais de dados no Brasil.

**Como ler este gráfico de Violino:**
*   **Forma do Violino:** A largura do violino em diferentes pontos representa a densidade dos dados naquela faixa salarial. Onde o violino é mais largo, há uma maior concentração de profissionais com salários naquele nível.
*   **Caixa Interna (Box Plot):** Dentro de cada violino, há um box plot:
    *   A **linha branca grossa** no centro da caixa indica a **mediana** salarial (o valor central).
    *   A **caixa retangular** representa o **intervalo interquartil (IQR)**, contendo 50% dos dados (do 25º ao 75º percentil).
    *   As **linhas/hastes (whiskers)** que se estendem da caixa mostram o alcance principal dos dados, e pontos além delas podem ser considerados outliers (embora o violino em si mostre a forma completa da distribuição, incluindo os extremos).
*   **Eixo Y (Vertical):** "Faixa\_salarial\_num" representa os salários em Reais (R$), variando de R$ 0 até mais de R$ 40.000.
*   **Eixo X (Horizontal):** "Nível de ensino alcançado" categoriza os profissionais pelos seguintes níveis de educação:
    *   Doutorado ou Phd
    *   Graduação/Bacharelado
    *   Estudante de Graduação
    *   Pós-graduação
    *   Mestrado

**Interpretação das Distribuições Salariais por Nível de Ensino:**

*   **Estudante de Graduação (Verde):**
    *   Apresenta a **menor mediana salarial**, localizada em torno de R$ 4.000 - R$ 5.000.
    *   A distribuição é mais concentrada em salários baixos, com a parte mais larga do violino nessa região. A maioria dos salários está abaixo de R$ 10.000, embora a cauda superior se estenda até cerca de R$ 25.000.

*   **Graduação/Bacharelado (Laranja):**
    *   A mediana salarial sobe para aproximadamente R$ 8.000 - R$ 9.000.
    *   A distribuição é mais ampla, com uma concentração significativa de salários entre R$ 5.000 e R$ 15.000. Apresenta uma cauda superior longa, indicando que alguns profissionais com esta formação atingem salários bem elevados, chegando até R$ 40.000 ou mais.

*   **Pós-graduação (Vermelho):**
    *   A mediana salarial é ligeiramente superior à de "Graduação/Bacharelado", situando-se em torno de R$ 10.000 - R$ 11.000.
    *   A forma da distribuição é semelhante à de "Graduação/Bacharelado", com uma concentração principal e uma cauda longa para salários mais altos, também atingindo valores acima de R$ 40.000. O violino parece ter uma ligeira "cintura" indicando uma menor densidade entre a concentração mais baixa e a mediana.

*   **Mestrado (Roxo):**
    *   Este grupo apresenta uma das **medianas salariais mais altas**, em torno de R$ 11.000 - R$ 13.000.
    *   A maior parte da densidade salarial está concentrada em uma faixa mais elevada em comparação com "Graduação/Bacharelado" e "Pós-graduação". A cauda superior também é proeminente, indicando potencial para altos salários.

*   **Doutorado ou Phd (Azul):**
    *   A mediana salarial é comparável à de "Mestrado" ou ligeiramente inferior, em torno de R$ 10.000 - R$ 12.000.
    *   A distribuição é bastante dispersa, com o corpo do violino sendo largo, indicando maior variabilidade nos salários para este grupo. A cauda superior é extensa, mostrando que profissionais com doutorado também podem alcançar os salários mais altos do dataset.

**Conclusões Gerais do Gráfico:**
*   Há uma tendência geral de **aumento da mediana salarial com o avanço no nível de ensino**, sendo mais notável a diferença entre "Estudante de Graduação" e os demais níveis.
*   Profissionais com **Mestrado** e **Doutorado/PhD** tendem a ter as medianas salariais mais elevadas, embora a diferença entre eles e "Pós-graduação" (lato sensu, especializações) possa não ser tão acentuada em termos de mediana, mas sim na forma da distribuição e potencial para salários muito altos.
*   Todos os níveis de ensino, a partir da graduação, mostram uma **assimetria à direita** (cauda longa para salários altos), indicando que em todos os níveis há profissionais que conseguem remunerações significativamente acima da média do seu grupo.
*   A **variabilidade salarial** (largura do violino e comprimento das caudas) também é considerável em todos os níveis, especialmente para aqueles com formação superior completa em diante.

## Grafico Interação entre Escolaridade, Experiência e Salário
### [Grafico Interativo - Clique aqui](https://htmlpreview.github.io/?https://gist.githubusercontent.com/pedrinndias/99901a7169839052f5473ff6f4b57242/raw/6c71c7167850cb50f4e98432a646db7c69f2ffa1/grafico_3d_interativo.html)

![newplot](https://github.com/user-attachments/assets/5bb94b6a-aa5d-416d-be48-9bac9d9d01c0)
## Explicação do Gráfico 3D Interativo: Interação entre Escolaridade, Experiência e Salário

O gráfico apresentado é uma visualização 3D interativa que tem como objetivo investigar a interação entre o nível de escolaridade, o tempo de experiência e o salário dos profissionais de dados no Brasil. Gráficos de superfície ou dispersão 3D são úteis para investigar como uma variável de resposta (neste caso, o salário) se relaciona com duas variáveis preditoras (escolaridade e experiência).

**Eixos do Gráfico:**
*   **Eixo X (Horizontal, profundidade):** "Tempo de Experiência (anos)" – Representa os anos de experiência profissional na área de dados. A escala parece variar de 0 a aproximadamente 10 anos.
*   **Eixo Y (Horizontal, largura):** "Nível de Escolaridade (numérico)" – Representa o nível de escolaridade, que foi convertido para uma escala numérica para permitir a plotagem. A legenda indica a correspondência:
    *   0: Doutorado ou PhD
    *   1: Estudante de Graduação
    *   2: Graduação/Bacharelado
    *   3: Mestrado
    *   4: Pós-graduação
*   **Eixo Z (Vertical):** "Salário (R$)" – Representa a remuneração mensal em Reais. A escala vai de R$0 até valores superiores a R$35.000.

**Interpretação dos Dados e Visualização:**
*   **Pontos de Dados (Scatter Plot 3D):** Cada ponto no gráfico representa um profissional de dados, posicionado de acordo com seu tempo de experiência, nível de escolaridade (numérico) e salário.
*   **Cores por Nível de Escolaridade:** Os pontos são coloridos de acordo com o nível de escolaridade, facilitando a distinção e a análise de como cada grupo educacional se distribui em relação à experiência e ao salário.
    *   **Doutorado ou PhD (Azul Escuro/Roxo):** Pontos para este grupo.
    *   **Estudante de Graduação (Azul Claro/Ciano):** Pontos para este grupo.
    *   **Graduação/Bacharelado (Verde):** Pontos para este grupo.
    *   **Mestrado (Laranja/Amarelo):** Pontos para este grupo.
    *   **Pós-graduação (Vermelho):** Pontos para este grupo.
*   **Interatividade:** A natureza interativa do gráfico permite ao usuário girar a visualização, alterar o ângulo de visão e dar zoom. Isso é crucial para explorar as relações complexas em um espaço tridimensional, identificando padrões, concentrações de pontos e outliers que poderiam não ser evidentes em gráficos 2D.

**Observações Gerais e Tendências (Inferidas pela Exploração Visual):**
*   **Impacto da Experiência:** Geralmente, observa-se que, para todos os níveis de escolaridade, um aumento no tempo de experiência (movimento ao longo do eixo X) tende a estar associado a salários mais altos (pontos mais elevados no eixo Z).
*   **Impacto da Escolaridade:**
    *   **Estudantes de Graduação (cor Azul Claro/Ciano):** Tendem a se concentrar na parte inferior da escala salarial e com menor tempo de experiência.
    *   **Graduação/Bacharelado (cor Verde) e Pós-graduação (cor Vermelho):** Mostram uma dispersão maior, com salários aumentando com a experiência. Muitos pontos se situam em faixas salariais intermediárias, mas com potencial de alcançar salários mais altos com mais experiência.
    *   **Mestrado (cor Laranja/Amarelo) e Doutorado/PhD (cor Azul Escuro/Roxo):** Estes grupos tendem a ter pontos que alcançam os níveis salariais mais altos, especialmente quando combinados com maior tempo de experiência. Pode-se observar se há uma "elevação" geral dos pontos dessas cores no eixo Z.
*   **Interação entre Escolaridade e Experiência:** O objetivo principal deste gráfico é visualizar como a combinação específica de um nível de escolaridade e anos de experiência influencia o salário. Por exemplo, pode-se tentar observar se o "retorno" (aumento salarial) por ano adicional de experiência é diferente para quem tem um Mestrado em comparação com quem tem apenas Graduação. A densidade de pontos em certas regiões do gráfico (por exemplo, alta experiência e alto nível de escolaridade resultando em altos salários) pode indicar essas interações. Picos e vales na distribuição dos pontos podem corresponder a combinações que produzem valores máximos ou mínimos de salário.

**Como Explorar o Gráfico Interativo:**
*   **Girar:** Clique e arraste para mudar o ponto de vista e observar a nuvem de pontos de diferentes ângulos. Isso ajuda a entender a profundidade e a sobreposição dos dados.
*   **Zoom:** Use o scroll do mouse para aproximar ou afastar, permitindo focar em áreas específicas de interesse (por exemplo, a distribuição salarial para um nível de escolaridade específico com muitos anos de experiência).
*   **Observar Agrupamentos:** Procure por concentrações de pontos de uma mesma cor em determinadas regiões do espaço 3D.

Este tipo de gráfico é uma ferramenta poderosa na análise exploratória de dados (EDA) para identificar relações multivariadas e gerar hipóteses sobre as interações entre diferentes fatores.

## Grafico Mapa de Calor de Correlações
![__results___0_5](https://github.com/user-attachments/assets/5cf1cb29-6d4c-46dc-bc80-b9b32d679b12)
## Explicação do Gráfico: Mapa de Calor de Correlações

O gráfico apresentado é um **Mapa de Calor de Correlações** (heatmap) que visualiza a força e a direção das relações lineares entre três variáveis numéricas: "Faixa\_salarial\_num", "Oportunidade de aprendizado" e "Reputação da empresa".

**Como ler este Mapa de Calor:**
*   **Variáveis:** As variáveis analisadas estão listadas tanto nas linhas (eixo Y) quanto nas colunas (eixo X) da matriz.
*   **Células Coloridas:** Cada célula na interseção de duas variáveis mostra o coeficiente de correlação entre elas. A cor da célula representa visualmente esse coeficiente.
*   **Barra de Cores (Escala):** Localizada à direita do gráfico, a barra de cores indica como os valores de correlação mapeiam para as cores. Nesta visualização:
    *   Cores quentes (como vermelho intenso) indicam correlações positivas fortes, aproximando-se de +1.0.
    *   Cores frias (como azul intenso/roxo) indicam correlações negativas fortes (aproximando-se de -1.0) ou, como neste caso, correlações muito fracas ou próximas de zero.
    *   Cores neutras ou claras no meio da escala (se presentes) indicariam correlações próximas de 0. A escala no gráfico vai de 0.0 (azul escuro) a 1.0 (vermelho escuro).
*   **Valores Numéricos:** Dentro de cada célula, o valor numérico exato do coeficiente de correlação é exibido. Estes coeficientes variam de -1 (correlação negativa perfeita) a +1 (correlação positiva perfeita), com 0 indicando ausência de correlação linear.

**Interpretação das Correlações Exibidas:**

1.  **Diagonal Principal (de cima para baixo, da esquerda para a direita):**
    *   As células na diagonal principal mostram a correlação de cada variável consigo mesma. Esses valores são sempre **1.00** (vermelho intenso), indicando uma correlação positiva perfeita, o que é esperado.
        *   Faixa\_salarial\_num com Faixa\_salarial\_num: 1.00
        *   Oportunidade de aprendizado com Oportunidade de aprendizado: 1.00
        *   Reputação da empresa com Reputação da empresa: 1.00

2.  **Correlações entre Variáveis Distintas:**
    *   **Faixa\_salarial\_num e Oportunidade de aprendizado:**
        *   Coeficiente: **-0.04**.
        *   Cor: Azul escuro.
        *   Interpretação: Existe uma correlação linear negativa muito fraca, praticamente inexistente, entre a faixa salarial e a oportunidade de aprendizado. Um valor tão próximo de zero sugere que não há uma tendência clara de aumento ou diminuição salarial associada diretamente a maiores ou menores oportunidades de aprendizado, conforme os dados analisados.

    *   **Faixa\_salarial\_num e Reputação da empresa:**
        *   Coeficiente: **0.00**.
        *   Cor: Azul escuro.
        *   Interpretação: Não há correlação linear entre a faixa salarial e a reputação da empresa. Isso indica que, neste conjunto de dados, a reputação da empresa não está linearmente associada a salários mais altos ou mais baixos.

    *   **Oportunidade de aprendizado e Reputação da empresa:**
        *   Coeficiente: **-0.05**.
        *   Cor: Azul escuro.
        *   Interpretação: Há uma correlação linear negativa muito fraca, quase nula, entre a oportunidade de aprendizado e a reputação da empresa. Isso sugere que não há uma relação linear significativa onde empresas com melhor reputação ofereçam consistentemente mais (ou menos) oportunidades de aprendizado, ou vice-versa, de acordo com os dados.

**Conclusão Geral do Mapa de Calor:**
Este mapa de calor indica que as três variáveis analisadas ("Faixa\_salarial\_num", "Oportunidade de aprendizado" e "Reputação da empresa") não possuem correlações lineares fortes entre si no contexto dos dados utilizados para esta análise. Todos os coeficientes de correlação entre pares de variáveis distintas são muito próximos de zero, sugerindo que essas variáveis são, em grande medida, linearmente independentes umas das outras. É importante notar que a correlação mede apenas relações lineares; podem existir relações não lineares que não seriam capturadas por este tipo de análise.

## Grafico Distribuição por Gênero e Raça-Etnia
![__results___0_6](https://github.com/user-attachments/assets/46d749b3-6293-46b5-bca7-021d3843a544)
## Explicação dos Gráficos: Distribuição por Gênero e Raça/Etnia

A imagem anexa exibe dois gráficos de barras que ilustram a distribuição demográfica dos profissionais no conjunto de dados analisado, um por gênero e outro por raça/etnia.

### Gráfico 1: Distribuição por Gênero

*   **Título:** "Distribuição por Gênero"
*   **Tipo de Gráfico:** Gráfico de barras verticais.
*   **Eixo Y (Vertical):** "count" (Contagem) – Indica o número de profissionais. A escala vai de 0 a 2500.
*   **Eixo X (Horizontal):** "Gênero do profissional" – Apresenta as categorias de gênero.
*   **Observações:**
    *   **Masculino:** É a categoria predominante, com uma contagem de aproximadamente 2500 profissionais. Esta é a barra mais alta no gráfico.
    *   **Feminino:** A segunda maior categoria, com uma contagem significativamente menor, em torno de 800 profissionais.
    *   **Outro:** Representa uma contagem muito pequena, quase insignificante visualmente no gráfico.
    *   **Prefiro não informar:** Também representa uma contagem muito pequena, similar à categoria "Outro".
*   **Conclusão:** O gráfico demonstra uma expressiva maioria de profissionais do gênero masculino no conjunto de dados analisado.

### Gráfico 2: Distribuição por Raça/Etnia

*   **Título:** "Distribuição por Raça/Etnia"
*   **Tipo de Gráfico:** Gráfico de barras verticais.
*   **Eixo Y (Vertical):** "count" (Contagem) – Indica o número de profissionais. A escala vai de 0 a mais de 2000.
*   **Eixo X (Horizontal):** "Cor/Raça/Etnia" – Apresenta as categorias de raça ou etnia.
*   **Observações:**
    *   **Branca:** É a categoria com a maior contagem, superando 2000 profissionais. Esta é a barra mais alta.
    *   **Parda:** A segunda categoria mais representada, com uma contagem de aproximadamente 800 profissionais.
    *   **Preta:** Apresenta uma contagem de cerca de 250 profissionais.
    *   **Amarela:** Possui uma contagem menor, em torno de 100 profissionais.
    *   **Prefiro não informar:** Representa uma contagem muito pequena, inferior a 50 profissionais.
    *   **Outra:** Contagem visualmente insignificante.
    *   **Indígena:** Contagem visualmente insignificante.
*   **Conclusão:** O gráfico indica que a maioria dos profissionais no conjunto de dados se identifica como Branca, seguida pela categoria Parda. Outras categorias raciais/étnicas têm representação consideravelmente menor.

**Resumo Geral:**
Ambos os gráficos mostram desequilíbrios significativos nas distribuições. Há uma predominância de profissionais do gênero masculino e de profissionais que se identificam como da cor/raça Branca no dataset utilizado para a análise exploratória de dados.

## Grafico Distribuição Geográfica dos Profissionais
![__results___0_8](https://github.com/user-attachments/assets/b1f41cbe-9705-44ac-8b50-9407b5b07dd2)
## Explicação do Gráfico: Distribuição Geográfica dos Profissionais

O gráfico de barras verticais intitulado "Distribuição Geográfica dos Profissionais" ilustra a contagem de profissionais de dados distribuídos pelos diferentes estados (Unidades Federativas - UF) do Brasil, conforme o conjunto de dados analisado.

**Eixos do Gráfico:**
*   **Eixo Y (Vertical):** "Contagem" – Representa o número de profissionais em cada estado. A escala varia de 0 a mais de 1200.
*   **Eixo X (Horizontal):** "Estado (UF)" – Apresenta as siglas dos estados brasileiros.

**Interpretação da Distribuição Geográfica:**

*   **Concentração em São Paulo (SP):** O estado de São Paulo (SP) destaca-se com a maior concentração de profissionais, com uma contagem que ultrapassa 1200. Esta é, de longe, a barra mais alta no gráfico, indicando que uma parcela muito significativa dos profissionais no dataset está localizada em SP.
*   **Estados com Representação Significativa:** Após São Paulo, alguns outros estados apresentam contagens notáveis, embora consideravelmente menores:
    *   **Minas Gerais (MG):** É o segundo estado com maior número de profissionais, com uma contagem próxima de 400 (especificamente, cerca de 380).
    *   **Paraná (PR):** Apresenta uma contagem um pouco acima de 300 profissionais.
    *   **Rio de Janeiro (RJ):** Também com uma contagem em torno de 300 profissionais.
    *   **Rio Grande do Sul (RS):** Possui cerca de 200 profissionais.
    *   **Santa Catarina (SC):** Apresenta uma contagem um pouco abaixo de 200, em torno de 180 profissionais.
*   **Demais Estados:**
    *   **Distrito Federal (DF), Bahia (BA), Ceará (CE), Pernambuco (PE), Espírito Santo (ES), Goiás (GO), Paraíba (PB):** Estes estados formam um grupo com contagens menores, variando aproximadamente entre 50 e 100 profissionais cada.
    *   **Outros Estados (MT, RN, AM, PA, SE, AL, MS, MA, PI, RO, AP, TO):** A grande maioria dos demais estados brasileiros apresenta contagens muito baixas, com barras quase insignificantes em comparação com os estados mais populosos em termos de profissionais de dados. Muitos desses estados têm menos de 50 profissionais representados no dataset.

**Conclusão Geral do Gráfico:**
O gráfico evidencia uma forte concentração geográfica dos profissionais de dados no Brasil, com o estado de São Paulo dominando expressivamente. A região Sudeste (com SP, MG, RJ, ES) e a região Sul (com PR, RS, SC) concentram a maior parte desses profissionais. As demais regiões e estados possuem uma representação significativamente menor no conjunto de dados analisado.

## Grafico Salário por Nível de Senioridade
![__results___0_9](https://github.com/user-attachments/assets/4cb778a5-1f36-40a9-b815-b0e97c02d2c8)
## Explicação do Gráfico: Salário por Nível de Senioridade

O gráfico de boxplot intitulado "Salário por Nível de Senioridade" ilustra a distribuição da faixa salarial numérica ("Faixa\_salarial\_num") entre diferentes níveis de senioridade profissional: Júnior, Pleno e Sênior.

**Como ler este gráfico de Boxplot:**
*   **Caixa (Box):** Representa o intervalo interquartil (IQR), onde se concentram 50% dos salários. A linha inferior da caixa é o primeiro quartil (Q1 - 25º percentil), e a linha superior é o terceiro quartil (Q3 - 75º percentil).
*   **Linha dentro da Caixa:** Indica a mediana (Q2 - 50º percentil), que é o valor salarial central para cada nível de senioridade.
*   **Hastess/"Bigodes" (Whiskers):** As linhas que se estendem a partir da caixa mostram o alcance dos dados, geralmente até 1,5 vezes o IQR. Pontos além dessas hastes são considerados outliers.
*   **Outliers:** São pontos individuais (representados por losangos no gráfico) que indicam salários atípicos, significativamente mais altos ou mais baixos do que a maioria dos salários para aquele nível de senioridade.
*   **Eixo Y (Vertical):** "Faixa\_salarial\_num" representa os salários em Reais (R$), com a escala variando de R$0 a R$40.000.
*   **Eixo X (Horizontal):** "Nível de senioridade" categoriza os profissionais em "Júnior", "Pleno" e "Sênior".

**Interpretação das Distribuições Salariais por Nível de Senioridade:**

*   **Júnior (Caixa Verde):**
    *   **Mediana Salarial:** É a mais baixa entre os três níveis, situando-se em torno de R$3.500 - R$4.000.
    *   **Intervalo Interquartil (IQR):** A maioria dos salários (50% centrais) está concentrada entre aproximadamente R$2.500 e R$5.000.
    *   **Dispersão e Outliers:** A faixa salarial típica (incluindo os "bigodes") vai de perto de R$0 até cerca de R$7.000. Observam-se alguns outliers com salários mais altos, chegando até aproximadamente R$18.000.

*   **Pleno (Caixa Laranja):**
    *   **Mediana Salarial:** Apresenta um aumento significativo em relação ao nível Júnior, localizando-se em torno de R$7.000.
    *   **Intervalo Interquartil (IQR):** Os 50% centrais dos salários estão entre aproximadamente R$5.000 e R$10.000.
    *   **Dispersão e Outliers:** A faixa salarial típica se estende de cerca de R$1.000 até aproximadamente R$14.000. Este nível possui vários outliers com salários mais elevados, incluindo valores próximos a R$18.000, R$22.500 e até um ponto próximo a R$40.000.

*   **Sênior (Caixa Azul):**
    *   **Mediana Salarial:** É a mais alta dos três níveis, posicionando-se em torno de R$11.500 - R$12.000.
    *   **Intervalo Interquartil (IQR):** A maior parte dos salários (50% centrais) varia entre R$10.000 e R$14.000.
    *   **Dispersão e Outliers:** A faixa salarial típica vai de aproximadamente R$5.000 até cerca de R$18.500. Assim como o nível Pleno, o nível Sênior também apresenta outliers com salários significativamente altos, com pontos próximos a R$22.500 e um próximo a R$40.000. Existem também alguns outliers inferiores, indicando salários mais baixos que o usual para esta senioridade.

**Conclusões Gerais do Gráfico:**
*   **Progressão Salarial Clara:** O gráfico demonstra uma clara progressão salarial à medida que o nível de senioridade aumenta. Profissionais Sênior têm a maior mediana salarial, seguidos por Pleno e depois Júnior.
*   **Aumento da Dispersão:** A variabilidade salarial (altura da caixa e extensão dos "bigodes") tende a aumentar com a senioridade, indicando uma gama mais ampla de salários pagos nos níveis Pleno e Sênior em comparação com o Júnior.
*   **Potencial de Altos Salários:** Embora os outliers existam em todos os níveis, eles atingem valores mais altos e são mais frequentes nos níveis Pleno e Sênior, sugerindo que profissionais com maior senioridade têm maior potencial para alcançar remunerações excepcionalmente elevadas.

Em resumo, o nível de senioridade é um fator importante na determinação da faixa salarial, com um aumento consistente na remuneração e na variabilidade salarial à medida que os profissionais progridem de Júnior para Pleno e Sênior.

## Grafico Análise Multivariada das Relações entre Variáveis Selecionadas
![__results___0_11](https://github.com/user-attachments/assets/f8a270d1-8bb7-4612-9c54-0c083f46936a)
## Explicação do Gráfico: Análise Multivariada das Relações entre Variáveis Selecionadas (Pair Plot)

O gráfico apresentado é uma **matriz de gráficos de dispersão (pair plot)**, intitulada "Análise Multivariada das Relações entre Variáveis Selecionadas". Este tipo de visualização é utilizado para mostrar as relações entre pares de múltiplas variáveis simultaneamente, bem como a distribuição individual de cada variável.

As variáveis analisadas são:
*   "Faixa\_salarial\_num" (Salário)
*   "Oportunidade de aprendizado"
*   "Reputação da empresa"

**Estrutura do Gráfico:**

*   **Diagonal Principal:** Os gráficos ao longo da diagonal (do canto superior esquerdo ao canto inferior direito) mostram a **distribuição de cada variável individualmente**, geralmente através de um histograma ou, como neste caso, uma estimativa de densidade do kernel (KDE).
*   **Fora da Diagonal:** Os gráficos fora da diagonal são **gráficos de dispersão (scatter plots)** que mostram a relação entre duas variáveis diferentes. Cada gráfico de dispersão (i,j) mostra a variável do eixo i contra a variável do eixo j.

**Interpretação dos Gráficos Individuais:**

1.  **Distribuições Individuais (Diagonal):**
    *   **Faixa\_salarial\_num (Topo Esquerdo):** A distribuição dos salários é multimodal (apresenta múltiplos picos) e assimétrica à direita. Há uma concentração maior em salários mais baixos (em torno de R$5.000-R$10.000), com picos menores em salários mais altos e uma cauda que se estende até R$40.000.
    *   **Oportunidade de aprendizado (Meio):** Esta variável parece ser binária ou categórica, com a grande maioria dos dados concentrada em dois valores principais (provavelmente 0 e 1, representando, por exemplo, baixa/alta oportunidade ou sim/não). Há um pico maior em um dos valores e um pico menor no outro.
    *   **Reputação da empresa (Inferior Direito):** Similar à "Oportunidade de aprendizado", esta variável também parece ser binária ou categórica, com a maioria dos dados concentrados em dois valores principais. Um dos valores tem uma densidade muito maior que o outro.

2.  **Relações entre Pares de Variáveis (Fora da Diagonal):**

    *   **Oportunidade de aprendizado vs. Faixa\_salarial\_num (Linha 1, Coluna 2 e Linha 2, Coluna 1):**
        *   Os pontos estão concentrados em duas faixas horizontais (ou verticais, dependendo da orientação do par), correspondentes aos dois principais valores da variável "Oportunidade de aprendizado".
        *   Visualmente, não há uma tendência clara (ascendente ou descendente) que sugira uma forte correlação linear entre salário e oportunidade de aprendizado. Os salários parecem variar amplamente para ambos os níveis de oportunidade de aprendizado.

    *   **Reputação da empresa vs. Faixa\_salarial\_num (Linha 1, Coluna 3 e Linha 3, Coluna 1):**
        *   Similar ao par anterior, os pontos se agrupam em duas faixas horizontais (ou verticais) correspondentes aos valores da "Reputação da empresa".
        *   Não se observa uma relação linear forte. Os salários variam amplamente independentemente do nível de reputação da empresa exibido.

    *   **Reputação da empresa vs. Oportunidade de aprendizado (Linha 2, Coluna 3 e Linha 3, Coluna 2):**
        *   Este gráfico mostra como os dois valores de "Oportunidade de aprendizado" se distribuem em relação aos dois valores de "Reputação da empresa". Os pontos se agrupam nos quatro cantos possíveis (0,0; 0,1; 1,0; 1,1), se as variáveis forem binárias 0/1. A densidade de pontos em cada um desses "cantos" indicaria a frequência dessas combinações.
        *   Visualmente, parece não haver um padrão forte de associação. Por exemplo, não parece que empresas com alta reputação consistentemente oferecem alta oportunidade de aprendizado, ou vice-versa.

**Conclusão Geral do Gráfico:**
O pair plot reforça visualmente a ausência de correlações lineares fortes entre "Faixa\_salarial\_num", "Oportunidade de aprendizado" e "Reputação da empresa", o que já havia sido sugerido pelo mapa de calor de correlações anteriormente. As variáveis "Oportunidade de aprendizado" e "Reputação da empresa" apresentam distribuições que sugerem natureza binária ou categórica com poucos níveis. As relações entre os pares de variáveis não exibem padrões lineares claros, indicando que esses fatores, isoladamente ou em pares diretos, não explicam de forma linear e significativa a variação salarial ou uns aos outros neste conjunto de dados.

## Grafico Sunburst da Distribuição de Profissionais de Dados
### [Grafico Interativo - Clique aqui](https://htmlpreview.github.io/?https://gist.githubusercontent.com/pedrinndias/11ec6c319fd644ad08f61cff87cc702c/raw/392be6308934280602be52c7a1ec9cab21e1ad03/sunburst_chart.html)
![newplot (1)](https://github.com/user-attachments/assets/fc4076b1-1a10-48d1-89b2-3f76a107321b)

## Explicação do Gráfico Interativo: Sunburst da Distribuição de Profissionais de Dados

O gráfico apresentado é um **gráfico de explosão solar (sunburst chart)** interativo. Este tipo de visualização é ideal para exibir dados hierárquicos, mostrando como um grupo principal se divide em subgrupos e assim por diante, em uma série de anéis concêntricos.

**Como Ler Este Gráfico Sunburst:**

*   **Círculos Concêntricos (Anéis):** Cada anel representa um nível na hierarquia dos dados.
    *   **Centro do Gráfico:** O círculo mais interno representa o topo da hierarquia, neste caso, o total de "Profissionais de Dados" no dataset analisado.
    *   **Anéis Subsequentes:** Cada anel externo subdivide as categorias do anel interno adjacente.
*   **Segmentos (Fatias):** Cada anel é dividido em segmentos. O tamanho (ângulo ou área) de cada segmento é proporcional à sua participação ou contagem dentro da categoria pai no anel interno.
*   **Cores:** Cores diferentes são usadas para distinguir as categorias em cada nível, ajudando na visualização das proporções e relações.
*   **Interatividade:**
    *   **Hover (Passar o Mouse):** Ao passar o mouse sobre um segmento, ele é destacado, e geralmente uma dica de ferramenta (tooltip) exibe informações detalhadas, como o caminho hierárquico completo e o valor (contagem de profissionais) para aquele segmento específico.
    *   **Clique:** Clicar em um segmento geralmente "foca" ou "dá zoom" naquela categoria, tornando-a o novo centro do gráfico e exibindo suas subdivisões com mais detalhes. Clicar no centro do gráfico retorna ao nível hierárquico anterior.

**Hierarquia e Interpretação dos Dados Neste Gráfico Específico:**

Observando o gráfico interativo:

1.  **Nível Central (Raiz):**
    *   Representa o total de "Profissionais de Dados" considerados na análise.

2.  **Primeiro Anel (Nível de Escolaridade):**
    *   Subdivide os profissionais de dados pelo "Nível de Escolaridade".
    *   As categorias visíveis são: "Graduação/Bacharelado", "Pós-graduação", "Mestrado", "Estudante de Graduação" e "Doutorado ou PhD".
    *   O tamanho de cada segmento neste anel indica a proporção de profissionais com aquele nível de escolaridade. Por exemplo, "Graduação/Bacharelado" parece ser a maior fatia, indicando o nível de escolaridade mais comum.

3.  **Segundo Anel (Tempo de Experiência):**
    *   Subdivide cada categoria de "Nível de Escolaridade" pelo "Tempo de experiência na área de dados".
    *   As faixas de experiência incluem: "de 1 a 2 anos", "de 3 a 4 anos", "Menos de 1 ano", "de 4 a 6 anos", "de 7 a 10 anos" e "de 5 a 6 anos".
    *   O tamanho de um segmento neste anel mostra, por exemplo, quantos profissionais com "Graduação/Bacharelado" têm "de 1 a 2 anos" de experiência.

4.  **Terceiro Anel (Faixa Salarial Média):**
    *   Subdivide cada combinação de "Nível de Escolaridade" e "Tempo de Experiência" pela "Faixa Salarial Média (R$)".
    *   As faixas salariais incluem: "0-5000", "5001-10000", "10001-15000", "15001-20000", etc.
    *   O tamanho de um segmento neste anel mais externo indica, por exemplo, quantos profissionais com "Graduação/Bacharelado" e "de 1 a 2 anos" de experiência se enquadram na faixa salarial de "5001-10000". Os números dentro dos segmentos representam a contagem de profissionais.

**Como Extrair Insights:**

*   **Proporções Dominantes:** Identifique rapidamente os níveis de escolaridade mais comuns, as faixas de experiência predominantes dentro de cada nível de escolaridade e as faixas salariais mais frequentes para cada combinação de escolaridade e experiência.
*   **Relações Hierárquicas:** Entenda como os grupos se subdividem. Por exemplo, pode-se explorar se profissionais com "Mestrado" e "de 7 a 10 anos" de experiência tendem a se concentrar em faixas salariais mais altas em comparação com aqueles com "Graduação/Bacharelado" e a mesma experiência.
*   **Exploração Interativa:** Use o clique para focar em segmentos de interesse. Por exemplo, clicando em "Mestrado", o gráfico se reorganizará para mostrar apenas as subdivisões de experiência e salário para mestres, permitindo uma análise mais detalhada desse subgrupo específico.

Este gráfico sunburst oferece uma visão rica e interativa da composição da força de trabalho de profissionais de dados no Brasil, de acordo com o dataset, permitindo a exploração de como a escolaridade, a experiência e os salários se inter-relacionam em diferentes níveis.

---

## Analise exploratoria de dados base de dados Microdados

---

## Grafico Distribuição Nacional de Níveis de Formação dos Docentes
![01_distribuicao_formacao_nacional](https://github.com/user-attachments/assets/0052b7ec-4124-4e90-a500-8abd26d0ccc8)
## Explicação do Gráfico: Distribuição Nacional de Níveis de Formação dos Docentes

O gráfico de pizza ilustra a proporção dos docentes em nível nacional, classificados de acordo com seu nível de formação acadêmica. Os dados são provenientes do arquivo `microdados_agrupados_por_uf.csv`.

**Principais observações do gráfico:**

*   **Docentes com Doutorado:** Este grupo constitui a maior fatia, representando **52,3%** do total de docentes analisados. Isso indica que mais da metade dos docentes possui o título acadêmico mais elevado.
*   **Docentes com Mestrado:** Correspondem a **33,3%** do corpo docente. Somados aos doutores, os docentes com pós-graduação *stricto sensu* (mestrado ou doutorado) são a grande maioria.
*   **Docentes com Especialização:** Representam **13,9%** dos docentes. Este grupo possui pós-graduação *lato sensu*.
*   **Docentes com Graduação:** Apenas **0,6%** dos docentes possuem somente a graduação como nível de formação mais alto. Este é o menor grupo, sugerindo que a progressão para níveis de pós-graduação é comum na carreira docente.

**Contextualização para a Análise Exploratória de Dados:**

Este gráfico de pizza fornece uma visão geral do perfil educacional dos docentes no Brasil, com base nos dados disponíveis. Ele demonstra uma alta qualificação acadêmica, com a maioria possuindo títulos de mestre ou doutor.

Para a pergunta de pesquisa original sobre "como fatores como formação acadêmica e experiência profissional interagem para influenciar a disparidade salarial entre profissionais de dados no Brasil", este gráfico oferece um panorama da variável "formação acadêmica" para o grupo de "docentes". No entanto, conforme discutido anteriormente, para analisar a disparidade salarial, seriam necessários dados de remuneração e uma clara identificação de "profissionais de dados", que não estão presentes no dataset atual.

A predominância de altos níveis de escolaridade é um fator importante, mas sua interação com a experiência profissional e o impacto na disparidade salarial demandariam um conjunto de dados mais completo.


## Grafico Top 10 Estados por Nível de Formação de Docentes
![02_top10_estados_formacao](https://github.com/user-attachments/assets/4513d6de-20bd-4e5b-9b93-1cd10b819ad5)
## Explicação do Gráfico: Top 10 Estados por Nível de Formação de Docentes

O gráfico de barras empilhadas ilustra o número total de docentes nos 10 estados com maior contingente, detalhando a distribuição desses profissionais conforme seu nível de formação acadêmica. O eixo vertical ("Número de Docentes") quantifica o total de docentes, enquanto o eixo horizontal ("Estado") lista as siglas dos respectivos estados. Cada barra é segmentada por cores que representam os diferentes níveis de formação:

*   **Rosa:** Docentes com Graduação
*   **Dourado/Marrom:** Docentes com Especialização
*   **Verde:** Docentes com Mestrado
*   **Azul-petróleo (Teal):** Docentes com Doutorado

**Principais observações do gráfico:**

*   **Liderança de São Paulo (SP):** O estado de São Paulo (SP) destaca-se com o maior número absoluto de docentes, ultrapassando 70.000 profissionais. Dentro deste total, a maior parcela é composta por docentes com doutorado, seguida por mestrado e especialização.
*   **Minas Gerais (MG) e Rio de Janeiro (RJ):** Minas Gerais (MG) ocupa a segunda posição, com aproximadamente 40.000 docentes, seguido pelo Rio de Janeiro (RJ), com pouco mais de 30.000. Ambos os estados também apresentam uma predominância de docentes com doutorado e mestrado.
*   **Demais Estados no Top 10:** Os estados do Paraná (PR), Rio Grande do Sul (RS), Bahia (BA), Santa Catarina (SC), Pernambuco (PE), Ceará (CE) e Goiás (GO) completam o ranking dos 10 estados com mais docentes. Em todos eles, a tendência de maior concentração nos níveis de doutorado e mestrado se mantém, embora em menor escala absoluta comparado a SP, MG e RJ.
*   **Proporção dos Níveis de Formação:** Em todos os estados visualizados, a formação de doutorado (azul-petróleo) representa a maior ou uma das maiores parcelas do total de docentes. Em seguida, geralmente aparecem os docentes com mestrado (verde). Docentes com apenas especialização (dourado/marrom) formam um grupo menor, e aqueles com apenas graduação (rosa) são a menor fração, quase imperceptível em alguns estados, indicando um alto nível de qualificação formal do corpo docente nesses estados.

**Contextualização para a Análise Exploratória de Dados:**

Este gráfico permite uma comparação visual da quantidade e do perfil de formação dos docentes entre os principais estados brasileiros. Ele reforça a observação de que o corpo docente, especialmente nos estados com maior número de profissionais, possui elevada qualificação acadêmica, com forte presença de doutores e mestres.

Para a pergunta de pesquisa sobre a influência da formação acadêmica e experiência profissional na disparidade salarial entre profissionais de dados, este gráfico detalha a variável "formação acadêmica" em um nível geográfico (estadual) para "docentes". A análise da disparidade salarial, contudo, ainda dependeria da inclusão de dados de remuneração e da identificação específica de "profissionais de dados" dentro desse universo de docentes ou em um dataset complementar. Observar onde se concentram os docentes mais qualificados pode ser um ponto de partida para investigar se há correlação com polos de desenvolvimento em ciência de dados, mas a relação direta com salários não pode ser inferida apenas com este gráfico.

## Grafico Distribuição Etária Nacional dos Docentes
![03_distribuicao_etaria_nacional](https://github.com/user-attachments/assets/38b315e0-7eb6-4c40-820f-3b0281b1b1d8)
## Explicação do Gráfico: Distribuição Etária Nacional dos Docentes

O gráfico de barras verticais, intitulado "Distribuição Etária Nacional dos Docentes", exibe a quantidade de docentes em nível nacional, agrupados por diferentes faixas etárias. O eixo vertical ("Quantidade") indica o número de docentes, enquanto o eixo horizontal ("Faixa Etária") categoriza os docentes em grupos de idade.

**Principais observações do gráfico:**

*   **Pico na Faixa de 40-44 anos:** A faixa etária com o maior número de docentes é a de "Docentes\_Idade\_40\_44", com quase 70.000 profissionais. Isso sugere que o maior contingente de docentes se encontra nessa fase da carreira.
*   **Concentração entre 35 e 49 anos:** As faixas etárias "Docentes\_Idade\_35\_39" (pouco mais de 60.000 docentes) e "Docentes\_Idade\_45\_49" (pouco menos de 60.000 docentes) também apresentam um número elevado de profissionais, indicando que uma parcela significativa do corpo docente nacional está entre 35 e 49 anos.
*   **Presença Significativa em Faixas Mais Elevadas:** A faixa "Docentes\_Idade\_60\_mais" também mostra um número considerável de docentes, com mais de 45.000 profissionais. Isso indica uma retenção de docentes mais experientes no sistema ou um envelhecimento da força de trabalho docente.
*   **Menor Quantidade nas Faixas Mais Jovens e Intermediárias Superiores:** As faixas "Docentes\_Idade\_30\_34" (pouco menos de 40.000), "Docentes\_Idade\_50\_54" (aproximadamente 45.000) e "Docentes\_Idade\_55\_59" (pouco menos de 40.000) apresentam quantidades menores em comparação com o pico, mas ainda representam um número substancial de docentes. A distribuição geral se assemelha a uma curva que atinge seu pico na faixa dos 40-44 anos e depois declina gradualmente, com uma leve recuperação na faixa de 60 anos ou mais.

**Contextualização para a Análise Exploratória de Dados:**

Este gráfico fornece um panorama da distribuição etária dos docentes no Brasil. No contexto da pergunta de pesquisa sobre "como fatores como formação acadêmica e experiência profissional interagem para influenciar a disparidade salarial entre profissionais de dados no Brasil", a idade pode ser utilizada como um *proxy* (uma aproximação) para a experiência profissional. Geralmente, espera-se que profissionais mais velhos tenham acumulado mais anos de experiência.

A concentração de docentes em faixas etárias mais maduras (40-49 anos) e a presença significativa de docentes com 60 anos ou mais podem indicar um corpo docente experiente. Para analisar a disparidade salarial, seria necessário cruzar esses dados etários (como proxy de experiência) com informações sobre a formação acadêmica (analisada em gráficos anteriores) e, crucialmente, com dados de remuneração específicos para "profissionais de dados", os quais não estão presentes no dataset atual. Este gráfico ajuda a caracterizar uma dimensão da "experiência profissional" de forma agregada para o grupo de docentes.


## Grafico Matriz de Correlação entre Formação e Faixa Etária
![04_heatmap_correlacao](https://github.com/user-attachments/assets/18c3148a-1e19-49af-bc4e-bbc1b61910bf)
## Explicação do Gráfico: Matriz de Correlação entre Formação e Faixa Etária

O gráfico apresentado é uma **matriz de correlação**, visualizada como um *heatmap* (mapa de calor). Ele exibe a força e a direção da relação linear entre diferentes níveis de formação acadêmica dos docentes e suas faixas etárias, com base nos dados agregados por Unidade da Federação (UF).

**Como interpretar o gráfico:**

*   **Eixos:** Tanto o eixo horizontal quanto o vertical listam as mesmas variáveis: os diferentes níveis de formação (`Docentes_Graduacao`, `Docentes_Especializacao`, `Docentes_Mestrado`, `Docentes_Doutorado`) e as diferentes faixas etárias (`Docentes_Idade_30_34`, ..., `Docentes_Idade_60_mais`).
*   **Células e Valores:** Cada célula na interseção de duas variáveis mostra o coeficiente de correlação de Pearson entre elas. Este coeficiente varia de -1 a +1:
    *   **+1:** Correlação positiva perfeita (quando uma variável aumenta, a outra também aumenta proporcionalmente).
    *   **0:** Nenhuma correlação linear.
    *   **-1:** Correlação negativa perfeita (quando uma variável aumenta, a outra diminui proporcionalmente).
*   **Cores:** A barra de cores à direita indica a intensidade da correlação:
    *   **Cores quentes (vermelho intenso):** Correlação positiva forte (próxima de +1).
    *   **Cores frias (azul intenso):** Correlação negativa forte (próxima de -1).
    *   **Cores neutras (próximo ao branco/cinza claro):** Correlação fraca (próxima de 0).
*   **Diagonal Principal:** A diagonal de cima para baixo, da esquerda para a direita, sempre mostra o valor 1.00 (vermelho intenso), pois representa a correlação de cada variável consigo mesma, que é sempre perfeita.

**Principais observações e correlações:**

1.  **Alta Correlação entre Níveis de Pós-Graduação:**
    *   Há correlações muito fortes e positivas entre os diferentes níveis de pós-graduação. Por exemplo, `Docentes_Mestrado` e `Docentes_Doutorado` têm uma correlação de 0.98. Similarmente, `Docentes_Especializacao` e `Docentes_Mestrado` também apresentam 0.98.
    *   Isso sugere que as UFs que possuem um alto número de docentes com um tipo de pós-graduação (ex: mestrado) tendem a ter também um alto número de docentes com outros tipos de pós-graduação (ex: doutorado, especialização).

2.  **Alta Correlação entre Faixas Etárias Adjacentes e Próximas:**
    *   As faixas etárias demonstram correlações positivas muito altas entre si, especialmente as adjacentes. Por exemplo, `Docentes_Idade_35_39` e `Docentes_Idade_40_44` têm correlação de 0.99.
    *   Isso indica que UFs com muitos docentes em uma faixa etária específica tendem a ter também muitos docentes nas faixas etárias vizinhas.

3.  **Forte Correlação entre Níveis de Pós-Graduação e a Maioria das Faixas Etárias:**
    *   Os níveis de pós-graduação (`Docentes_Especializacao`, `Docentes_Mestrado`, `Docentes_Doutorado`) mostram correlações positivas consistentemente altas (geralmente acima de 0.90) com a maioria das faixas etárias, especialmente as intermediárias e mais velhas (a partir de `Docentes_Idade_35_39` até `Docentes_Idade_55_59`).
    *   Por exemplo, `Docentes_Mestrado` tem correlação de 1.00 com `Docentes_Idade_45_49`, e `Docentes_Doutorado` tem 0.99 com `Docentes_Idade_40_44` e `Docentes_Idade_45_49`.
    *   Isso sugere que UFs com um grande número de docentes pós-graduados tendem a ter um grande número de docentes distribuídos por diversas faixas etárias, refletindo um corpo docente qualificado e maduro.

4.  **Correlações Mais Baixas com `Docentes_Graduacao`:**
    *   A variável `Docentes_Graduacao` (que representa docentes apenas com graduação) apresenta correlações consideravelmente mais baixas com todos os outros níveis de formação e com todas as faixas etárias (valores variando de 0.26 a 0.40).
    *   Por exemplo, a correlação entre `Docentes_Graduacao` e `Docentes_Doutorado` é de 0.38, e entre `Docentes_Graduacao` e `Docentes_Idade_35_39` é de 0.40.
    *   Isso pode indicar que a distribuição de docentes apenas com graduação pelas UFs não segue o mesmo padrão da distribuição de docentes pós-graduados ou das diferentes faixas etárias de forma tão intensa.

5.  **Correlações Ligeiramente Menores nas Faixas Etárias Extremas com Formação:**
    *   Para a faixa etária mais jovem (`Docentes_Idade_30_34`), as correlações com os níveis mais altos de formação (Mestrado e Doutorado) são um pouco menores (0.95 e 0.94, respectivamente) em comparação com faixas etárias intermediárias. Isso é esperado, pois leva tempo para obter esses títulos.
    *   Da mesma forma, para a faixa `Docentes_Idade_60_mais`, as correlações com os níveis de pós-graduação também são um pouco menores, embora ainda altas (ex: 0.96 com Doutorado, 0.89 com `Docentes_Idade_35_39`).

**Contextualização para a Análise Exploratória de Dados:**

Esta matriz de correlação revela que, em nível estadual, a presença de docentes com alta qualificação (mestrado, doutorado) está fortemente associada à presença de docentes em diversas faixas etárias, especialmente as mais experientes. Indica também que estados com um forte contingente em um nível de pós-graduação tendem a ser fortes nos outros.

Para a pergunta de pesquisa sobre como formação e experiência (proxy pela idade) interagem para influenciar a disparidade salarial, esta análise mostra que, nos estados, há uma coocorrência significativa de alta formação e diversas faixas etárias. No entanto, a matriz não inclui dados salariais. Se dados salariais fossem adicionados, poderíamos investigar se UFs com alta correlação entre formação e idade (experiência) apresentam padrões específicos de disparidade salarial para "profissionais de dados". A ausência de uma forte correlação da variável `Docentes_Graduacao` com as demais sugere que este grupo pode ter características distintas que precisariam ser exploradas separadamente.


## Grafico Mapa Interativo de Bolhas - Distribuição de Docentes por Nível de Formação e UF
### [Grafico Interativo - Clique aqui](https://htmlpreview.github.io/?https://gist.githubusercontent.com/pedrinndias/9d708a6e00717a471ed00ab3e3742a40/raw/c1f0d385f7c9ad6f156de6d78dfcc9d245c68c99/06_mapa_bolhas_interativo.html)
![06_mapa_bolhas](https://github.com/user-attachments/assets/8a39d31d-a20f-4e3a-a51a-010005ad43b1)
## Explicação do Gráfico: Mapa Interativo de Bolhas - Distribuição de Docentes por Nível de Formação e UF

O gráfico apresentado é um **mapa de bolhas interativo** que visualiza a distribuição do número de docentes em cada Unidade da Federação (UF) do Brasil, segmentado por nível de formação acadêmica. Este tipo de gráfico utiliza círculos (bolhas) de tamanhos variados sobre um mapa para representar a magnitude de uma variável em diferentes regiões geográficas.

**Como interpretar o gráfico:**

*   **Base Geográfica:** O mapa do Brasil serve como plano de fundo, com as bolhas posicionadas sobre os respectivos estados.
*   **Bolhas:** Cada bolha no mapa representa um nível de formação específico dentro de um estado.
    *   **Cor da Bolha:** A cor da bolha indica o nível de formação acadêmica, conforme a legenda fornecida no gráfico:
        *   **Azul:** Docentes com Doutorado
        *   **Verde:** Docentes com Mestrado
        *   **Laranja/Amarelo:** Docentes com Especialização
        *   **Vermelho:** Docentes com Graduação
    *   **Tamanho da Bolha:** O tamanho da bolha é diretamente proporcional ao **número de docentes** com aquele nível de formação específico naquela UF. Bolhas maiores indicam um número maior de docentes.
    *   **Interatividade:** Ao passar o cursor do mouse sobre uma bolha, uma caixa de informações (tooltip) aparece, exibindo detalhes como a sigla da UF, o nível de formação representado pela bolha e o número exato de docentes correspondente.

**Principais observações do gráfico:**

*   **Concentração Regional de Alta Qualificação:** Observa-se visualmente que estados como São Paulo (SP), Minas Gerais (MG), Rio de Janeiro (RJ), Paraná (PR) e Rio Grande do Sul (RS) tendem a apresentar bolhas azuis (Doutorado) e verdes (Mestrado) proeminentes, indicando uma concentração significativa de docentes com alta qualificação nessas regiões.
*   **Predominância de Doutorado e Mestrado:** Em muitos estados, as bolhas azuis (Doutorado) e verdes (Mestrado) são as de maior tamanho, reforçando a constatação de gráficos anteriores sobre a alta qualificação (pós-graduação *stricto sensu*) do corpo docente na maioria das UFs.
*   **Variações Estaduais:** O mapa permite uma rápida comparação entre os estados. Alguns estados, especialmente nas regiões Norte e Nordeste, podem apresentar um volume total de docentes menor (bolhas geralmente menores) ou uma distribuição proporcional diferente entre os níveis de formação quando comparados aos estados do Sul e Sudeste.
*   **Baixa Representatividade da Graduação:** As bolhas vermelhas (Graduação), que representam docentes com apenas graduação, são consistentemente as menores em todos os estados, muitas vezes quase imperceptíveis, confirmando o baixo número de docentes que não possuem pós-graduação.

**Contextualização para a Análise Exploratória de Dados:**

Este mapa de bolhas interativo oferece uma dimensão geográfica à análise da formação acadêmica dos docentes. Ele permite identificar visualmente "hotspots" ou áreas de maior concentração de docentes por nível de formação.

No contexto da pergunta de pesquisa sobre "como fatores como formação acadêmica e experiência profissional interagem para influenciar a disparidade salarial entre profissionais de dados no Brasil", este gráfico contribui ao:
*   Mapear a distribuição da **formação acadêmica** dos docentes (o grupo disponível no dataset) pelo território nacional.
*   Permitir a identificação de estados com maior ou menor concentração de docentes altamente qualificados.

Para avançar na resposta à pergunta de pesquisa, seria necessário cruzar essas informações geográficas de formação com dados de experiência profissional (que poderiam ser agregados por UF) e, fundamentalmente, com dados salariais específicos para "profissionais de dados" em cada estado. O mapa atual é uma ferramenta exploratória valiosa para entender a distribuição da qualificação docente, mas não contém, por si só, informações sobre salários ou experiência para analisar diretamente a disparidade salarial de profissionais de dados.


## Grafico Gráfico de Dispersão 3D Interativo - Mestrado, Doutorado e Média de Idade dos Docentes por UF
### [Grafico Interativo - Clique aqui](https://htmlpreview.github.io/?https://gist.githubusercontent.com/pedrinndias/5edbfdc4c69d324455e65eef06c591b6/raw/d304db3742f4839c7bf4360c2ed75a06bce75bbe/07_3d_interativo.html)
![07_3d_interativo](https://github.com/user-attachments/assets/7b396546-3b72-4dc2-9897-0f6af9600cc7)
## Explicação do Gráfico: Gráfico de Dispersão 3D Interativo - Mestrado, Doutorado e Média de Idade dos Docentes por UF

O gráfico apresentado é um **gráfico de dispersão 3D interativo**. Ele visualiza a relação entre três variáveis para cada Unidade da Federação (UF) do Brasil: o número de docentes com mestrado, o número de docentes com doutorado e a média de idade dos docentes.

**Como interpretar o gráfico:**

*   **Eixos:** O gráfico possui três eixos, cada um representando uma variável quantitativa:
    *   **Eixo X (horizontal, profundidade):** `Docentes_Mestrado` - Número de docentes com título de Mestre na UF.
    *   **Eixo Y (horizontal, largura):** `Docentes_Doutorado` - Número de docentes com título de Doutor na UF.
    *   **Eixo Z (vertical, altura):** `Media_Idade_Docentes` - Média de idade dos docentes na UF.
*   **Pontos:** Cada ponto (esfera) no espaço 3D representa uma Unidade da Federação (UF). A posição do ponto é determinada pelos valores das três variáveis para aquela UF.
*   **Cores dos Pontos:** No gráfico visualizado, os pontos parecem ter uma cor azulada uniforme. A legenda ou interatividade poderiam revelar se a cor representa alguma outra variável, mas com base na imagem estática, ela parece ser apenas para visualização dos pontos.
*   **Interatividade:** Por ser um gráfico interativo (geralmente criado com bibliotecas como Plotly):
    *   **Rotação:** É possível girar o gráfico para visualizar a dispersão dos pontos de diferentes ângulos, ajudando a perceber padrões e relações espaciais.
    *   **Zoom:** Pode-se aproximar ou afastar para focar em regiões específicas do gráfico.
    *   **Hover (Passar o mouse):** Ao passar o cursor sobre um ponto, informações adicionais sobre aquela UF (como o nome da UF e os valores exatos das três variáveis) são tipicamente exibidas.

**Principais observações (baseadas na estrutura visual):**

*   **Relação entre Mestrado e Doutorado:** Observa-se uma tendência geral de que UFs com um alto número de docentes com mestrado (valores mais altos no eixo X) também tendem a ter um alto número de docentes com doutorado (valores mais altos no eixo Y). Isso é indicado pela dispersão dos pontos que tende a se estender diagonalmente no plano XY.
*   **Variação na Média de Idade:** Os pontos se distribuem em diferentes alturas ao longo do eixo Z, indicando variação na média de idade dos docentes entre as UFs.
*   **Identificação de Clusters e Outliers:**
    *   Pode haver agrupamentos (clusters) de UFs com características semelhantes (por exemplo, UFs com muitos mestres, muitos doutores e alta média de idade).
    *   Alguns pontos podem estar mais isolados (outliers), representando UFs com combinações menos comuns dessas três variáveis. Por exemplo, um ponto no canto superior direito do plano XY e alto no eixo Z representaria uma UF com muitos mestres, muitos doutores e uma alta média de idade dos docentes.
*   **Concentração de UFs:** A maioria dos pontos parece se concentrar em uma região onde os números de docentes com mestrado e doutorado não são os máximos observados, e a média de idade varia. Estados com grandes contingentes de docentes (como São Paulo, visualizado em gráficos anteriores) provavelmente se destacariam nas extremidades superiores dos eixos X e Y.

**Contextualização para a Análise Exploratória de Dados:**

Este gráfico 3D permite uma análise simultânea da **formação acadêmica** (níveis de mestrado e doutorado) e de um proxy para a **experiência profissional** (média de idade dos docentes) em nível estadual.

Para a pergunta de pesquisa ("Como fatores como formação acadêmica e experiência profissional interagem para influenciar a disparidade salarial entre profissionais de dados no Brasil?"):
*   Este gráfico visualiza diretamente a coocorrência de altos níveis de formação (mestrado e doutorado) e diferentes médias de idade (experiência) nas UFs.
*   Ele ajuda a identificar se UFs com um perfil específico de formação e idade (ex: alta formação e alta média de idade) se agrupam.

Contudo, assim como os gráficos anteriores, este não inclui dados salariais. Para analisar a disparidade salarial, seria necessário integrar informações de remuneração a essa análise tridimensional, possivelmente usando a cor ou o tamanho dos pontos para representar uma variável salarial, ou realizando análises estatísticas subsequentes com dados mais completos. Este gráfico é uma ferramenta exploratória poderosa para entender a inter-relação das variáveis de formação e idade dos docentes entre os estados.


---

## Analise exploratoria de dados bases integradas

---

## Grafico Salário Médio Estimado e Total de Docentes por UF
![bar_line_salario_medio_total_docentes_uf](https://github.com/user-attachments/assets/6060f457-2f9f-4c68-9839-82f9f4ac9312)
## Análise do Gráfico: Salário Médio Estimado e Total de Docentes por UF

O gráfico apresentado é uma visualização combinada que utiliza barras para representar o "Salário Médio Estimado (R$)" dos profissionais de dados e uma linha para mostrar o "Total de Docentes na UF" (Unidade Federativa) onde esses profissionais residem.

**Elementos do Gráfico:**

*   **Eixo X (Horizontal):** Apresenta as Unidades Federativas (UF onde mora), ordenadas da esquerda para a direita, aparentemente pela ordem decrescente do salário médio estimado.
*   **Eixo Y Esquerdo (Vertical):** Indica o "Salário Médio Estimado (R$)" e corresponde às barras vermelhas. A escala varia de R$0 a R$14.000.
*   **Eixo Y Direito (Vertical):** Representa o "Total de Docentes na UF" e corresponde à linha azul tracejada com marcadores. A escala vai de 0 a aproximadamente 70.000.
*   **Barras Vermelhas (Salário Médio):** Cada barra mostra o salário médio estimado dos profissionais de dados para uma UF específica.
*   **Linha Azul Tracejada (Total Docentes):** A linha indica o número total de docentes em cada UF.

**Observações e Interpretações:**

*   **Salário Médio Estimado:**
    *   Tocantins (TO) exibe o maior salário médio estimado, superando os R$14.000.
    *   O Distrito Federal (DF) e São Paulo (SP) aparecem em seguida, com salários médios entre R$9.000 e R$10.000 para o DF e um pouco acima de R$9.000 para SP.
    *   Observa-se uma tendência de diminuição do salário médio ao se mover da esquerda para a direita do gráfico. UFs como Piauí (PI) e Rondônia (RO) apresentam os menores salários médios, em torno de R$4.000.

*   **Total de Docentes:**
    *   São Paulo (SP) possui, de longe, o maior número de docentes, ultrapassando 70.000.
    *   Minas Gerais (MG) e Rio de Janeiro (RJ) também têm um volume expressivo de docentes (MG entre 30.000 e 40.000, RJ acima de 30.000).
    *   Muitas outras UFs, incluindo aquelas com salários médios mais baixos e algumas com salários mais altos como TO e DF, têm um número consideravelmente menor de docentes (frequentemente abaixo de 10.000 ou 20.000).

*   **Relação entre Salário Médio e Total de Docentes:**
    *   **Não se observa uma correlação direta e simples** entre o salário médio dos profissionais de dados e o número total de docentes na UF.
        *   Por exemplo, TO tem o salário médio mais alto, mas um número relativamente baixo de docentes.
        *   SP combina um salário médio alto (terceiro maior) com o maior número de docentes.
        *   DF possui o segundo maior salário médio, mas um número de docentes bem inferior ao de SP, MG ou RJ.
    *   Isso sugere que o salário médio dos profissionais de dados em cada estado é influenciado por um conjunto de fatores que vai além da quantidade de docentes (que poderia ser um indicador da oferta de formação ou do tamanho do sistema educacional). Fatores como a demanda do mercado de trabalho local, o custo de vida, a concentração de empresas de tecnologia e o nível de desenvolvimento econômico da UF provavelmente desempenham papéis cruciais.

**Conclusão do Gráfico:**

O gráfico demonstra que não há uma relação causal direta entre o número de docentes em uma UF e o salário médio dos profissionais de dados nessa mesma UF. Enquanto São Paulo apresenta um alto volume de docentes e um alto salário médio, o caso de Tocantins (alto salário médio, poucos docentes) exemplifica que outros fatores são determinantes para a remuneração na área de dados. A dinâmica salarial é complexa e moldada por múltiplas variáveis, não sendo explicada isoladamente pela infraestrutura educacional em termos de quantidade de docentes.

## Grafico Salário Estimado por Área de Formação - Top 5
![boxplot_salario_por_area_formacao_top5](https://github.com/user-attachments/assets/521f1e12-e4bb-445e-982d-733d52142401)
## Análise do Gráfico: Salário Estimado por Área de Formação (Top 5)

O gráfico apresentado é um boxplot que ilustra a distribuição do "Salário Estimado (R$)" para as cinco principais áreas de formação dos profissionais de dados. Cada boxplot resume a distribuição salarial para uma área específica, permitindo comparações entre elas.

**Elementos do Gráfico:**

*   **Eixo Y (Vertical):** "Área de Formação", listando as cinco categorias de formação mais comuns ou relevantes.
    *   Computação / Engenharia de Software / Sistemas de Informação/ TI
    *   Outras Engenharias
    *   Economia/ Administração / Contabilidade / Finanças/ Negócios
    *   Estatística/ Matemática / Matemática Computacional/ Ciências Atuariais
    *   Outra opção
*   **Eixo X (Horizontal):** "Salário Estimado (R$)", variando de R$0 até mais de R$40.000.
*   **Boxplot (Caixa e Bigodes):** Para cada área de formação:
    *   A **linha central** dentro da caixa representa a **mediana** salarial (o valor que divide os salários em 50% abaixo e 50% acima).
    *   A **caixa** em si abrange o **intervalo interquartil (IQR)**, ou seja, os 50% centrais dos salários (do primeiro quartil - Q1 - ao terceiro quartil - Q3). A largura da caixa indica a dispersão desses salários centrais.
    *   Os **"bigodes"** (linhas que se estendem a partir da caixa) mostram o alcance dos salários, geralmente até 1.5 vezes o IQR a partir da caixa.
    *   Os **pontos individuais** (losangos) fora dos bigodes são considerados **outliers**, indicando salários atipicamente altos ou baixos em relação ao restante do grupo.

**Observações e Interpretações por Área de Formação:**

1.  **Computação / Engenharia de Software / Sistemas de Informação/ TI:**
    *   **Mediana Salarial:** Parece ser a mais alta entre as áreas, situada próxima a R$10.000.
    *   **Dispersão (IQR):** A caixa é relativamente compacta, sugerindo que a maioria dos profissionais dessa área tem salários concentrados em torno da mediana.
    *   **Alcance e Outliers:** Apresenta um alcance considerável nos bigodes e múltiplos outliers indicando salários bem elevados, alguns ultrapassando R$40.000.

2.  **Outras Engenharias:**
    *   **Mediana Salarial:** Ligeiramente inferior à de Computação/TI, talvez em torno de R$8.000 - R$9.000.
    *   **Dispersão (IQR):** Similar ou um pouco maior que Computação/TI.
    *   **Alcance e Outliers:** Também possui um bom alcance e múltiplos outliers com salários altos.

3.  **Economia/ Administração / Contabilidade / Finanças/ Negócios:**
    *   **Mediana Salarial:** Parece estar na faixa de R$7.000 - R$8.000.
    *   **Dispersão (IQR):** A caixa aparenta ser um pouco mais larga, indicando uma maior variabilidade nos salários do grupo central em comparação com Computação/TI.
    *   **Alcance e Outliers:** Presença de outliers com salários elevados.

4.  **Estatística/ Matemática / Matemática Computacional/ Ciências Atuariais:**
    *   **Mediana Salarial:** Próxima à área de Economia/Negócios, possivelmente entre R$7.000 e R$8.000.
    *   **Dispersão (IQR):** A caixa parece ter uma dispersão considerável.
    *   **Alcance e Outliers:** Também exibe outliers significativos.

5.  **Outra opção:**
    *   **Mediana Salarial:** Aparenta ter a menor mediana entre as cinco categorias, talvez em torno de R$6.000 - R$7.000.
    *   **Dispersão (IQR):** A caixa parece ser relativamente larga, sugerindo uma variabilidade salarial significativa dentro deste grupo.
    *   **Alcance e Outliers:** Possui outliers, incluindo um que se destaca próximo a R$40.000.

**Comparações e Conclusões Gerais:**

*   Profissionais com formação na área de **Computação / Engenharia de Software / Sistemas de Informação/ TI** tendem a ter a mediana salarial mais alta.
*   Todas as áreas de formação apresentam uma dispersão salarial considerável, evidenciada pelos tamanhos das caixas e, principalmente, pela presença de outliers com salários significativamente altos. Isso sugere que, dentro de cada área, há profissionais que conseguem remunerações bem acima da média do seu grupo.
*   A categoria "Outra opção" apresenta a menor mediana salarial, o que é esperado, pois agrupa diversas formações menos diretamente ligadas às habilidades centrais da área de dados.
*   As áreas de "Outras Engenharias", "Economia/Administração/etc." e "Estatística/Matemática/etc." apresentam medianas salariais intermediárias e relativamente próximas entre si, mas com variações na dispersão dos salários.

Este gráfico é útil para entender como a área de formação inicial se relaciona com os níveis salariais no campo de dados, destacando que, embora formações em TI/Computação pareçam ter uma vantagem na mediana, todas as áreas analisadas possuem profissionais alcançando altos patamares salariais.


## Grafico Salário Estimado por Tempo de Experiência
### [Grafico Interativo - Clique aqui](https://htmlpreview.github.io/?https://gist.githubusercontent.com/pedrinndias/a62a1fa0a659e7a351b966759dafa417/raw/4b807c1571bb235ffa8469985f8f14d4f3c80d74/boxplot_salario_por_experiencia_plotly.html)
![newplot](https://github.com/user-attachments/assets/3733a3c3-9327-497c-87db-1550f799e558)
## Análise do Gráfico: Salário Estimado por Tempo de Experiência

O gráfico visualizado é um boxplot que demonstra a distribuição do "Salário Estimado (R$)" para diferentes níveis de "Tempo de Experiência na Área de Dados (Anos Estimados)". Essa representação gráfica permite comparar como a remuneração varia conforme os profissionais acumulam mais anos de experiência na área.

**Elementos do Gráfico:**

*   **Eixo Y (Vertical):** Representa as categorias de "Tempo de Experiência na Área de Dados (Anos Estimados)". As categorias são:
    *   Menos de 1 ano (Rotulado como 0.5 no gráfico)
    *   de 1 a 2 anos (Rotulado como 1.5)
    *   de 3 a 4 anos (Rotulado como 3.5)
    *   de 4 a 6 anos (Rotulado como 5.0)
    *   de 6 a 10 anos (Rotulado como 8.0)
    *   Mais de 10 anos (Rotulado como 10.0)
*   **Eixo X (Horizontal):** Indica o "Salário Estimado (R$)", com valores que vão de R$0 até mais de R$30.000.
*   **Boxplot (Diagrama de Caixa):** Para cada faixa de experiência, o boxplot exibe:
    *   A **linha central** na caixa: Representa a **mediana** salarial (50º percentil), o valor que divide os salários em duas metades iguais.
    *   A **caixa**: Abrange o **intervalo interquartil (IQR)**, que contém os 50% centrais dos dados salariais (do primeiro quartil, Q1 ou 25º percentil, ao terceiro quartil, Q3 ou 75º percentil). A altura da caixa indica a dispersão dos salários nesse intervalo central.
    *   Os **"bigodes" (whiskers)**: Linhas que se estendem da caixa para mostrar o alcance dos dados salariais, geralmente até 1.5 vezes o IQR. Valores além dos bigodes podem ser outliers.
    *   **Outliers**: Pontos individuais (neste gráfico, parecem pequenos círculos) que se localizam fora dos bigodes, indicando salários atipicamente altos ou baixos em comparação com o restante do grupo para aquela faixa de experiência.

**Observações e Interpretações por Faixa de Experiência:**

1.  **Menos de 1 ano (0.5):**
    *   **Mediana Salarial:** A mais baixa entre todas as faixas, situando-se em torno de R$2.000 - R$3.000.
    *   **Dispersão (IQR):** A caixa é relativamente compacta, mas há uma concentração na parte inferior da faixa salarial.
    *   **Outliers:** Apresenta alguns outliers, indicando que mesmo com pouca experiência, alguns profissionais conseguem salários acima da média do grupo.

2.  **de 1 a 2 anos (1.5):**
    *   **Mediana Salarial:** Aumenta visivelmente em relação à faixa anterior, provavelmente entre R$4.000 e R$5.000.
    *   **Dispersão (IQR):** A caixa se expande, mostrando maior variabilidade salarial.
    *   **Outliers:** Mais outliers presentes, e com valores mais altos.

3.  **de 3 a 4 anos (3.5):**
    *   **Mediana Salarial:** Continua a crescer, situando-se talvez em torno de R$7.000 - R$8.000.
    *   **Dispersão (IQR):** A dispersão dos 50% centrais dos salários aumenta.
    *   **Outliers:** Número significativo de outliers, alcançando salários mais elevados.

4.  **de 4 a 6 anos (5.0):**
    *   **Mediana Salarial:** Apresenta um salto expressivo, posicionando-se próximo ou acima de R$10.000.
    *   **Dispersão (IQR):** A caixa é mais ampla, refletindo uma maior diversidade salarial.
    *   **Outliers:** Muitos outliers, com alguns ultrapassando R$30.000.

5.  **de 6 a 10 anos (8.0):**
    *   **Mediana Salarial:** Continua a tendência de alta, possivelmente entre R$12.000 e R$14.000.
    *   **Dispersão (IQR):** Grande dispersão salarial, com a caixa sendo bastante longa.
    *   **Outliers:** Vários outliers com salários muito altos.

6.  **Mais de 10 anos (10.0):**
    *   **Mediana Salarial:** Atinge o patamar mais alto, superando R$15.000 e aproximando-se de R$18.000 - R$20.000.
    *   **Dispersão (IQR):** A maior dispersão entre todas as faixas, indicando uma ampla gama de salários para os profissionais mais experientes.
    *   **Outliers:** Presença marcante de outliers com os salários mais altos do dataset, muitos acima de R$30.000.

**Conclusões Gerais:**

*   **Impacto Positivo da Experiência:** Há uma clara e consistente tendência de aumento da mediana salarial à medida que o tempo de experiência na área de dados aumenta. Profissionais com mais anos de atuação tendem a receber salários significativamente maiores.
*   **Aumento da Dispersão Salarial com a Experiência:** Não apenas a mediana, mas também a dispersão dos salários (representada pelo tamanho da caixa e pelo alcance dos bigodes e outliers) tende a aumentar com a experiência. Isso sugere que, entre os profissionais mais experientes, há uma variação salarial maior – alguns podem ter salários excepcionalmente altos, enquanto outros podem permanecer em faixas mais modestas em comparação com os "top earners" do mesmo nível de experiência.
*   **Potencial de Altos Salários:** Em todas as faixas de experiência, a presença de outliers superiores indica que existem oportunidades para alcançar salários acima da média do respectivo grupo, mas essa possibilidade se torna mais pronunciada e os valores mais altos com o aumento da experiência.

Este gráfico reforça a noção de que a experiência profissional é um fator crucial na progressão salarial dentro da área de dados no Brasil, com os profissionais mais experientes não apenas alcançando medianas salariais mais altas, mas também apresentando uma gama mais ampla de possibilidades de remuneração.


## Grafico Salário Estimado por Tempo de Experiência em Dados
![boxplot_salario_por_experiencia_seaborn](https://github.com/user-attachments/assets/1ae56e9f-614e-490c-9cea-c70402bd333c)
## Análise do Gráfico: Salário Estimado por Tempo de Experiência em Dados

O gráfico de boxplot anexado ilustra a relação entre o "Tempo de Experiência" dos profissionais de dados e o "Salário Estimado (R$)". Cada caixa no gráfico representa a distribuição salarial para uma faixa específica de anos de experiência.

**Elementos do Gráfico:**

*   **Eixo Y (Vertical):** "Tempo de Experiência", dividido nas seguintes categorias:
    *   Menos de 1 ano
    *   de 1 a 2 anos
    *   de 3 a 4 anos
    *   de 5 a 6 anos
    *   de 7 a 10 anos
    *   Mais de 10 anos
*   **Eixo X (Horizontal):** "Salário Estimado (R$)", com escala de R$0 até mais de R$40.000.
*   **Boxplot (Diagrama de Caixa):** Para cada categoria de experiência:
    *   A **linha vertical dentro da caixa** indica a **mediana** salarial (o valor central que divide os salários em 50% abaixo e 50% acima).
    *   A **caixa (box)** representa o **intervalo interquartil (IQR)**, contendo os 50% centrais dos salários (do primeiro quartil - Q1 - ao terceiro quartil - Q3). A largura da caixa mostra a dispersão desses salários centrais.
    *   Os **"bigodes" (whiskers)** são as linhas horizontais que se estendem da caixa, mostrando o alcance principal dos salários (tipicamente 1.5 vezes o IQR).
    *   Os **pontos individuais (losangos)** fora dos bigodes são considerados **outliers**, representando salários atipicamente altos ou baixos em relação ao grosso dos dados para aquela faixa de experiência.

**Observações e Interpretações por Faixa de Experiência:**

1.  **Menos de 1 ano:**
    *   **Mediana Salarial:** A mais baixa, em torno de R$4.000.
    *   **Dispersão (IQR):** Relativamente concentrada, com a maioria dos salários entre aproximadamente R$2.000 e R$6.000.
    *   **Outliers:** Alguns outliers superiores, chegando até cerca de R$20.000.

2.  **de 1 a 2 anos:**
    *   **Mediana Salarial:** Aumenta para cerca de R$6.000.
    *   **Dispersão (IQR):** A caixa se alarga um pouco, com salários centrais entre R$4.000 e R$8.000, aproximadamente.
    *   **Outliers:** Mais outliers e com valores mais altos, alguns ultrapassando R$30.000.

3.  **de 3 a 4 anos:**
    *   **Mediana Salarial:** Um salto significativo, posicionando-se em torno de R$9.000 - R$10.000.
    *   **Dispersão (IQR):** Maior variabilidade, com a caixa indo de cerca de R$6.000 a R$12.000.
    *   **Outliers:** Vários outliers, com alguns alcançando e ultrapassando R$40.000.

4.  **de 5 a 6 anos:**
    *   **Mediana Salarial:** Continua a crescer, situando-se em torno de R$12.000.
    *   **Dispersão (IQR):** A caixa é ampla, indicando diversidade salarial, aproximadamente entre R$8.000 e R$16.000.
    *   **Outliers:** Presença de outliers tanto superiores (ultrapassando R$40.000) quanto inferiores (próximos a R$0).

5.  **de 7 a 10 anos:**
    *   **Mediana Salarial:** Aumenta para cerca de R$14.000 - R$15.000.
    *   **Dispersão (IQR):** A caixa se estende de aproximadamente R$10.000 a R$20.000.
    *   **Outliers:** Similar à faixa anterior, com outliers em ambas as extremidades.

6.  **Mais de 10 anos:**
    *   **Mediana Salarial:** A mais alta, em torno de R$16.000 - R$18.000.
    *   **Dispersão (IQR):** A maior dispersão dos salários centrais, com a caixa indo de cerca de R$12.000 a R$25.000. Isso indica uma grande variação salarial entre os profissionais mais experientes.
    *   **Outliers:** Numerosos outliers, especialmente na extremidade superior, indicando que profissionais com vasta experiência podem alcançar remunerações muito elevadas. Também há outliers inferiores.

**Conclusões Gerais:**

*   **Progressão Salarial com Experiência:** O gráfico demonstra claramente que a mediana salarial tende a aumentar consistentemente com o aumento do tempo de experiência na área de dados.
*   **Aumento da Variabilidade Salarial:** À medida que a experiência aumenta, não só a mediana salarial cresce, mas também a dispersão dos salários (indicada pela largura da caixa e pela presença de outliers). Isso sugere que, com mais experiência, as faixas salariais se tornam mais amplas.
*   **Potencial de Alta Remuneração:** Em todos os níveis de experiência, existem profissionais (outliers) que ganham significativamente mais do que a mediana do seu grupo. Esse potencial para salários muito altos é particularmente evidente nas faixas de maior experiência.
*   **Outliers Inferiores:** A presença de outliers na extremidade inferior, especialmente nas faixas de maior experiência, pode indicar diversos cenários, como transições de carreira, atuação em setores ou regiões com menor remuneração, ou outros fatores não capturados apenas pela variável "tempo de experiência".

Este gráfico é uma ferramenta visual eficaz para entender como a remuneração na área de dados evolui com a experiência, destacando a valorização progressiva dos profissionais à medida que acumulam mais anos de atuação.


## Grafico Salário Estimado por Nível de Ensino
### [Grafico Interativo - Clique aqui](https://htmlpreview.github.io/?https://gist.githubusercontent.com/pedrinndias/d4a35514b072e73dcb602e3c936f3324/raw/da8b4afe7bd6ce83a87a646bfc6e978bee28b69a/gistfile1.txt)
![newplot(1)](https://github.com/user-attachments/assets/933aba1b-01fa-45fe-b4ad-6380af43469e)
## Análise do Gráfico: Salário Estimado por Nível de Ensino

O gráfico visualizado é um boxplot que ilustra a distribuição do "Salário Estimado (R$)" para diferentes categorias de "Nível de Ensino" alcançado pelos profissionais de dados. Este tipo de gráfico é uma ferramenta eficaz na análise exploratória de dados para comparar a tendência central, dispersão e identificar valores atípicos entre diferentes grupos.

**Elementos do Gráfico:**

*   **Eixo Y (Vertical):** "Nível de Ensino", apresentando as seguintes categorias:
    *   Estudante de Graduação
    *   Graduação/Bacharelado
    *   Pós-graduação
    *   Mestrado
    *   Doutorado ou Phd
*   **Eixo X (Horizontal):** "Salário Estimado (R$)", com a escala variando de R$0 até mais de R$30.000.
*   **Boxplot (Diagrama de Caixa):** Para cada nível de ensino, o boxplot resume a distribuição salarial da seguinte forma:
    *   A **linha vertical dentro da caixa** representa a **mediana** salarial (o 50º percentil), que é o valor central dividindo os salários em duas metades iguais.
    *   A **caixa (box)** delimita o **intervalo interquartil (IQR)**, que contém os 50% centrais dos dados salariais (do primeiro quartil, Q1 ou 25º percentil, ao terceiro quartil, Q3 ou 75º percentil). A largura da caixa indica a dispersão dos salários neste intervalo.
    *   Os **"bigodes" (whiskers)** são as linhas horizontais que se estendem a partir da caixa, mostrando o alcance dos dados salariais considerados típicos (geralmente até 1.5 vezes o IQR a partir da caixa).
    *   Os **pontos individuais (losangos)** localizados fora dos bigodes são considerados **outliers**, indicando salários que são atipicamente altos ou baixos em comparação com o restante dos profissionais naquele nível de ensino.

**Observações e Interpretações por Nível de Ensino:**

1.  **Estudante de Graduação:**
    *   **Mediana Salarial:** A mais baixa entre todos os níveis, situando-se em torno de R$2.000 - R$3.000.
    *   **Dispersão (IQR):** A caixa é relativamente compacta, indicando que a maioria dos estudantes de graduação tem salários próximos a essa mediana baixa.
    *   **Outliers:** Apresenta alguns outliers superiores, sugerindo que alguns estudantes já conseguem remunerações mais elevadas.

2.  **Graduação/Bacharelado:**
    *   **Mediana Salarial:** Aumenta consideravelmente em relação aos estudantes, posicionando-se em torno de R$7.000 - R$8.000.
    *   **Dispersão (IQR):** A caixa é mais ampla, mostrando uma maior variabilidade nos salários dos graduados.
    *   **Outliers:** Presença significativa de outliers, com alguns salários ultrapassando R$30.000.

3.  **Pós-graduação:**
    *   **Mediana Salarial:** Ligeiramente superior à da graduação, talvez em torno de R$8.000 - R$9.000.
    *   **Dispersão (IQR):** A dispersão parece similar ou um pouco maior que a dos graduados.
    *   **Outliers:** Muitos outliers, alcançando patamares salariais elevados.

4.  **Mestrado:**
    *   **Mediana Salarial:** Apresenta um aumento notável em relação à pós-graduação, situando-se acima de R$10.000, talvez próximo a R$12.000.
    *   **Dispersão (IQR):** A caixa é relativamente ampla, indicando uma boa variabilidade salarial.
    *   **Outliers:** Muitos outliers com salários altos, alguns bem acima de R$30.000.

5.  **Doutorado ou Phd:**
    *   **Mediana Salarial:** A mais alta entre todos os níveis de ensino, superando a do mestrado e posicionando-se em torno de R$14.000 - R$15.000.
    *   **Dispersão (IQR):** A caixa é bastante extensa, refletindo uma grande dispersão salarial entre os doutores.
    *   **Outliers:** Presença marcante de outliers com os salários mais elevados do conjunto de dados, indicando um alto potencial de ganhos para este grupo.

**Conclusões Gerais:**

*   **Impacto Positivo do Nível de Ensino:** O gráfico demonstra uma tendência clara de aumento da mediana salarial à medida que o nível de ensino aumenta. Profissionais com níveis de formação mais elevados (Mestrado, Doutorado) tendem a ter medianas salariais significativamente maiores.
*   **Aumento da Dispersão Salarial em Níveis Mais Altos:** Nos níveis de ensino mais elevados, especialmente Doutorado, não apenas a mediana é maior, mas também a dispersão dos salários (o tamanho da caixa e o alcance dos outliers). Isso sugere uma gama mais ampla de remunerações, com alguns profissionais alcançando salários excepcionalmente altos.
*   **Valor da Graduação:** Há um salto salarial expressivo ao se completar a graduação em comparação com o nível de estudante.
*   **Outliers Significativos:** Em todos os níveis a partir da graduação, a presença de outliers superiores indica que, independentemente do nível de formação específico (pós-graduação, mestrado), existem oportunidades para alcançar salários bem acima da média do grupo.

Este gráfico reforça a ideia de que o investimento em educação formal, especialmente em níveis mais avançados como mestrado e doutorado, está associado a um maior potencial de remuneração na área de dados no Brasil.


## Grafico Salário Estimado por Nível de Ensino
![boxplot_salario_por_nivel_ensino_seaborn](https://github.com/user-attachments/assets/320b22fc-43fb-40af-be93-e02572699fec)
## Análise do Gráfico: Salário Estimado por Nível de Ensino

O gráfico anexado é um boxplot que exibe a distribuição do "Salário Estimado (R$)" para diferentes níveis de escolaridade ("Nível de Ensino") alcançados pelos profissionais de dados. Esta visualização permite comparar como a remuneração varia entre os diferentes graus de formação acadêmica.

**Elementos do Gráfico:**

*   **Eixo Y (Vertical):** "Nível de Ensino", com as seguintes categorias (de cima para baixo):
    *   Estudante de Graduação
    *   Graduação/Bacharelado
    *   Pós-graduação
    *   Mestrado
    *   Doutorado ou Phd
*   **Eixo X (Horizontal):** "Salário Estimado (R$)", com uma escala que se estende de R$0 até mais de R$40.000.
*   **Boxplot (Diagrama de Caixa):** Para cada nível de ensino, o boxplot mostra:
    *   A **linha vertical dentro da caixa**: Indica a **mediana** salarial (o valor que divide a distribuição dos salários em duas metades iguais).
    *   A **caixa**: Representa o **intervalo interquartil (IQR)**, que contém os 50% centrais dos salários (entre o primeiro quartil - Q1 - e o terceiro quartil - Q3). A largura da caixa reflete a dispersão desses salários centrais.
    *   Os **"bigodes" (whiskers)**: Linhas horizontais que se estendem da caixa para mostrar o alcance dos salários considerados típicos.
    *   Os **pontos individuais (losangos)**: Representam **outliers**, ou seja, salários que são atipicamente altos (ou baixos) em comparação com a maioria dos profissionais daquele nível de ensino.

**Observações e Interpretações por Nível de Ensino:**

1.  **Estudante de Graduação:**
    *   **Mediana Salarial:** É a mais baixa de todas as categorias, situando-se em torno de R$4.000 - R$5.000.
    *   **Dispersão (IQR):** A caixa é relativamente estreita, indicando que a maioria dos estudantes de graduação tem salários concentrados em uma faixa menor, aproximadamente entre R$2.500 e R$6.000.
    *   **Outliers:** Apresenta alguns outliers superiores, com salários chegando a cerca de R$15.000, e um outlier próximo a R$20.000.

2.  **Graduação/Bacharelado:**
    *   **Mediana Salarial:** Aumenta significativamente em relação aos estudantes, localizando-se em torno de R$8.000 - R$9.000.
    *   **Dispersão (IQR):** A caixa é consideravelmente mais larga, com os 50% centrais dos salários variando aproximadamente de R$5.000 a R$12.000, indicando maior variabilidade salarial.
    *   **Outliers:** Numerosos outliers superiores, com vários profissionais alcançando salários acima de R$20.000, R$30.000 e até R$40.000.

3.  **Pós-graduação:**
    *   **Mediana Salarial:** Um pouco superior à da graduação, possivelmente em torno de R$9.000 - R$10.000.
    *   **Dispersão (IQR):** Semelhante ou ligeiramente maior que a da graduação, com salários centrais entre aproximadamente R$6.000 e R$14.000.
    *   **Outliers:** Também apresenta muitos outliers com salários elevados, ultrapassando R$40.000 em alguns casos.

4.  **Mestrado:**
    *   **Mediana Salarial:** Demonstra um novo aumento, situando-se em torno de R$10.000 - R$12.000.
    *   **Dispersão (IQR):** A caixa é ampla, indicando uma variabilidade salarial considerável, com os 50% centrais entre aproximadamente R$7.000 e R$15.000.
    *   **Outliers:** Vários outliers superiores, incluindo salários acima de R$20.000, R$30.000 e alguns próximos ou acima de R$40.000.

5.  **Doutorado ou Phd:**
    *   **Mediana Salarial:** A mais alta entre todos os níveis de ensino, posicionando-se em torno de R$12.000 - R$14.000.
    *   **Dispersão (IQR):** A caixa é bastante larga, indicando uma grande dispersão salarial. Os 50% centrais dos salários parecem estar entre R$8.000 e R$20.000.
    *   **Outliers:** Presença marcante de outliers com salários elevados, com vários profissionais superando R$30.000 e R$40.000. Há também um outlier inferior, próximo a R$0.

**Conclusões Gerais:**

*   **Valorização da Educação:** O gráfico evidencia uma tendência geral de aumento da mediana salarial conforme o nível de ensino aumenta. Profissionais com níveis de formação mais avançados, como Mestrado e Doutorado, tendem a ter medianas salariais mais altas.
*   **Aumento da Dispersão com Níveis Mais Altos:** A variabilidade salarial (largura da caixa e presença de outliers) também tende a ser maior nos níveis de ensino mais elevados. Isso sugere que, embora a mediana aumente, a faixa de salários possíveis também se amplia, especialmente para cima.
*   **Salto Salarial Pós-Graduação (Lato Sensu e Stricto Sensu):** Completar uma graduação representa um salto salarial significativo em relação ao status de estudante. Pós-graduações (incluindo especializações, mestrado e doutorado) continuam essa tendência de aumento na mediana salarial.
*   **Potencial de Alta Remuneração:** Em todos os níveis a partir da Graduação/Bacharelado, a existência de múltiplos outliers superiores indica que há profissionais que alcançam remunerações consideravelmente acima da média de seus respectivos grupos de escolaridade. Esse potencial parece se acentuar com o Doutorado.

Este gráfico sugere que o investimento em educação formal, particularmente em níveis mais avançados, está associado a um maior potencial de ganhos na área de dados.


## Grafico Salário Estimado por Experiência, Agrupado por Nível de Ensino
![catplot_salario_exp_facet_nivel_ensino](https://github.com/user-attachments/assets/71164ccd-585b-4354-8473-631eac8a4f02)
## Análise do Gráfico: Salário Estimado por Experiência, Agrupado por Nível de Ensino

O gráfico apresentado é um conjunto de boxplots (diagramas de caixa) que visualiza a interação entre "Tempo de Experiência" e "Nível de Ensino" na determinação do "Salário Estimado (R$)" dos profissionais de dados. O gráfico é facetado por "Nível de Ensino", o que significa que para cada nível de escolaridade, há uma série de boxplots mostrando a distribuição salarial para diferentes faixas de tempo de experiência.

**Elementos do Gráfico:**

*   **Título Principal:** "Salário Estimado por Experiência, Agrupado por Nível de Ensino".
*   **Facetas (Subgráficos):** Cada subgráfico representa um "Nível de Ensino" específico:
    *   Estudante de Graduação
    *   Graduação/Bacharelado
    *   Pós-graduação
    *   Mestrado
    *   Doutorado ou Phd
*   **Eixo Y (Vertical) de cada subgráfico:** "Salário Estimado (R$)", com escala de R$0 a R$40.000.
*   **Eixo X (Horizontal) de cada subgráfico:** "Tempo de Experiência". Embora as categorias exatas não estejam rotuladas individualmente no eixo x de cada faceta, a progressão das caixas da esquerda para a direita (e as cores distintas das caixas) dentro de cada subgráfico representa o aumento do tempo de experiência. Podemos inferir que são as mesmas faixas de experiência usadas em gráficos anteriores (ex: <1 ano, 1-2 anos, 3-4 anos, 5-6 anos, 7-10 anos, Mais de 10 anos).
*   **Boxplot (Diagrama de Caixa):** Para cada combinação de nível de ensino e faixa de experiência:
    *   A **linha horizontal dentro da caixa** indica a **mediana** salarial.
    *   A **caixa** representa o **intervalo interquartil (IQR)**, contendo os 50% centrais dos salários.
    *   Os **"bigodes" (whiskers)** mostram o alcance dos salários considerados típicos.
    *   Os **pontos individuais (losangos)** são **outliers**, indicando salários atipicamente altos ou baixos.

**Observações e Interpretações:**

**Tendência Geral Dentro de Cada Nível de Ensino:**

*   **Progressão Salarial com Experiência:** Em *todos* os níveis de ensino, há uma clara tendência de aumento da mediana salarial (a linha dentro da caixa) à medida que o tempo de experiência aumenta (movendo-se da esquerda para a direita dentro de cada subgráfico). Isso é visível pela subida geral das caixas.
*   **Aumento da Dispersão com Experiência:** Frequentemente, a dispersão salarial (altura da caixa e alcance dos bigodes/outliers) também aumenta com mais experiência. Isso significa que, entre os mais experientes, há uma variação salarial maior.

**Comparações Entre Níveis de Ensino para Faixas de Experiência Similares:**

1.  **Início de Carreira (Faixas de Menor Experiência - caixas à esquerda):**
    *   **Estudantes de Graduação:** Apresentam as menores medianas salariais em todas as faixas de experiência que participam.
    *   **Graduação/Bacharelado e Pós-graduação:** Para pouca experiência, as medianas salariais são semelhantes e mais altas que as dos estudantes. A pós-graduação parece oferecer uma ligeira vantagem inicial sobre apenas a graduação.
    *   **Mestrado e Doutorado:** Mesmo com pouca experiência, profissionais com mestrado e, especialmente, doutorado, tendem a ter medianas salariais iniciais mais altas em comparação com os níveis de ensino inferiores.

2.  **Meio de Carreira (Faixas de Experiência Intermediárias - caixas centrais):**
    *   A diferença salarial entre os níveis de ensino torna-se mais pronunciada.
    *   **Graduação/Bacharelado e Pós-graduação:** A pós-graduação continua a mostrar uma vantagem sobre a graduação.
    *   **Mestrado e Doutorado:** Apresentam medianas salariais consistentemente mais altas. Profissionais com doutorado, com experiência intermediária, já alcançam patamares salariais elevados.

3.  **Final de Carreira (Faixas de Maior Experiência - caixas à direita):**
    *   **Estudantes de Graduação:** Mesmo com mais experiência (se aplicável dentro do status de estudante), os salários permanecem os mais baixos.
    *   **Graduação/Bacharelado e Pós-graduação:** A progressão continua, mas as medianas tendem a ser superadas pelos níveis de mestrado e doutorado.
    *   **Mestrado:** Profissionais com mestrado e vasta experiência alcançam salários significativamente altos.
    *   **Doutorado ou Phd:** Este grupo, com alta experiência, apresenta as maiores medianas salariais e também uma dispersão muito grande, com outliers indicando salários excepcionalmente altos (alguns acima de R$40.000). A caixa para o maior nível de experiência em Doutorado é notavelmente alta.

**Interação entre Experiência e Nível de Ensino:**

*   **Benefício da Experiência é Universal:** A experiência aumenta o potencial salarial em todos os níveis de ensino.
*   **Nível de Ensino Potencializa o Efeito da Experiência:** O "retorno" da experiência parece ser maior para níveis de ensino mais altos. Ou seja, um ano adicional de experiência pode resultar em um aumento salarial proporcionalmente maior para quem tem mestrado ou doutorado em comparação com quem tem apenas graduação. Isso é visualizado pela inclinação mais acentuada da progressão salarial com a experiência nos níveis de ensino mais altos.
*   **Teto Salarial Mais Alto com Maior Escolaridade e Experiência:** Os salários mais altos no dataset (outliers superiores) são geralmente encontrados entre profissionais com níveis de ensino mais elevados (Mestrado, Doutorado) *e* mais tempo de experiência.

**Conclusões Gerais:**

Este gráfico é particularmente elucidativo ao mostrar que tanto a formação acadêmica quanto a experiência profissional são fatores cruciais na determinação salarial, e eles interagem de forma positiva.
*   Para alcançar os patamares salariais mais elevados na área de dados, a combinação de um alto nível de ensino (especialmente Mestrado ou Doutorado) com uma experiência profissional substancial parece ser o caminho mais promissor.
*   Enquanto a experiência por si só eleva os salários em todos os níveis de formação, o nível de formação parece definir diferentes "faixas" ou "tetos" potenciais de remuneração que são então explorados e alcançados através da experiência.


## Grafico Distribuição de Profissionais por Área de Formação Acadêmica
![distribuicao_area_formacao](https://github.com/user-attachments/assets/fd0d4cb9-5e30-4f52-8a7e-9cd074ee04c5)
## Análise do Gráfico: Distribuição de Profissionais por Área de Formação Acadêmica

O gráfico em anexo é um gráfico de barras horizontais que ilustra a "Distribuição de Profissionais por Área de Formação Acadêmica". Ele mostra a contagem de profissionais de dados provenientes de diferentes campos de estudo.

**Elementos do Gráfico:**

*   **Título:** "Distribuição de Profissionais por Área de Formação Acadêmica".
*   **Eixo Y (Vertical):** "Área de Formação". Lista as diversas áreas de formação acadêmica dos profissionais.
*   **Eixo X (Horizontal):** "Contagem". Indica o número de profissionais correspondente a cada área de formação, com a escala variando de 0 a mais de 1200.
*   **Barras Horizontais:** O comprimento de cada barra é proporcional à quantidade de profissionais com formação naquela área específica. As áreas estão ordenadas da maior para a menor contagem, de cima para baixo.

**Observações e Interpretações:**

1.  **Computação / Engenharia de Software / Sistemas de Informação/ TI:**
    *   Esta é, de longe, a área de formação mais comum entre os profissionais de dados no dataset, com uma contagem superior a 1200 profissionais. Isso indica uma forte predominância de backgrounds técnicos diretamente relacionados à computação e tecnologia da informação na área de dados.

2.  **Outras Engenharias:**
    *   A segunda área mais representativa, com aproximadamente 800 profissionais. Isso sugere que as habilidades analíticas e de resolução de problemas desenvolvidas em diversas engenharias são transferíveis e valorizadas no campo de dados.

3.  **Economia/ Administração / Contabilidade / Finanças/ Negócios:**
    *   Esta categoria ocupa a terceira posição, com cerca de 450 profissionais. Profissionais com formação em negócios e áreas correlatas trazem uma perspectiva de aplicação e valor de negócio para a análise de dados.

4.  **Estatística/ Matemática / Matemática Computacional/ Ciências Atuariais:**
    *   Com pouco mais de 200 profissionais, esta área, que possui fundamentos quantitativos essenciais para a ciência de dados, aparece em quarto lugar em termos de volume.

5.  **Outra opção:**
    *   Uma categoria genérica que agrupa formações não especificadas nas demais, com pouco menos de 200 profissionais.

6.  **Áreas Menos Representadas:**
    *   As demais áreas listadas apresentam contagens significativamente menores (abaixo de 100 profissionais cada):
        *   Química / Física
        *   Ciências Biológicas/ Farmácia/ Medicina/ Área da Saúde
        *   Marketing / Publicidade / Comunicação / Jornalismo
        *   Ciências Sociais
    *   Isso indica que, embora profissionais dessas áreas também atuem no campo de dados, eles representam uma parcela menor do total.

**Conclusões Gerais:**

*   **Predominância de Formações Técnicas e Quantitativas:** As áreas de Computação/TI, Engenharias e, em menor grau, Estatística/Matemática, dominam o cenário de formação dos profissionais de dados, o que é esperado dada a natureza técnica e analítica da área.
*   **Relevância de Formações em Negócios:** A presença significativa de profissionais com background em Economia, Administração e áreas afins destaca a importância do entendimento do contexto de negócios para a aplicação eficaz de técnicas de dados.
*   **Multidisciplinaridade Crescente, Mas Concentrada:** Embora a área de dados seja conhecida por sua multidisciplinaridade, este gráfico mostra que a maioria dos profissionais ainda provém de um conjunto relativamente concentrado de formações mais tradicionais para o setor de tecnologia e análise.
*   **Oportunidades para Diversas Formações:** A presença, mesmo que minoritária, de profissionais de áreas como Ciências Sociais, Saúde e Comunicação sugere que há espaço para diferentes perspectivas e habilidades no campo de dados, embora a transição possa ser menos comum ou exigir aquisição de habilidades técnicas adicionais.

Este gráfico oferece um panorama claro sobre as origens acadêmicas mais comuns dos profissionais que atualmente trabalham com dados, ressaltando a forte base em tecnologia e engenharias.


## Grafico Distribuição de Profissionais por Faixa Salarial Mensal
![distribuicao_faixa_salarial](https://github.com/user-attachments/assets/29688dff-55fd-492f-a897-ad9a4e89a657)
## Análise do Gráfico: Distribuição de Profissionais por Faixa Salarial Mensal

O gráfico apresentado é um gráfico de barras horizontais que ilustra a "Distribuição de Profissionais por Faixa Salarial Mensal". Ele mostra quantas pessoas se enquadram em cada faixa salarial.

**Elementos do Gráfico:**

*   **Título:** "Distribuição de Profissionais por Faixa Salarial Mensal".
*   **Eixo Y (Vertical):** "Faixa Salarial Mensal". Lista as diferentes faixas de salários mensais.
*   **Eixo X (Horizontal):** "Contagem". Indica o número de profissionais em cada faixa salarial, variando de 0 a 800.
*   **Barras Horizontais:** O comprimento de cada barra representa o número de profissionais naquela faixa salarial. As barras são organizadas verticalmente, com as faixas salariais mais baixas na parte superior e as mais altas na parte inferior.

**Observações e Interpretações:**

1.  **de R$8.001/mês a R$12.000/mês:**
    *   Esta é a faixa salarial com o maior número de profissionais, com uma contagem próxima a 800. Isso sugere que a maioria dos profissionais de dados no conjunto de dados ganha entre R$8.001 e R$12.000 por mês.

2.  **de R$12.001/mês a R$16.000/mês:**
    *   A segunda maior concentração está nesta faixa salarial, com uma contagem em torno de 400. Isso indica que muitos profissionais também ganham entre R$12.001 e R$16.000 por mês.

3.  **de R$6.001/mês a R$8.000/mês:**
    *   A terceira maior concentração está nesta faixa salarial, com uma contagem também em torno de 550.

4.  **de R$3.001/mês a R$4.000/mês:**
    *   A contagem é aproximadamente 300.

5.  **de R$4.001/mês a R$6.000/mês:**
    *   A contagem é aproximadamente 300.

6.  **de R$2.001/mês a R$3.000/mês:**
    *   A contagem é aproximadamente 200.

7.  **de R$1.001/mês a R$2.000/mês:**
    *   A contagem é pouco acima de 100.

8.  **Faixas Salariais Mais Altas (de R$16.001/mês a Acima de R$40.001/mês):**
    *   As faixas salariais mais altas apresentam contagens progressivamente menores. Isso indica que há menos profissionais ganhando salários mais elevados.
    *   As faixas de R$16.001/mês a R$20.000/mês e de R$20.001/mês a R$25.000/mês são as mais representadas entre as faixas salariais mais altas.

9.  **Menos de R$1.000/mês:**
    *   A menor contagem é para essa categoria, indicando que poucos profissionais ganham menos de R$1.000 por mês.

**Conclusões Gerais:**

*   **Concentração em Faixas Salariais Intermediárias:** A maioria dos profissionais de dados neste conjunto de dados se concentra nas faixas salariais entre R$6.001 e R$16.000 por mês.
*   **Distribuição Assimétrica:** A distribuição salarial é assimétrica, com uma cauda longa para a direita, indicando que, embora a maioria ganhe entre R$6.001 e R$16.000, alguns profissionais ganham significativamente mais.
*   **Minoria nas Faixas Mais Baixas:** Poucos profissionais relatam ganhar menos de R$2.000 por mês.

Este gráfico fornece uma visão geral da distribuição de salários entre os profissionais de dados, mostrando onde a maioria se concentra e como os salários se distribuem nas faixas mais altas e mais baixas.


## Grafico Distribuição de Profissionais por Nível de Ensino
![distribuicao_nivel_ensino](https://github.com/user-attachments/assets/044e5446-b6bd-474d-86d4-3c8a94ca44c7)
## Análise do Gráfico: Distribuição de Profissionais por Nível de Ensino

O gráfico anexado é um gráfico de barras horizontais que mostra a "Distribuição de Profissionais por Nível de Ensino". Ele quantifica o número de profissionais de dados em diferentes estágios de sua formação acadêmica.

**Elementos do Gráfico:**

*   **Título:** "Distribuição de Profissionais por Nível de Ensino".
*   **Eixo Y (Vertical):** "Nível de Ensino". Lista as categorias de escolaridade dos profissionais:
    *   Estudante de Graduação
    *   Graduação/Bacharelado
    *   Pós-graduação
    *   Mestrado
    *   Doutorado ou Phd
*   **Eixo X (Horizontal):** "Contagem". Indica o número de profissionais correspondente a cada nível de ensino, com a escala variando de 0 a 1200.
*   **Barras Horizontais:** O comprimento de cada barra é proporcional à quantidade de profissionais com aquele nível de ensino. As categorias estão ordenadas de cima para baixo, aparentemente refletindo uma progressão no nível educacional.

**Observações e Interpretações:**

1.  **Graduação/Bacharelado:**
    *   Esta é a categoria com o maior número de profissionais, ultrapassando a marca de 1200. Isso indica que a maioria dos profissionais de dados no dataset possui, no mínimo, um diploma de graduação completo.

2.  **Pós-graduação:**
    *   A segunda maior concentração de profissionais está neste nível, com uma contagem superior a 1000, mas inferior à da graduação (aproximadamente 1050). Este grupo inclui provavelmente especializações e MBAs (pós-graduação lato sensu).

3.  **Estudante de Graduação:**
    *   Este grupo representa a terceira maior contagem, com aproximadamente 450 profissionais. Isso mostra uma presença significativa de indivíduos que ainda estão cursando a graduação, mas já atuam na área de dados.

4.  **Mestrado:**
    *   Profissionais com mestrado (pós-graduação stricto sensu) somam cerca de 350, representando o quarto maior grupo.

5.  **Doutorado ou Phd:**
    *   Este é o grupo com a menor representatividade, com uma contagem de aproximadamente 100 profissionais. Embora seja o nível de ensino mais alto, é o menos comum entre os profissionais de dados no dataset.

**Conclusões Gerais:**

*   **Base Educacional Sólida:** A grande maioria dos profissionais de dados possui pelo menos uma graduação completa, com um número expressivo também tendo concluído algum tipo de pós-graduação (lato sensu ou stricto sensu).
*   **Entrada Precoce no Mercado:** A presença considerável de estudantes de graduação sugere que muitos iniciam suas carreiras na área de dados antes mesmo de concluir a formação universitária inicial.
*   **Funil Educacional:** Observa-se um afunilamento no número de profissionais à medida que o nível de ensino se torna mais avançado (Mestrado e, especialmente, Doutorado). Isso é comum em diversas áreas, refletindo o menor número de pessoas que prosseguem para os níveis mais altos de qualificação acadêmica.
*   **Valorização de Diferentes Níveis:** O gráfico demonstra que há profissionais de dados em todos os principais níveis de ensino, desde estudantes até doutores, indicando que o mercado absorve talentos com diferentes graus de formação.

Este gráfico oferece uma visão clara do perfil educacional dos profissionais de dados, destacando a importância da graduação e da pós-graduação, ao mesmo tempo que mostra a participação de estudantes e o menor, porém qualificado, contingente de mestres e doutores.


## Grafico Distribuição do Salário Estimado
![distribuicao_salario_estimado](https://github.com/user-attachments/assets/cb8d3675-ed41-4fcb-bf09-7f1c8b69cda4)
## Análise do Gráfico: Distribuição do Salário Estimado (R$)

O gráfico anexado é um histograma que representa a "Distribuição do Salário Estimado (R$)" dos profissionais de dados. Ele mostra a frequência de profissionais em diferentes intervalos de salário estimado.

**Elementos do Gráfico:**

*   **Título:** "Distribuição do Salário Estimado (R$)".
*   **Eixo Y (Vertical):** "Frequência". Indica o número de profissionais (contagem) para cada intervalo de salário. A escala vai de 0 a mais de 800.
*   **Eixo X (Horizontal):** "Salário Estimado (R$)". Representa os valores dos salários estimados em Reais, agrupados em intervalos (bins). A escala vai de R$0 a mais de R$40.000.
*   **Barras (Histograma):** A altura de cada barra corresponde à frequência (número de profissionais) cujo salário estimado cai dentro do intervalo (bin) que a barra representa.
*   **Linha Azul (Estimativa de Densidade do Kernel - KDE):** Sobreposta às barras, há uma linha curva suave que representa uma estimativa da função de densidade de probabilidade da distribuição dos salários. Ela ajuda a visualizar a forma geral da distribuição.

**Observações e Interpretações:**

1.  **Picos Principais (Modas):**
    *   O gráfico exibe uma distribuição multimodal, com pelo menos dois picos proeminentes.
    *   O primeiro pico, e o mais alto, ocorre na faixa salarial em torno de R$4.000 - R$6.000 (aproximadamente), onde a frequência ultrapassa 900 profissionais.
    *   O segundo pico significativo está na faixa de R$10.000 - R$12.000 (aproximadamente), com uma frequência em torno de 800 profissionais.
    *   Um terceiro pico menor, mas notável, aparece em torno de R$14.000 - R$16.000, com frequência próxima a 400.

2.  **Concentração de Salários:**
    *   A maioria dos profissionais parece se concentrar nas faixas salariais abaixo de R$16.000, com as maiores concentrações nos dois primeiros picos mencionados.

3.  **Cauda à Direita (Assimetria Positiva):**
    *   A distribuição é assimétrica à direita (ou positivamente assimétrica). Isso significa que, embora a maioria dos salários esteja concentrada nas faixas mais baixas e médias, há uma "cauda" de profissionais que recebem salários consideravelmente mais altos, estendendo-se para além de R$20.000, R$30.000 e até R$40.000. As frequências nessas faixas mais altas são progressivamente menores.

4.  **Intervalos de Salário:**
    *   A primeira barra, de R$0 a aproximadamente R$2.500, tem uma frequência em torno de 400.
    *   Após o pico principal em torno de R$5.000, há uma queda na frequência antes de subir novamente para o segundo pico em torno de R$11.000.
    *   Depois do terceiro pico em torno de R$15.000, as frequências diminuem consideravelmente, indicando que menos profissionais se encontram nas faixas salariais mais elevadas.

**Conclusões Gerais:**

*   **Distribuição Salarial Heterogênea:** A presença de múltiplos picos sugere que pode haver subgrupos distintos dentro da população de profissionais de dados com diferentes níveis salariais predominantes. Isso pode ser influenciado por fatores como nível de experiência, área de atuação, nível de ensino, região geográfica, etc.
*   **Maioria em Faixas Médias-Baixas:** Uma grande proporção dos profissionais aufere salários nas faixas que vão até aproximadamente R$16.000, com picos notáveis em torno de R$5.000 e R$11.000.
*   **Potencial para Altos Salários:** A cauda longa à direita indica que, embora menos comuns, existem salários significativamente altos na área de dados, ultrapassando R$40.000.
*   **Necessidade de Análise Multivariada:** A forma multimodal do histograma sugere que analisar apenas a distribuição geral do salário pode não contar a história completa. Seria interessante investigar quais fatores contribuem para os diferentes picos observados, como feito nas análises anteriores que segmentaram por experiência e nível de ensino.

Este histograma fornece uma visão geral da estrutura salarial dos profissionais de dados, destacando as faixas de remuneração mais comuns e a existência de um segmento com ganhos consideravelmente mais altos.


## Grafico Distribuição de Profissionais por Tempo de Experiência em Dados
![distribuicao_tempo_experiencia](https://github.com/user-attachments/assets/986f2138-2838-4ff8-ae15-8495f36f0728)
## Análise do Gráfico: Distribuição de Profissionais por Tempo de Experiência em Dados

O gráfico anexado é um gráfico de barras horizontais que ilustra a "Distribuição de Profissionais por Tempo de Experiência em Dados". Ele mostra o número de profissionais de dados classificados em diferentes faixas de tempo de experiência na área.

**Elementos do Gráfico:**

*   **Título:** "Distribuição de Profissionais por Tempo de Experiência em Dados".
*   **Eixo Y (Vertical):** "Tempo de Experiência". Apresenta as seguintes categorias de tempo de atuação profissional na área de dados:
    *   Menos de 1 ano
    *   de 1 a 2 anos
    *   de 3 a 4 anos
    *   de 5 a 6 anos
    *   de 7 a 10 anos
    *   Mais de 10 anos
*   **Eixo X (Horizontal):** "Contagem". Indica o número de profissionais correspondente a cada faixa de experiência, com a escala variando de 0 a mais de 1000.
*   **Barras Horizontais:** O comprimento de cada barra é proporcional à quantidade de profissionais naquela faixa de experiência específica. As barras estão ordenadas de cima para baixo, começando com a menor experiência e progredindo para a maior.

**Observações e Interpretações por Faixa de Experiência:**

1.  **de 1 a 2 anos:**
    *   Esta é a faixa com o maior número de profissionais, com uma contagem superior a 1000 (aproximadamente 1050-1100). Isso sugere que uma grande parcela dos profissionais de dados no dataset possui uma experiência relativamente inicial, mas já consolidada, na área.

2.  **de 3 a 4 anos:**
    *   A segunda maior concentração de profissionais está nesta faixa, com uma contagem próxima a 950. Juntamente com a faixa anterior, indica que a maioria dos profissionais tem entre 1 e 4 anos de experiência.

3.  **Menos de 1 ano:**
    *   Profissionais com menos de um ano de experiência representam o terceiro maior grupo, com uma contagem em torno de 400. Isso mostra um contingente significativo de recém-chegados à área.

4.  **de 5 a 6 anos:**
    *   A contagem de profissionais nesta faixa é de aproximadamente 250-280, indicando um número menor de profissionais com este nível de experiência intermediária mais longa.

5.  **de 7 a 10 anos:**
    *   Esta faixa possui uma contagem similar à anterior, em torno de 250-280 profissionais.

6.  **Mais de 10 anos:**
    *   Este é o grupo com a menor representatividade, com uma contagem visivelmente inferior às demais, parecendo ser inferior a 100 (talvez em torno de 50-80). Isso indica que profissionais com vasta experiência (mais de uma década) na área de dados são menos comuns no dataset, o que pode refletir a relativa novidade da área de "dados" como um campo formalizado ou a nomenclatura utilizada.

**Conclusões Gerais:**

*   **Concentração em Níveis Iniciais e Intermediários de Experiência:** A maioria dos profissionais de dados no dataset possui entre 1 e 4 anos de experiência, com um número também considerável de iniciantes (menos de 1 ano).
*   **Menor Representatividade de Profissionais Altamente Experientes:** Há um declínio no número de profissionais à medida que o tempo de experiência aumenta, sendo que aqueles com mais de 10 anos de experiência são os menos numerosos.
*   **Perfil da Área de Dados:** A distribuição pode sugerir que a área de dados, como campo profissional distinto, tem crescido rapidamente nos últimos anos, resultando em muitos profissionais com menos anos de experiência específica "em dados". Também pode indicar uma alta rotatividade ou transição para outras funções após alguns anos.
*   **Formato de Funil:** A distribuição se assemelha a um funil, onde muitos entram na área, mas o número de profissionais diminui nas faixas de experiência mais longas.

Este gráfico fornece uma visão clara do perfil de experiência dos profissionais de dados, destacando uma concentração maior nos estágios iniciais e intermediários da carreira na área.


## Grafico Top 10 UF de Residência dos Profissionais de Dados
![distribuicao_top10_uf](https://github.com/user-attachments/assets/1cf90782-fb39-475d-b70e-ac4b18bb3f7d)
## Análise do Gráfico: Top 10 UF de Residência dos Profissionais de Dados

O gráfico em anexo é um gráfico de barras verticais que apresenta o "Top 10 UF de Residência dos Profissionais de Dados". Ele mostra a contagem de profissionais de dados que residem nas dez Unidades Federativas (estados) com maior representatividade no dataset.

**Elementos do Gráfico:**

*   **Título:** "Top 10 UF de Residência dos Profissionais de Dados".
*   **Eixo Y (Vertical):** "Contagem". Indica o número de profissionais de dados, com a escala variando de 0 a mais de 1200.
*   **Eixo X (Horizontal):** "UF". Apresenta as siglas das Unidades Federativas. As UFs estão ordenadas da esquerda para a direita, da maior para a menor contagem de profissionais.
*   **Barras Verticais:** A altura de cada barra é proporcional ao número de profissionais de dados que residem naquela UF. As barras possuem diferentes tonalidades de azul, possivelmente para melhor distinção visual ou para indicar uma hierarquia, embora a ordenação já cumpra essa função.

**Observações e Interpretações por UF:**

1.  **SP (São Paulo):**
    *   Destaca-se como a UF com a maior concentração de profissionais de dados, com uma contagem muito superior às demais, ultrapassando 1200 (aproximadamente 1300 profissionais). Isso indica que São Paulo é o principal polo de profissionais de dados no Brasil, de acordo com este dataset.

2.  **MG (Minas Gerais):**
    *   A segunda UF com mais profissionais, com uma contagem em torno de 350-380. Embora seja um número significativo, é consideravelmente menor que o de São Paulo.

3.  **PR (Paraná):**
    *   Ocupa a terceira posição, com uma contagem próxima a 300 profissionais.

4.  **RJ (Rio de Janeiro):**
    *   Apresenta uma contagem muito similar à do Paraná, também em torno de 290-300 profissionais, posicionando-se como o quarto estado com mais profissionais de dados.

5.  **RS (Rio Grande do Sul):**
    *   A contagem de profissionais é de aproximadamente 180.

6.  **SC (Santa Catarina):**
    *   Possui uma contagem ligeiramente inferior ao RS, em torno de 160-170 profissionais.

7.  **DF (Distrito Federal):**
    *   Apresenta uma contagem próxima a 90-100 profissionais.

8.  **BA (Bahia), CE (Ceará), PE (Pernambuco):**
    *   Estas três UFs da região Nordeste encerram o top 10, com contagens menores e relativamente próximas entre si, todas abaixo de 100 (aproximadamente entre 70 e 85 profissionais cada).

**Conclusões Gerais:**

*   **Concentração Regional Sudeste-Sul:** A grande maioria dos profissionais de dados está concentrada na região Sudeste (SP, MG, RJ) e Sul (PR, RS, SC), com São Paulo liderando de forma proeminente.
*   **Disparidade Geográfica:** Existe uma notável disparidade na distribuição geográfica dos profissionais de dados, com um número muito maior de profissionais em São Paulo em comparação com todos os outros estados.
*   **Presença em Outras Regiões:** Embora em menor número, o Distrito Federal (Centro-Oeste) e estados do Nordeste (BA, CE, PE) também figuram no top 10, indicando a presença de polos de profissionais de dados nessas regiões, ainda que menos expressivos em volume.
*   **Implicações para o Mercado:** Essa concentração pode refletir onde estão as maiores oportunidades de emprego, os principais centros de formação ou os ecossistemas de inovação e tecnologia mais desenvolvidos no país.

Este gráfico fornece uma visão clara da distribuição geográfica dos profissionais de dados no Brasil, destacando a liderança de São Paulo e a importância das regiões Sudeste e Sul como principais centros para esses profissionais.


## Grafico Heatmap de Correlação entre Salário, Experiência e Nível de Ensino
![heatmap_correlacao_salario_exp_ensino](https://github.com/user-attachments/assets/2cd9887a-0a1d-4c89-b513-3a852d07b35c)
## Análise do Gráfico: Heatmap de Correlação entre Salário, Experiência (anos) e Nível de Ensino (ordinal)

O gráfico apresentado é um heatmap (mapa de calor) que visualiza a matriz de correlação entre três variáveis quantitativas: "Salário Estimado", "Experiência (anos) Estimados" e "Nível de Ensino (ordinal)". Este tipo de gráfico utiliza cores para representar a força e a direção das correlações lineares entre pares de variáveis.

**Elementos do Gráfico:**

*   **Título:** "Heatmap de Correlação entre Salário, Experiência (anos) e Nível de Ensino (ordinal)".
*   **Eixos (Linhas e Colunas):** As mesmas três variáveis são listadas tanto nas linhas quanto nas colunas:
    *   Salario_Estimado
    *   Experiencia_Anos_Estimados
    *   Nivel_Ensino_Ordinal
*   **Células da Matriz:** Cada célula na interseção de uma linha e uma coluna mostra o coeficiente de correlação de Pearson entre as duas variáveis correspondentes. O valor do coeficiente é exibido numericamente dentro da célula.
*   **Escala de Cores (Barra Lateral):** À direita do heatmap, uma barra de cores indica como os valores de correlação são mapeados para as cores. A escala varia de aproximadamente 0.2 (azul escuro) a 1.0 (vermelho escuro).
    *   Cores mais quentes (tendendo ao vermelho) indicam correlações positivas mais fortes.
    *   Cores mais frias (tendendo ao azul) indicam correlações positivas mais fracas (neste caso, todas as correlações são positivas).
    *   Se houvesse correlações negativas, elas normalmente seriam representadas por uma gama diferente de cores.

**Interpretação dos Coeficientes de Correlação:**

Os coeficientes de correlação variam de -1 a +1:
*   +1 indica uma correlação linear positiva perfeita.
*   -1 indica uma correlação linear negativa perfeita.
*   0 indica ausência de correlação linear.
*   Valores próximos de +1 ou -1 indicam correlações fortes, enquanto valores próximos de 0 indicam correlações fracas.

**Análise das Correlações Específicas:**

1.  **Diagonal Principal (Vermelho Escuro - Valor 1.00):**
    *   Salario_Estimado com Salario_Estimado: 1.00
    *   Experiencia_Anos_Estimados com Experiencia_Anos_Estimados: 1.00
    *   Nivel_Ensino_Ordinal com Nivel_Ensino_Ordinal: 1.00
    *   Isso é esperado, pois a correlação de qualquer variável consigo mesma é sempre perfeita e positiva.

2.  **Salario_Estimado vs. Experiencia_Anos_Estimados:**
    *   Coeficiente: 0.53
    *   Cor: Azul claro, tendendo para o centro da escala.
    *   Interpretação: Existe uma correlação positiva moderada entre o salário estimado e os anos de experiência. Isso sugere que, de forma geral, à medida que os anos de experiência aumentam, o salário estimado também tende a aumentar.

3.  **Salario_Estimado vs. Nivel_Ensino_Ordinal:**
    *   Coeficiente: 0.30
    *   Cor: Azul médio.
    *   Interpretação: Há uma correlação positiva fraca a moderada entre o salário estimado e o nível de ensino ordinal. Isso indica que, em geral, níveis de ensino mais altos estão associados a salários estimados mais altos, mas a relação é menos forte do que a observada com a experiência.

4.  **Experiencia_Anos_Estimados vs. Nivel_Ensino_Ordinal:**
    *   Coeficiente: 0.24
    *   Cor: Azul mais escuro, na parte inferior da escala de cores.
    *   Interpretação: Existe uma correlação positiva fraca entre os anos de experiência estimados e o nível de ensino ordinal. Isso pode sugerir uma leve tendência de que profissionais com níveis de ensino mais altos também possam ter um pouco mais de tempo de experiência, ou vice-versa, mas a relação é bastante tênue.

**Conclusões Gerais:**

*   **Influência da Experiência no Salário:** A experiência profissional ("Experiencia_Anos_Estimados") apresenta a correlação positiva mais forte com o salário ("Salario_Estimado") entre as variáveis analisadas (0.53), indicando que é um fator importante associado à remuneração.
*   **Influência do Nível de Ensino no Salário:** O nível de ensino ("Nivel_Ensino_Ordinal") também tem uma correlação positiva com o salário (0.30), mas essa relação é menos acentuada do que a da experiência.
*   **Relação entre Experiência e Nível de Ensino:** A correlação entre experiência e nível de ensino é a mais fraca entre os pares (0.24), sugerindo que esses dois fatores, embora ambos influenciem o salário, não estão fortemente interligados entre si no dataset.

Este heatmap fornece uma visão concisa de como essas três variáveis chave estão linearmente relacionadas, destacando a importância da experiência e, em menor grau, do nível de ensino, na determinação do salário estimado dos profissionais de dados.


## Grafico Salário Médio Estimado vs. Anos de Experiência por Nível de Ensino
![lineplot_salario_exp_por_nivel_ensino](https://github.com/user-attachments/assets/8e847b68-732a-4df6-ac5f-3abde32e4245)
## Análise do Gráfico: Salário Médio Estimado vs. Anos de Experiência por Nível de Ensino

O gráfico apresentado é um gráfico de linhas que ilustra a relação entre o "Salário Médio Estimado (R$)" e os "Anos de Experiência Estimados", segmentado por "Nível de Ensino". Cada linha representa um nível de formação acadêmica diferente, mostrando como a trajetória salarial se desenvolve com o aumento da experiência para cada grupo.

**Elementos do Gráfico:**

*   **Título:** "Salário Médio Estimado vs. Anos de Experiência por Nível de Ensino".
*   **Eixo Y (Vertical):** "Salário Médio Estimado (R$)", com a escala variando de R$2.500 a R$22.500.
*   **Eixo X (Horizontal):** "Anos de Experiência Estimados", variando de aproximadamente 0.5 (representando "Menos de 1 ano") até 8 anos (representando "de 7 a 10 anos", e possivelmente agrupando "Mais de 10 anos" no ponto final, embora a imagem corte antes de mostrar o extremo dos 10+ anos de forma explícita).
*   **Linhas Coloridas:** Cada linha representa um "Nível de Ensino" diferente, conforme a legenda:
    *   **Azul escuro/Roxo:** Estudante de Graduação
    *   **Azul médio:** Graduação/Bacharelado
    *   **Verde-azulado (Turquesa):** Pós-graduação
    *   **Verde:** Mestrado
    *   **Verde claro (Lima):** Doutorado ou Phd
*   **Pontos nas Linhas:** Marcam os valores médios de salário para faixas específicas de experiência dentro de cada nível de ensino.
*   **Áreas Sombreadas (Intervalos de Confiança):** As faixas coloridas translúcidas ao redor de cada linha provavelmente representam intervalos de confiança para o salário médio estimado. Isso indica a variabilidade ou incerteza em torno da média estimada; quanto mais larga a faixa, maior a incerteza ou dispersão dos dados.

**Observações e Interpretações:**

1.  **Progressão Salarial com Experiência (Geral):**
    *   Para *todos* os níveis de ensino, há uma clara tendência ascendente: o salário médio estimado aumenta consistentemente com o aumento dos anos de experiência. As linhas sobem da esquerda para a direita.

2.  **Impacto do Nível de Ensino no Salário Inicial (Ponto de Partida):**
    *   Mesmo com pouca ou nenhuma experiência (extrema esquerda do gráfico), os níveis de ensino mais altos tendem a começar com salários médios estimados mais elevados.
        *   "Doutorado ou Phd" e "Mestrado" iniciam com os maiores salários médios, seguidos por "Pós-graduação", "Graduação/Bacharelado", e por último "Estudante de Graduação".

3.  **Diferenças Salariais Ampliadas com a Experiência:**
    *   As linhas tendem a se divergir mais à medida que os anos de experiência aumentam. Isso significa que a diferença salarial entre os níveis de ensino se torna mais pronunciada para profissionais mais experientes.
    *   Por exemplo, a diferença salarial entre um "Doutorado ou Phd" e um "Graduado/Bacharel" com 1 ano de experiência é menor do que a diferença entre esses mesmos dois níveis com 5 ou 8 anos de experiência.

4.  **Hierarquia dos Níveis de Ensino:**
    *   Ao longo da maior parte da trajetória de experiência, a hierarquia salarial geralmente segue a ordem do nível de ensino: Doutorado > Mestrado > Pós-graduação > Graduação > Estudante de Graduação.
    *   Há um cruzamento ou proximidade muito grande entre as linhas de "Graduação/Bacharelado" e "Pós-graduação" em certos pontos, sugerindo que, para algumas faixas de experiência, a diferença salarial média entre ter apenas graduação e ter uma pós-graduação (lato sensu, provavelmente) pode não ser tão acentuada como a diferença para mestrado ou doutorado.

5.  **Retorno da Experiência por Nível de Ensino:**
    *   As inclinações das linhas sugerem que o "retorno" por ano adicional de experiência pode variar entre os níveis de ensino. As linhas para "Doutorado ou Phd" e "Mestrado" parecem ter inclinações consistentemente acentuadas, indicando um forte crescimento salarial com a experiência.

6.  **Variabilidade (Áreas Sombreadas):**
    *   As áreas sombreadas para "Doutorado ou Phd" e "Mestrado", especialmente nos níveis mais altos de experiência, parecem ser mais largas. Isso pode indicar uma maior variabilidade nos salários para esses grupos (ou seja, alguns doutores/mestres experientes ganham muito bem, enquanto outros podem ter salários mais próximos dos demais grupos, aumentando a dispersão) ou menor número de amostras nessas categorias, levando a maior incerteza na estimativa da média.
    *   A faixa para "Estudante de Graduação" é consistentemente a mais baixa e parece ter uma variabilidade relativamente menor em comparação com os níveis superiores.

**Conclusões Gerais:**

*   **Valorização da Experiência e Educação:** O gráfico demonstra claramente que tanto o tempo de experiência quanto o nível de ensino são fatores cruciais que influenciam positivamente o salário médio estimado dos profissionais de dados.
*   **Efeito Combinado:** O maior potencial salarial é observado em profissionais que combinam um alto nível de ensino (Mestrado ou Doutorado) com um volume significativo de anos de experiência.
*   **Investimento em Educação:** Níveis mais altos de educação formal tendem a proporcionar um ponto de partida salarial mais elevado e mantêm uma trajetória de crescimento salarial superior ao longo da carreira, em média.

Este gráfico sintetiza de forma eficaz como a formação acadêmica e a experiência profissional interagem para moldar a progressão salarial na área de dados, reforçando a importância de ambos os fatores para o desenvolvimento de carreira e potencial de ganhos.


## Grafico Relação 3D entre Salário, Experiência e Nível de Ensino
### [Grafico Interativo - Clique aqui](https://htmlpreview.github.io/?https://gist.githubusercontent.com/pedrinndias/c8f65f4a0c3ba1736c5a2687f8a7c448/raw/b83fdbae94c7706b5fbc5cd2215d132558201ddb/scatter3d_salario_exp_ensino.html)
![newplot(2)](https://github.com/user-attachments/assets/ec28770a-f3a3-4129-b517-f0fc40afd8f1)
## Análise do Gráfico: Relação 3D entre Salário, Experiência e Nível de Ensino

O gráfico interativo apresentado é um gráfico de dispersão 3D (3D Scatter Plot) que visualiza a relação entre três variáveis principais: "Salário Estimado (R$)", "Experiência (Anos Estimados)" e "Nível de Ensino (Ordinal)". Cada ponto no espaço tridimensional representa um profissional de dados.

**Elementos do Gráfico:**

*   **Eixos:**
    *   **Eixo X (Horizontal, profundidade):** "Experiencia_Anos_Estimados". Este eixo representa o tempo de experiência profissional em anos, variando de aproximadamente 0.5 (menos de 1 ano) até 10.0 (mais de 10 anos).
    *   **Eixo Y (Horizontal, largura):** "Nivel_Ensino_Ordinal". Este eixo representa o nível de formação acadêmica de forma ordinal, onde valores menores indicam níveis de ensino mais básicos (0 para Estudante de Graduação) e valores maiores indicam níveis mais avançados (4 para Doutorado ou Phd).
    *   **Eixo Z (Vertical, altura):** "Salario_Estimado". Este eixo representa a remuneração estimada em Reais, variando de R$0 até mais de R$40.000.
*   **Pontos de Dados:** Cada ponto (esfera) no gráfico representa um profissional individual no dataset, posicionado de acordo com seus valores nas três variáveis mencionadas.
*   **Cor dos Pontos (Nivel_Ensino_Ordinal):** Os pontos são coloridos de acordo com o "Nivel_Ensino_Ordinal", facilitando a identificação de grupos com diferentes níveis de formação. A legenda de cores normalmente acompanha esse tipo de gráfico (embora não visível estaticamente na imagem fornecida, é um padrão em gráficos interativos como os do Plotly):
    *   Estudante de Graduação (Ordinal 0): Cor específica (ex: azul)
    *   Graduação/Bacharelado (Ordinal 1): Outra cor (ex: laranja)
    *   Pós-graduação (Ordinal 2): Outra cor (ex: verde)
    *   Mestrado (Ordinal 3): Outra cor (ex: vermelho)
    *   Doutorado ou Phd (Ordinal 4): Outra cor (ex: roxo)

**Observações e Interpretações (Baseadas na Interação Típica com Gráficos 3D):**

1.  **Concentração de Pontos:**
    *   Observa-se uma maior concentração de pontos nas regiões de menor "Salario_Estimado", especialmente para níveis de ensino mais baixos e menor tempo de experiência.
    *   À medida que o "Nivel_Ensino_Ordinal" e a "Experiencia_Anos_Estimados" aumentam (movendo-se para "cima" no eixo Y e para "frente" no eixo X), os pontos tendem a se posicionar mais alto no eixo Z ("Salario_Estimado").

2.  **Tendência Geral:**
    *   Há uma tendência visual clara de que salários mais altos (pontos mais altos no eixo Z) estão associados a combinações de maior experiência e/ou níveis de ensino mais elevados.
    *   A "nuvem" de pontos parece se inclinar para cima à medida que se avança nos eixos de experiência e nível de ensino.

3.  **Impacto Combinado de Experiência e Nível de Ensino:**
    *   **Baixa Experiência, Qualquer Nível de Ensino:** Profissionais com pouca experiência (próximo ao plano traseiro do gráfico) geralmente apresentam salários mais baixos, mesmo aqueles com níveis de ensino mais altos (ex: Doutorado com pouca experiência pode ter salário menor que um Graduado com muita experiência).
    *   **Alta Experiência, Nível de Ensino Variado:** Profissionais com muita experiência (próximo ao plano frontal) mostram uma ampla gama de salários. No entanto, dentro desse grupo de alta experiência, aqueles com níveis de ensino mais altos (cores associadas a Mestrado/Doutorado) tendem a alcançar os patamares salariais mais elevados.
    *   **Nível de Ensino Alto, Experiência Variada:** Profissionais com Doutorado (cor específica, ordinal 4), por exemplo, estão espalhados ao longo do eixo de experiência. Aqueles com mais experiência nesse grupo tendem a ter os salários mais altos do dataset.

4.  **Visualização de Outliers:**
    *   O gráfico 3D permite identificar visualmente outliers – profissionais que, por exemplo, têm um salário muito alto para seu nível de experiência e ensino, ou vice-versa. Esses pontos se destacariam da "nuvem" principal.

5.  **Interatividade:**
    *   A natureza interativa desses gráficos (possibilidade de girar, dar zoom) é crucial para uma exploração completa. Girar o gráfico permite observar a relação entre pares de variáveis, mantendo a terceira como referência, ou identificar clusters e padrões que não seriam óbvios em visualizações 2D separadas.

**Conclusões Gerais:**

*   O gráfico de dispersão 3D reforça as conclusões de análises 2D anteriores: tanto a experiência profissional quanto o nível de formação acadêmica são fatores importantes que influenciam positivamente o salário estimado dos profissionais de dados.
*   A visualização tridimensional destaca a **interação** entre esses dois fatores. Para alcançar os salários mais altos, geralmente é necessária uma combinação de alto nível de ensino *e* experiência substancial.
*   Profissionais com níveis de ensino mais baixos, mesmo com muita experiência, podem ter um "teto" salarial inferior ao de profissionais com formação mais avançada e experiência similar.
*   Da mesma forma, profissionais com alta formação, mas pouca experiência, podem não atingir os salários mais elevados até que acumulem mais tempo de atuação no mercado.

Este tipo de visualização é poderoso para entender relações multivariadas complexas, mostrando como diferentes fatores se combinam para influenciar um resultado, neste caso, o salário.


## Grafico Salário Estimado vs. Proporção de Docentes com Doutorado na UF de Residência
![scatterplot_salario_vs_prop_doc_doutorado_uf](https://github.com/user-attachments/assets/004cf9f3-3691-4536-aa8a-ae2a9ec938e9)
## Análise do Gráfico: Salário Estimado vs. Proporção de Docentes com Doutorado na UF de Residência

O gráfico apresentado é um gráfico de dispersão (scatter plot) que busca explorar a relação entre o "Salário Estimado (R$)" dos profissionais de dados e a "Proporção de Docentes com Doutorado na UF de Residência". Adicionalmente, os pontos no gráfico são codificados por cor para representar o "Nível de ensino alcançado" e por tamanho para indicar os "Experiencia_Anos_Estimados".

**Elementos do Gráfico:**

*   **Título:** "Salário Estimado vs. Proporção de Docentes com Doutorado na UF de Residência".
*   **Eixo Y (Vertical):** "Salário Estimado (R$)", com escala de R$0 até mais de R$40.000.
*   **Eixo X (Horizontal):** "Proporção de Docentes com Doutorado na UF de Residência", variando aproximadamente de 0.30 a pouco mais de 0.60. Este eixo representa a fração de docentes em uma determinada Unidade Federativa que possuem doutorado.
*   **Pontos de Dados:** Cada ponto representa um profissional de dados.
    *   **Cor (Nível de ensino alcançado):** Conforme a legenda:
        *   Verde claro/Turquesa: Estudante de Graduação
        *   Laranja: Graduação/Bacharelado
        *   Azul: Pós-graduação
        *   Roxo/Rosa: Mestrado
        *   Verde escuro: Doutorado ou Phd
    *   **Tamanho (Experiencia_Anos_Estimados):** Pontos maiores indicam maior tempo de experiência (0.5, 1.5, 3.5, 5.5, 8.5 anos estimados), conforme a legenda.

**Observações e Interpretações:**

1.  **Dispersão Geral dos Pontos:**
    *   Os pontos estão amplamente dispersos pelo gráfico, não formando um padrão linear claro (positivo ou negativo) entre a proporção de docentes com doutorado na UF e o salário estimado dos profissionais de dados.
    *   Isso sugere que, isoladamente, a proporção de docentes com doutorado em uma UF não parece ser um forte preditor direto do salário individual de um profissional de dados que reside naquela UF.

2.  **Distribuição Salarial:**
    *   Profissionais com salários muito variados (desde próximos a R$0 até acima de R$40.000) são encontrados em UFs com diferentes proporções de docentes com doutorado. Por exemplo, tanto em UFs com proporção em torno de 0.45 quanto em UFs com proporção em torno de 0.55, observa-se toda a gama de salários.

3.  **Impacto do Nível de Ensino (Cor):**
    *   **Estudantes de Graduação (Verde claro/Turquesa):** Concentram-se predominantemente nas faixas salariais mais baixas, independentemente da proporção de docentes com doutorado na UF.
    *   **Outros Níveis de Ensino:** Profissionais com Graduação (Laranja), Pós-graduação (Azul), Mestrado (Roxo/Rosa) e Doutorado (Verde escuro) estão espalhados por uma ampla faixa de salários. Os salários mais altos (acima de R$30.000) são alcançados por profissionais de diversos níveis de ensino a partir da graduação, mas frequentemente associados a maior experiência.

4.  **Impacto da Experiência (Tamanho):**
    *   Visualmente, os pontos maiores (mais experiência) tendem a se localizar nas faixas salariais mais altas. Por exemplo, muitos dos pontos com salários acima de R$20.000 são de tamanho médio a grande. Isso reforça a observação de análises anteriores de que a experiência é um fator importante na determinação salarial.
    *   Os salários mais elevados (acima de R$40.000) são consistentemente representados por pontos de tamanho médio a grande, indicando profissionais com experiência considerável (3.5 anos ou mais).

5.  **Ausência de Relação Clara com a Proporção de Docentes com Doutorado:**
    *   Não se observa que UFs com maior proporção de docentes com doutorado tenham consistentemente profissionais de dados com salários mais altos, ou vice-versa.
    *   Por exemplo, alguns dos salários mais altos (>R$40.000) aparecem em UFs com proporção de docentes com doutorado em torno de 0.45-0.50, enquanto outros salários altos também aparecem em UFs com proporção em torno de 0.55-0.60.

**Conclusões Gerais:**

*   O gráfico sugere que a proporção de docentes com doutorado na UF de residência de um profissional de dados **não é um fator determinante primário** para o salário estimado desse profissional. A qualidade do ambiente acadêmico local, se proxy pela qualificação dos docentes, não se traduz diretamente em maiores salários individuais para os profissionais de dados ali residentes.
*   Fatores individuais como **nível de ensino alcançado e, principalmente, anos de experiência**, parecem ter uma influência mais visível na determinação salarial, como indicado pela distribuição das cores e tamanhos dos pontos em relação ao eixo do salário.
*   Outros fatores não representados neste gráfico específico, como o setor de atuação da empresa, o cargo específico, as habilidades individuais, a demanda do mercado local na UF e o custo de vida, provavelmente desempenham papéis mais significativos na definição dos salários dos profissionais de dados.

Este gráfico é útil para descartar uma relação causal ou correlacional forte entre a proporção de docentes com doutorado na UF e os salários dos profissionais de dados, direcionando a atenção para outros fatores mais diretamente ligados ao perfil do profissional e ao mercado de trabalho.


## Gráfico Relação 3D entre Salário, Experiência e Nível de Ensino
### [Grafico Interativo - Clique aqui](https://htmlpreview.github.io/?https://gist.githubusercontent.com/pedrinndias/6bdfb7fdb2be6a819758ca7b1b05d011/raw/7db0af70c340fb3c01d6a052579873f03cacbf1c/gistfile1.txt)
![newplot(3)](https://github.com/user-attachments/assets/6ebf06b9-3667-4d2f-bb06-2802e19b8949)
## Análise do Gráfico: Relação 3D entre Salário, Experiência e Nível de Ensino

O gráfico interativo apresentado é um gráfico de dispersão 3D (3D Scatter Plot) que visualiza a relação entre três variáveis principais: "Salário Estimado (R$)", "Experiência (Anos Estimados)" e "Nível de Ensino (Ordinal)". Cada ponto no espaço tridimensional representa um profissional de dados. Este tipo de análise exploratória de dados (AED) ajuda a investigar conjuntos de dados e resumir suas principais características usando métodos de visualização.

**Elementos do Gráfico:**

*   **Eixos:**
    *   **Eixo X (Horizontal, geralmente representado como profundidade ou eixo frontal):** "Experiencia_Anos_Estimados". Este eixo representa o tempo de experiência profissional em anos, variando de aproximadamente 0.5 (para "Menos de 1 ano") até 10.0 (para "Mais de 10 anos").
    *   **Eixo Y (Horizontal, geralmente representado como largura ou eixo lateral):** "Nivel_Ensino_Ordinal". Este eixo representa o nível de formação acadêmica de forma ordinal, onde valores menores indicam níveis de ensino mais básicos (0 para Estudante de Graduação) e valores maiores indicam níveis mais avançados (4 para Doutorado ou Phd).
    *   **Eixo Z (Vertical, altura):** "Salario_Estimado". Este eixo representa a remuneração estimada em Reais, variando de R$0 até valores que podem exceder R$40.000.
*   **Pontos de Dados:** Cada ponto (esfera) no gráfico representa um profissional individual no dataset, posicionado de acordo com seus valores nas três variáveis mencionadas.
*   **Cor dos Pontos (Nivel_Ensino_Ordinal):** Os pontos são coloridos de acordo com o "Nivel_Ensino_Ordinal", o que facilita a identificação visual de grupos com diferentes níveis de formação acadêmica. A legenda de cores, que tipicamente acompanha esses gráficos interativos, seria (assumindo um esquema de cores padrão para variáveis ordinais):
    *   Estudante de Graduação (Ordinal 0): Uma cor específica (ex: azul)
    *   Graduação/Bacharelado (Ordinal 1): Outra cor (ex: laranja)
    *   Pós-graduação (Ordinal 2): Outra cor (ex: verde)
    *   Mestrado (Ordinal 3): Outra cor (ex: vermelho)
    *   Doutorado ou Phd (Ordinal 4): Outra cor (ex: roxo)

**Observações e Interpretações (Baseadas na Interação Típica com Gráficos 3D):**

1.  **Concentração Geral dos Pontos:**
    *   Observa-se uma maior densidade de pontos nas regiões correspondentes a menores salários estimados (parte inferior do eixo Z), especialmente para combinações de baixo nível de ensino e pouco tempo de experiência.
    *   À medida que os valores nos eixos "Nivel_Ensino_Ordinal" e "Experiencia_Anos_Estimados" aumentam (movendo-se para valores ordinais mais altos no eixo Y e para mais anos no eixo X), os pontos tendem a se posicionar em níveis mais elevados no eixo Z ("Salario_Estimado").

2.  **Tendência Global:**
    *   Visualmente, existe uma tendência clara de que salários mais altos (pontos mais altos no eixo Z) estão associados a combinações de maior tempo de experiência e/ou níveis de ensino mais elevados. A "nuvem" de pontos parece se elevar à medida que se avança ao longo dos eixos de experiência e nível de ensino.

3.  **Impacto Combinado e Interação entre Experiência e Nível de Ensino:**
    *   **Profissionais com Baixa Experiência:** Independentemente do nível de ensino, aqueles com pouca experiência (valores baixos no eixo X) geralmente apresentam salários mais baixos. Mesmo um doutor com pouca experiência pode ter um salário menor do que um graduado com muitos anos de experiência.
    *   **Profissionais com Alta Experiência:** Aqueles com muitos anos de experiência (valores altos no eixo X) exibem uma gama mais ampla de salários. Dentro deste grupo, os profissionais com níveis de ensino mais altos (cores associadas a Mestrado/Doutorado) tendem a alcançar os patamares salariais mais elevados.
    *   **Profissionais com Nível de Ensino Elevado:** Por exemplo, indivíduos com Doutorado (ordinal 4, cor específica) estão distribuídos ao longo de diferentes faixas de experiência. Aqueles que combinam doutorado com mais anos de experiência tendem a estar entre os que recebem os salários mais altos do dataset.

4.  **Identificação de Outliers:**
    *   A visualização 3D pode ajudar a identificar outliers – por exemplo, profissionais com um salário muito alto para seu nível de experiência e ensino, ou o contrário. Esses pontos se destacariam da concentração principal de dados.

5.  **Vantagem da Interatividade:**
    *   A capacidade de girar, dar zoom e interagir com o gráfico 3D é fundamental para uma análise completa. Isso permite observar as relações entre pares de variáveis de diferentes ângulos, facilitando a identificação de padrões, clusters ou tendências que poderiam não ser evidentes em gráficos 2D estáticos.

**Conclusões Gerais:**

*   O gráfico de dispersão 3D corrobora e integra as descobertas de análises 2D anteriores: tanto a experiência profissional quanto o nível de formação acadêmica são fatores positivamente correlacionados com o salário estimado dos profissionais de dados.
*   A principal contribuição desta visualização é destacar a **interação** entre esses dois fatores. Para alcançar os salários mais elevados, geralmente é necessária uma combinação de um alto nível de ensino *e* uma experiência profissional substancial.
*   Profissionais com níveis de ensino mais baixos podem encontrar um "teto" salarial mais baixo, mesmo com muita experiência, em comparação com aqueles com formação mais avançada e experiência similar.
*   Da mesma forma, profissionais com alta qualificação acadêmica, mas pouca experiência prática, podem não atingir os salários mais altos até acumularem mais tempo de atuação no mercado.

Este tipo de gráfico é uma ferramenta poderosa para a análise exploratória de dados (AED), pois permite uma compreensão mais intuitiva de relações multivariadas complexas, mostrando como diferentes fatores se combinam para influenciar um resultado específico como o salário.


-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

# Indução de modelos

*   [1º Pergunta orientada a dados ](#modelos-1º-pergunta-orietada-a-dados)
  
	*   [Modelo 1 Análise de Disparidade Salarial de Profissionais de Dados no Brasil Utilizando o Modelo Random Forest](#modelo-1-análise-de-disparidade-salarial-de-profissionais-de-dados-no-brasil-utilizando-o-modelo-random-forest)
  
		*   [Justificativa1.1](#justificativa1-1)
		*   [Processo de Amostragem de Dados (Particionamento e Cross-Validation1.1)](#processo-de-amostragem-de-dados1-1)
		*   [Parâmetros utilizados1.1](#parâmetros-utilizados1-1)
		*   [Explicação do Código1.1](#explicação-do-código1-1)

	*   [Modelo 2 Análise de Disparidade Salarial de Profissionais de Dados no Brasil Utilizando o Arvore de decisão por classificação](#modelo-1-análise-de-disparidade-salarial-de-profissionais-de-dados-no-brasil-utilizando-o-arvore-de-decisão-por-classificação)
  
		*   [Justificativa1.2](#justificativa1-2)
		*   [Processo de Amostragem de Dados (Particionamento e Cross-Validation1.2)](#processo-de-amostragem-de-dados1-2)
		*   [Parâmetros utilizados1.2](#parâmetros-utilizados1-2)
		*   [Explicação do Código1.2](#explicação-do-código1-2)


# Modelos 1º pergunta orietada a dados

## Modelo 1 Análise de Disparidade Salarial de Profissionais de Dados no Brasil Utilizando o Modelo Random Forest

## *Justificativa1-1*

O modelo `RandomForestClassifier` é uma boa escolha para sua pergunta porque ele consegue identificar como diferentes fatores, como educação e experiência, interagem e qual a importância de cada um para explicar as diferenças salariais.

### Capacidade Inerente de Modelar Interações Complexas 🧩
A pergunta foca explicitamente na **interação** entre formação e experiência. Modelos baseados em árvores, como o Random Forest, são excelentes em capturar automaticamente interações não lineares entre features. Cada caminho da raiz até uma folha em uma árvore de decisão representa uma sequência de condições, que é, em essência, uma regra de interação. Por exemplo, o impacto da "experiência profissional" no salário pode ser diferente para quem tem "doutorado" versus quem tem apenas "graduação". O Random Forest, ao agregar centenas de árvores, explora inúmeras dessas interações potenciais. O notebook até inclui uma visualização específica (`interacao_formacao_experiencia.png`) que tenta mostrar a probabilidade de salário alto com base na combinação de níveis de formação e experiência, demonstrando a capacidade do modelo de aprender e representar essas interações.

---
### Identificação dos Fatores Mais Influentes (Importância das Features) 📊
Para entender como diferentes fatores influenciam a disparidade salarial, é crucial saber quais são os mais determinantes. O Random Forest fornece uma métrica de "importância das features", que quantifica a contribuição de cada variável (como 'Nível de ensino alcançado', 'Tempo de experiência na área de dados', 'Nível de senioridade', 'UF onde mora', etc.) para a precisão da previsão. O notebook demonstra a extração e visualização dessas importâncias, permitindo identificar os principais direcionadores da disparidade salarial.

---
### Flexibilidade para Modelar Relações Não Lineares 📈
A relação entre fatores socioeconômicos e salário raramente é linear. Por exemplo, o aumento salarial com a experiência pode não ser constante, ou o benefício de um diploma adicional pode variar dependendo do nível de senioridade atual. O Random Forest não assume relações lineares e pode modelar essas complexidades de forma eficaz.

---
### Robustez e Desempenho Geral 🚀
Random Forests são conhecidos por sua **robustez** a outliers (em certa medida) e por seu **bom desempenho preditivo** em uma ampla gama de problemas de classificação sem a necessidade de um ajuste extensivo de hiperparâmetros (embora o tuning, como feito no notebook via `GridSearchCV`, geralmente melhore ainda mais o desempenho). A capacidade de lidar com diferentes tipos de features (numéricas e categóricas codificadas) e a menor propensão a overfitting em comparação com árvores de decisão únicas também são vantagens significativas.

---
### Adequação à Definição do Problema no Notebook 🎯
No notebook fornecido, a "disparidade salarial" foi transformada em um problema de **classificação binária** (salário alto vs. salário baixo/médio). O `RandomForestClassifier` é projetado especificamente para esse tipo de tarefa. Além disso, o código implementa:
* **Engenharia de features** relevante (mapeamento de níveis de formação, experiência, etc.).
* **Tratamento de classes desbalanceadas** (usando `sample_weights` e `class_weight`), o que é comum em dados salariais.
* **Calibração de probabilidades** e **otimização de limiar**, levando a um modelo mais confiável e ajustado ao problema.

---
## - Capacidade de Capturar Interações Complexas:

### Como as Árvores de Decisão (Base do Random Forest) Capturam Interações

* **Natureza Hierárquica e Condicional**:
    * Uma árvore de decisão funciona dividindo o espaço das features em regiões menores através de uma série de **decisões condicionais (splits)**.
    * O caminho de uma amostra de dados da raiz até uma folha (nó terminal) representa uma **sequência específica de condições** sobre diferentes features.
    * Por exemplo, uma árvore pode aprender que "SE `Nível de senioridade` é 'Sênior' E `Tempo de experiência na área de dados` é 'Mais de 10 anos', ENTÃO a probabilidade de `salario_alto` é X". Esta é uma interação direta entre `Nível de senioridade` e `Tempo de experiência`. O efeito da experiência no salário pode ser diferente para um júnior versus um sênior.

* **Profundidade da Árvore**:
    * Árvores mais profundas (controladas por `max_depth`, `min_samples_split`, `min_samples_leaf`) podem capturar interações de ordem superior (interações entre três ou mais features). No modelo otimizado, `max_depth` foi definido como `None`, permitindo que as árvores cresçam até que os critérios de `min_samples_leaf: 7` e `min_samples_split: 15` sejam atingidos. Isso dá flexibilidade para capturar interações significativas.

---

### Como o Random Forest (Ensemble) Amplifica essa Capacidade

* **Múltiplas Perspectivas**:
    * O Random Forest constrói **muitas árvores de decisão** (100 neste caso), cada uma treinada em uma subamostra diferente dos dados (bootstrap) e considerando um subconjunto aleatório de features em cada divisão.
    * Isso significa que diferentes árvores terão a oportunidade de explorar e modelar **diferentes interações** ou as mesmas interações de maneiras ligeiramente diferentes. Algumas árvores podem priorizar certas interações, enquanto outras focam em combinações distintas.

* **Agregação de Conhecimento**:
    * A previsão final do Random Forest é uma agregação (média de probabilidades para classificação) das previsões de todas as árvores individuais.
    * Ao combinar o "conhecimento" de muitas árvores que aprenderam diversas interações, o ensemble se torna capaz de representar um **panorama de interações muito mais rico e robusto** do que uma única árvore conseguiria.

---

### Evidências e Suporte no Código do Notebook

* **Visualização de Interação Específica**:
    * O notebook inclui uma "Análise de Interação entre Formação e Experiência" que gera um heatmap (`interacao_formacao_experiencia.png`). Este gráfico mostra a probabilidade média de `salario_alto` para diferentes combinações de `formacao_academica_encoded` e `experiencia_profissional_encoded`.
    * O fato de o modelo conseguir gerar previsões que resultam em um padrão claro neste heatmap (por exemplo, mostrando que a combinação de alta formação E alta experiência leva a uma maior probabilidade de salário alto) é uma **demonstração direta** de que o modelo está capturando e utilizando essa interação específica.

* **Engenharia de Features**:
    * A codificação one-hot de features como `'Área de formação acadêmica'`, `'UF onde mora'`, e `'Setor de atuação da empresa'` cria colunas binárias. O modelo pode então aprender, por exemplo, se o impacto do `'Tempo de experiência na área de dados'` no salário é diferente para `'UF onde mora_São Paulo'` versus `'UF onde mora_Bahia'`.

* **Desempenho Geral do Modelo**:
    * Um bom desempenho em um problema complexo como a previsão salarial, que intuitivamente depende de como múltiplos fatores se combinam, sugere que o modelo está efetivamente capturando não apenas os efeitos principais das features, mas também suas interações. Se o modelo não conseguisse capturar essas interações, seu poder preditivo seria provavelmente muito menor.

Em resumo, a estrutura baseada em árvores do Random Forest, combinada com a diversidade introduzida pelo bagging e pela amostragem aleatória de features, permite que o modelo aprenda e utilize automaticamente as interações complexas e não lineares entre as variáveis preditoras, o que é fundamental para sua eficácia em muitos problemas do mundo real.

---
## - Fornecimento de Importância das Features:

### Como o Random Forest Calcula a Importância das Features

* **Redução Média da Impureza (Mean Decrease in Impurity - MDI)**:
    * O método mais comum, e o padrão no Scikit-learn para `RandomForestClassifier`, é baseado na **impureza de Gini** (ou entropia, dependendo da configuração do critério da árvore).
    * Quando uma árvore de decisão é construída, cada divisão de um nó é feita escolhendo a feature que resulta na maior redução da impureza (ou seja, que torna os nós filhos mais "puros" em termos de classes).
    * A importância de uma feature é calculada como a **média da redução da impureza** que ela proporciona em todas as árvores da floresta. Quanto mais uma feature contribui para reduzir a impureza nos nós onde é utilizada para divisão, maior será sua importância.
    * As importâncias são então normalizadas para que a soma de todas as importâncias seja igual a 1.

---

### Implementação no Código do Notebook

O notebook extrai e utiliza a importância das features da seguinte maneira:

1.  **Extração dos Valores de Importância**:
    * Após o treinamento e a otimização do `RandomForestClassifier` (armazenado em `best_rf_model`), os valores de importância são acessados diretamente através do atributo:
        ```python
        importances = best_rf_model.feature_importances_
        ```
    * Os nomes das features correspondentes são obtidos a partir das colunas do DataFrame `X`:
        ```python
        feature_names = X.columns
        ```

2.  **Ordenação e Seleção**:
    * As importâncias são ordenadas em ordem decrescente para identificar as features mais relevantes:
        ```python
        indices = np.argsort(importances)[::-1]
        ```

3.  **Visualização da Importância das Features**:
    * O código gera múltiplos gráficos para visualizar essas importâncias, facilitando a interpretação:
        * **Top 20 Features Mais Relevantes**: Um gráfico de barras horizontais mostrando as 20 features com maior pontuação de importância (`importancia_features_top20.png`).
        * **Importância Agrupada por Prefixo**: Se houver muitas features (especialmente após o one-hot encoding), gráficos de barras separados são criados para grupos de features com o mesmo prefixo (ex: "UF onde mora\_", "Área de formação acadêmica\_") para melhor organização (`importancia_features_grupo_*.png`).
        * **Top 3 Features Mais Importantes**: Um gráfico de barras focado nas três features de maior impacto, com os valores de importância anotados (`top3_features.png`).
        * **Gráfico de Dispersão das Duas Features Mais Importantes**: Visualiza a relação entre as duas features mais importantes e a probabilidade de salário alto (`dispersao_top2_features.png`).

---

### Valor da Análise de Importância das Features

Conhecer a importância das features é extremamente útil por diversos motivos:

* **Interpretabilidade do Modelo**: Ajuda a entender quais fatores o modelo considera mais decisivos para fazer suas previsões. No contexto do problema, revela quais aspectos (como nível de ensino, experiência, senioridade, etc.) são mais determinantes para a faixa salarial.
* **Seleção de Features (Feature Selection)**:
    * Features com importância muito baixa podem, em alguns casos, ser removidas do modelo sem grande perda de performance (ou até mesmo com ganho, ao reduzir ruído e complexidade).
    * Isso pode levar a modelos mais simples, mais rápidos de treinar e, potencialmente, mais generalizáveis.
* **Direcionamento de Negócios e Pesquisas**:
    * As features mais importantes podem indicar áreas onde intervenções ou foco podem ser mais eficazes. Por exemplo, se "Nível de ensino alcançado" é muito importante, isso reforça o valor da educação para progressão salarial.
* **Detecção de Problemas (Sanity Check)**: Se uma feature que intuitivamente não deveria ser importante aparece com alta relevância, isso pode indicar problemas nos dados (vazamento de dados - data leakage) ou na formulação do problema.
* **Comunicação dos Resultados**: É mais fácil explicar o comportamento de um modelo para stakeholders não técnicos destacando as poucas variáveis que têm o maior impacto.

A análise de importância das features fornecida pelo Random Forest é, portanto, uma etapa crucial não apenas para avaliar o modelo, mas também para extrair insights acionáveis a partir dos dados.

---
## - Robustez e Generalização:

### Robustez do Modelo 💪

A robustez refere-se à capacidade do modelo de manter seu desempenho mesmo diante de variações nos dados de entrada, como ruído ou outliers.

* **Natureza de Ensemble (Bagging)**:
    * O Random Forest constrói múltiplas árvores de decisão (100 neste modelo). Cada árvore é treinada em uma subamostra diferente dos dados (bootstrap).
    * Ao agregar as previsões de muitas árvores, o impacto de **outliers** ou **ruído** que possam ter afetado uma ou algumas árvores é diluído. Uma única árvore pode ser sensível a esses pontos, mas é menos provável que a maioria das árvores seja influenciada da mesma maneira.

* **Aleatoriedade na Seleção de Features**:
    * Em cada divisão de nó de cada árvore, apenas um subconjunto aleatório de features é considerado. Isso **descorrelaciona as árvores** e impede que features individualmente muito fortes (mas possivelmente ruidosas ou específicas demais para a amostra de treino) dominem a construção de todas as árvores. Isso torna o modelo menos sensível a pequenas variações nas features individuais.

* **Controle da Complexidade das Árvores**:
    * Os hiperparâmetros otimizados `min_samples_split: 15` e `min_samples_leaf: 7` restringem o crescimento das árvores. Eles evitam que as árvores se tornem excessivamente complexas e se ajustem ao ruído presente nos dados de treinamento. Árvores mais simples e robustas contribuem para uma floresta mais robusta.

* **Tratamento de Desbalanceamento de Classes**:
    * O uso de `class_weight='balanced_subsample'` e `sample_weights` torna o modelo robusto a distribuições de classe desiguais. Sem isso, o modelo poderia simplesmente aprender a prever a classe majoritária, mostrando um desempenho pobre e não robusto quando confrontado com diferentes proporções de classe ou com a importância da classe minoritária.

---

### Generalização do Modelo 🌍

A generalização é a capacidade do modelo de performar bem em dados novos e não vistos, após ter sido treinado em um conjunto de dados específico. É o objetivo principal do aprendizado de máquina.

* **Redução de Variância pelo Bagging**:
    * A principal vantagem do bagging (usado no Random Forest) é a **redução da variância** do modelo sem aumentar significativamente o bias. Modelos com alta variância tendem a se ajustar demais aos dados de treinamento (overfitting) e generalizam mal. Ao agregar múltiplas árvores, o Random Forest suaviza as previsões e melhora a generalização.

* **Validação Cruzada (`GridSearchCV` e `CalibratedClassifierCV`)**:
    * O uso de validação cruzada de **5 folds** tanto no `GridSearchCV` (para otimização de hiperparâmetros) quanto no `CalibratedClassifierCV` (para calibração) é fundamental para a generalização.
    * Nesses processos, o modelo é treinado e avaliado múltiplas vezes em diferentes subconjuntos dos dados de treinamento. Isso ajuda a garantir que os hiperparâmetros selecionados e o processo de calibração sejam eficazes não apenas para uma divisão específica dos dados, mas que **generalizem bem** para porções não vistas do conjunto de treinamento.

* **Divisão em Conjunto de Treino e Teste**:
    * A separação inicial dos dados em conjuntos de treino (70%) e teste (30%) é a prática padrão para avaliar a generalização. O modelo é treinado exclusivamente nos dados de treino, e seu desempenho final no conjunto de teste (dados que o modelo nunca viu durante o treinamento, otimização ou calibração) é uma estimativa de quão bem ele generalizará para dados do mundo real.

* **Otimização de Hiperparâmetros Focada em Generalização**:
    * Parâmetros como `min_samples_split` e `min_samples_leaf` (além de `max_depth`, que aqui foi `None` mas efetivamente limitado pelos outros) são cruciais para controlar a complexidade do modelo.
    * O `GridSearchCV` seleciona a combinação desses parâmetros que maximiza a `balanced_accuracy` na validação cruzada, buscando um equilíbrio que evite o overfitting aos dados de treino e promova uma boa performance em dados não vistos.

* **Número Adequado de Árvores (`n_estimators=100`)**:
    * Construir um número suficiente de árvores (100, no caso) geralmente leva a um modelo mais estável e com melhor generalização, pois a agregação se beneficia da "sabedoria da multidão" das árvores. Embora adicionar mais árvores possa não prejudicar (além do custo computacional) após um certo ponto, um número muito pequeno poderia levar a uma generalização pobre.

Em resumo, o modelo Random Forest do notebook é projetado e treinado de forma a não apenas se ajustar bem aos dados de treinamento, mas também a ser estável e performar de maneira confiável em novos dados, o que é essencial para sua aplicação prática.

---
## - Bom Desempenho em Problemas de Classificação:

### 1. Forças Fundamentais do Algoritmo Random Forest

* **Aprendizado por Ensemble (Bagging)**:
    * O Random Forest constrói múltiplas árvores de decisão (100, neste caso) treinadas em diferentes subamostras dos dados (bootstrap).
    * A decisão final é tomada por agregação (média das probabilidades ou voto majoritário para classificação). Isso **reduz a variância** do modelo em comparação com uma única árvore de decisão, tornando-o menos propenso a memorizar o ruído nos dados de treinamento e melhorando a **generalização** para dados não vistos.

* **Alta Capacidade de Modelagem (Não Linearidade)**:
    * Árvores de decisão, a base do Random Forest, são capazes de capturar relações complexas e **não lineares** entre as features e o alvo. O ensemble herda essa capacidade.

* **Robustez a Outliers e Ruído (Relativa)**:
    * Devido à agregação de múltiplas árvores, o impacto de outliers individuais ou ruído em algumas árvores tende a ser mitigado pelas outras, tornando o modelo geralmente mais robusto.

* **Redução de Overfitting (Comparado a Árvores Individuais)**:
    * Ao combinar muitas árvores, cada uma possivelmente overfit a uma parte dos dados, o Random Forest como um todo tende a ter um **overfitting menor**. A aleatoriedade na seleção de features para cada divisão também contribui para isso.

* **Fornecimento de Importância das Features**:
    * O modelo calcula intrinsecamente a importância de cada feature, o que ajuda a entender os direcionadores da previsão e pode guiar a seleção de features. O código utiliza essa capacidade extensivamente para análise.

---

### 2. Técnicas Específicas Aplicadas no Código que Potencializam o Desempenho

* **Otimização de Hiperparâmetros (`GridSearchCV`)**:
    * O uso do `GridSearchCV` permitiu testar sistematicamente uma grade de hiperparâmetros (`n_estimators`, `max_depth`, `min_samples_split`, `min_samples_leaf`, `class_weight`).
    * A seleção dos **melhores parâmetros** (`{'class_weight': 'balanced_subsample', 'max_depth': None, 'min_samples_leaf': 7, 'min_samples_split': 15, 'n_estimators': 100}`) otimiza o modelo especificamente para este conjunto de dados, maximizando a métrica `balanced_accuracy`.

* **Tratamento Eficaz de Classes Desbalanceadas**:
    * **`class_weight='balanced_subsample'`**: Este hiperparâmetro ajusta automaticamente os pesos das classes em cada árvore com base nas frequências da subamostra de bootstrap, dando mais importância à classe minoritária.
    * **`sample_weights`**: Pesos foram explicitamente calculados e passados aos métodos `.fit()` do `GridSearchCV` e `CalibratedClassifierCV`. Isso força o modelo a prestar mais atenção aos exemplos da classe minoritária durante o treinamento.
    * **Métrica de Avaliação Adequada (`balanced_accuracy`)**: A escolha da `balanced_accuracy` como métrica de scoring no `GridSearchCV` e para a seleção do melhor limiar garante que o desempenho seja avaliado de forma justa, mesmo com classes desbalanceadas.

* **Calibração de Probabilidades (`CalibratedClassifierCV`)**:
    * Modelos como Random Forest podem produzir probabilidades de classe que não são perfeitamente calibradas (ou seja, uma probabilidade prevista de 0.8 não corresponde necessariamente a uma chance real de 80%).
    * A calibração com `method='isotonic'` ajusta essas probabilidades para serem **mais confiáveis e realistas**, o que pode ser crucial para a tomada de decisão baseada nas saídas do modelo.

* **Otimização do Limiar de Classificação**:
    * Em vez de usar o limiar padrão de 0.5 para converter probabilidades em classes, o código **testa múltiplos limiares** (0.3, 0.4, 0.5, 0.6, 0.7).
    * O limiar que maximiza a `balanced_accuracy` (neste caso, 0.6) é selecionado. Isso ajusta o ponto de decisão do modelo para otimizar o desempenho na métrica escolhida, sendo particularmente útil em cenários com classes desbalanceadas ou custos de erro assimétricos.

* **Engenharia de Features Cuidadosa**:
    * O mapeamento de variáveis categóricas ordinais para numéricas (`nivel_ensino_map`, `experiencia_map`, etc.) e a aplicação de one-hot encoding (`pd.get_dummies`) para variáveis nominais são etapas cruciais que preparam os dados adequadamente para o algoritmo Random Forest.

* **Avaliação Abrangente e Visualizações Detalhadas**:
    * O uso de múltiplas métricas (Acurácia, Acurácia Balanceada, F1-Score, Precisão, Recall, Matriz de Confusão, Curva ROC, Curva Precision-Recall) fornece uma visão completa do desempenho do modelo.
    * As visualizações ajudam a diagnosticar o comportamento do modelo e a identificar áreas de força e fraqueza.

A combinação desses fatores – as qualidades inerentes do Random Forest e as técnicas de modelagem e avaliação cuidadosamente implementadas – resulta em um modelo de classificação com bom desempenho e confiabilidade para o problema em questão.

---
## - Manejo de Features Categóricas e Numéricas:

| Atributo                                         | Nome                                      | Tipo         | Subtipo                             | Descrição                                                                                     | Relevância |
|--------------------------------------------------|-------------------------------------------|--------------|-------------------------------------|-----------------------------------------------------------------------------------------------|------------|
| P0                                               | id                 		       | Qualitativo  | Nominal                             | Para identificação da resposta                                    		            | Alta       |
| P1l                                              | Nível de ensino alcançado                 | Qualitativo  | Ordinal                             | Nível de ensino do respondente (graduação, mestrado, etc.)                                    | Alta       |
| P1m                                              | Área de formação acadêmica                | Qualitativo  | Nominal (Multivalorado)             | Área de formação acadêmica do respondente (TI, Economia, etc.)                                | Alta       |
| P2h                                              | Faixa salarial mensal                     | Qualitativo  | Ordinal                             | Faixa salarial mensal do respondente                                                          | Alta       |
| P2i                                              | Tempo de experiência na área de dados     | Quantitativo | Discreto                            | Tempo de experiência do respondente na área de dados (em anos)                                | Alta       |
| P2g                                              | Nível de senioridade                      | Qualitativo  | Ordinal                             | Nível de senioridade do respondente (Júnior, Pleno, Sênior)                                   | Alta       |
| P1b                                              | Gênero do profissional                    | Qualitativo  | Nominal (Multivalorado)             | Identidade de gênero do respondente                                                           | Alta       |
| P1c                                              | Cor/Raça/Etnia                            | Qualitativo  | Nominal (Multivalorado)             | Cor ou raça do respondente                                                                    | Alta       |
| P2b                                              | Setor de atuação da empresa               | Qualitativo  | Nominal (Multivalorado)             | Setor em que a empresa do respondente atua (Tecnologia, Finanças, etc.)                       | Alta       |
| P1i1                                             | UF onde mora                              | Qualitativo  | Nominal (Multivalorado)             | Unidade Federativa onde o respondente reside                                                  | Alta       |
| P2f                                              | Cargo atual                               | Qualitativo  | Nominal (Multivalorado)             | Cargo atual ocupado pelo respondente                                                          | Alta       |
| P2o6                                             | Oportunidade de aprendizado               | Qualitativo  | Nominal (Multivalorado)             | Valorização das oportunidades de aprendizado e crescimento profissional                       | Alta       |
| P2o10                                            | Reputação da empresa                      | Qualitativo  | Nominal (Multivalorado)             | Valorização da reputação que a empresa tem no mercado                                         | Alta       |

---

## *Processo de Amostragem de Dados1-1*
### 1. Divisão Inicial dos Dados em Treino e Teste  partitioning

* **Método**: A função `train_test_split` do Scikit-learn é utilizada para dividir o conjunto de dados completo (`X`, `y`) e os pesos das amostras (`sample_weights`) em conjuntos de treinamento e teste.
    ```python
    X_train, X_test, y_train, y_test, sample_weights_train, _ = train_test_split(
        X, y, sample_weights, test_size=0.3, random_state=42, stratify=y
    )
    ```
* **Proporção**: **70%** dos dados são alocados para o conjunto de **treinamento** (`X_train`, `y_train`, `sample_weights_train`) e **30%** para o conjunto de **teste** (`X_test`, `y_test`).
* **Estratificação**: O parâmetro `stratify=y` garante que a proporção das classes da variável alvo (`y`) seja mantida tanto no conjunto de treino quanto no de teste. Isso é crucial, especialmente porque o dataset possui classes desbalanceadas, assegurando que ambas as classes estejam representadas adequadamente em ambas as divisões.
* **Reprodutibilidade**: `random_state=42` é usado para que a divisão seja sempre a mesma em diferentes execuções do código, garantindo a reprodutibilidade dos resultados.
* **Pesos das Amostras (`sample_weights_train`)**: Os pesos calculados para lidar com o desbalanceamento de classes são divididos juntamente com os dados, e a porção de treino (`sample_weights_train`) é usada nas etapas subsequentes de treinamento e otimização.

---

### 2. Amostragem Interna do `RandomForestClassifier` (Bootstrap) 🌳

* **Bootstrap Aggregating (Bagging)**: O `RandomForestClassifier` é um ensemble de árvores de decisão. Por padrão (**`bootstrap=True`**, que é o default no Scikit-learn e não foi alterado no código), cada árvore na floresta é treinada em uma amostra diferente do conjunto de treinamento, gerada através de **amostragem com reposição** (bootstrap).
    * Isso significa que, para cada uma das `n_estimators` (100 árvores, conforme o melhor parâmetro encontrado), uma nova subamostra do `X_train` é criada, tendo o mesmo tamanho do `X_train` original, mas com algumas instâncias repetidas e outras ausentes.
* **`class_weight='balanced_subsample'`**: Este parâmetro, definido como o melhor pelo `GridSearchCV`, interage com o processo de bootstrap. Os pesos das classes são calculados para cada amostra de bootstrap individualmente, ajustando a importância das classes dentro de cada árvore de forma dinâmica. Isso ajuda a mitigar o desbalanceamento em cada árvore construída.
* **Amostragem de Features**: Além da amostragem de instâncias (linhas), o Random Forest também realiza uma amostragem de features (colunas) ao procurar a melhor divisão em cada nó de cada árvore. O número de features consideradas é tipicamente `sqrt(n_features)`.

---

### 3. Amostragem na Otimização de Hiperparâmetros (`GridSearchCV`) 🔄

* **Validação Cruzada (Cross-Validation)**: O `GridSearchCV` utiliza validação cruzada para avaliar o desempenho de diferentes combinações de hiperparâmetros. No código, `cv=5` foi especificado.
    * O conjunto de **treinamento** (`X_train`, `y_train`) é dividido em **5 folds (subconjuntos)** de tamanho aproximadamente igual.
    * Para cada combinação de hiperparâmetros, o modelo é treinado 5 vezes:
        * Em cada iteração, 4 folds são usados para treinar o modelo.
        * O fold restante (1 fold) é usado como conjunto de validação para avaliar o desempenho.
    * A métrica de desempenho (`balanced_accuracy`) é calculada para cada fold de validação, e a média dessas métricas é usada para classificar a combinação de hiperparâmetros.
* **Uso de `sample_weights_train`**: Os pesos das amostras (`sample_weights_train`) são passados para o método `fit` do `GridSearchCV`. Isso significa que, durante o treinamento de cada modelo dentro da validação cruzada, as amostras são ponderadas conforme definido, influenciando o aprendizado do modelo e o cálculo da métrica de avaliação em cada fold.

---

### 4. Amostragem na Calibração do Modelo (`CalibratedClassifierCV`) ⚖️

* **Validação Cruzada Interna**: O `CalibratedClassifierCV` também utiliza um esquema de validação cruzada para ajustar o calibrador (neste caso, usando o método `'isotonic'`). O parâmetro `cv=5` foi usado aqui também.
    * O conjunto de **treinamento** (`X_train`, `y_train`) é novamente dividido em 5 folds.
    * O `base_estimator` (o `best_rf_model` encontrado pelo GridSearchCV) é treinado em 4 folds, e as previsões de probabilidade são feitas no fold restante.
    * Este processo é repetido para todos os 5 folds, de modo que se obtêm previsões de probabilidade "out-of-fold" para todo o conjunto de treinamento.
    * O calibrador (regressor isotônico) é então treinado usando essas previsões "out-of-fold" como entrada e os verdadeiros rótulos `y_train` como saída.
    * Finalmente, o `base_estimator` é retreinado em todo o conjunto `X_train`, `y_train` (com `sample_weights_train`), e o calibrador treinado é aplicado a ele.
* **Uso de `sample_weights_train`**: Assim como no `GridSearchCV`, os `sample_weights_train` são passados para o método `fit` do `CalibratedClassifierCV`, garantindo que o processo de calibração também leve em consideração o desbalanceamento das classes através da ponderação das amostras.

Este conjunto de técnicas de amostragem e reponderação visa construir um modelo robusto, generalizável e que lide adequadamente com o desbalanceamento inerente aos dados.

---
## *Parâmetros utilizados1-1*
O modelo final é um `RandomForestClassifier` cujos hiperparâmetros foram otimizados usando `GridSearchCV`, e subsequentemente, este modelo otimizado foi calibrado usando `CalibratedClassifierCV`.

### 1. Hiperparâmetros Otimizados do `RandomForestClassifier` (Resultado do `GridSearchCV`)

Estes são os melhores parâmetros encontrados pelo `GridSearchCV` para o `RandomForestClassifier`, que é então usado como `base_estimator` para a calibração:

* **`class_weight`**: `'balanced_subsample'`
    * *Explicação*: Ajusta os pesos das classes de forma inversamente proporcional às suas frequências. A variante `'balanced_subsample'` calcula os pesos com base nas amostras de bootstrap para cada árvore.
* **`max_depth`**: `None`
    * *Explicação*: Indica que não há um limite predefinido para a profundidade máxima das árvores. As árvores são expandidas até que todas as folhas sejam puras ou até que todas as folhas contenham menos amostras do que `min_samples_split`.
* **`min_samples_leaf`**: `7`
    * *Explicação*: O número mínimo de amostras que um nó folha (nó terminal de uma árvore) deve ter. Um valor maior previne a criação de folhas muito específicas, ajudando a evitar overfitting.
* **`min_samples_split`**: `15`
    * *Explicação*: O número mínimo de amostras que um nó interno deve ter para poder ser dividido em novos nós. Similar ao `min_samples_leaf`, ajuda a controlar a complexidade da árvore e a evitar overfitting.
* **`n_estimators`**: `100`
    * *Explicação*: O número de árvores na floresta. Um valor maior geralmente leva a um modelo melhor e mais estável, mas também aumenta o tempo de treinamento.

**Parâmetros Adicionais (Fixos na Instanciação Base do `RandomForestClassifier` antes do `GridSearchCV`):**

* **`random_state`**: `42`
    * *Explicação*: Controla tanto a aleatoriedade do bootstrapping das amostras usadas ao construir as árvores (se `bootstrap=True`) quanto a amostragem das features a serem consideradas ao procurar a melhor divisão em cada nó. Usado para reprodutibilidade.
* **`n_jobs`**: `-1`
    * *Explicação*: Indica ao Scikit-learn para usar todos os processadores disponíveis para paralelizar o treinamento das árvores, acelerando o processo.

### 2. Parâmetros do `CalibratedClassifierCV`

O `best_rf_model` (com os hiperparâmetros acima) é então usado como o estimador base para a calibração:

* **`base_estimator`**: `best_rf_model` (o RandomForestClassifier com os parâmetros otimizados listados acima)
    * *Explicação*: O modelo cujas probabilidades serão calibradas.
* **`method`**: `'isotonic'`
    * *Explicação*: O método usado para a calibração. A regressão isotônica é um método não paramétrico que ajusta as probabilidades de forma a minimizar o erro quadrático médio, sob a restrição de que a função de calibração seja monotonicamente crescente. É geralmente mais flexível que o método 'sigmoid'.
* **`cv`**: `5`
    * *Explicação*: Determina a estratégia de validação cruzada. Aqui, 5 folds são usados. O modelo é treinado em 4 folds e calibrado no fold restante, e este processo é repetido para todos os folds. As previsões para cada fold são então usadas para treinar o calibrador final.

### 3. Parâmetros Utilizados na Chamada `.fit()` do `GridSearchCV` e `CalibratedClassifierCV`

* **`sample_weight`**: `sample_weights_train`
    * *Explicação*: Pesos aplicados a amostras individuais durante o treinamento. No código, esses pesos são calculados para dar maior importância às amostras da classe minoritária, ajudando a lidar com o desbalanceamento dos dados. Este parâmetro é passado tanto para o `.fit()` do `GridSearchCV` quanto do `CalibratedClassifierCV`.

---

# *Explicação do Código1-1*

## Análise Detalhada do Código Python: Modelo Random Forest para Previsão Salarial

### 1. Visão Geral do Código

* **Objetivo Principal:** O script tem como objetivo construir um modelo de Machine Learning, especificamente um `RandomForestClassifier`, para prever se um profissional da área de dados possui um salário "alto" (acima de R$ 8.000/mês) ou "baixo/médio" (até R$ 8.000/mês). Isso é tratado como um problema de classificação binária.
* **Bibliotecas Utilizadas:**
    * **`pandas`**: Para manipulação e análise de dados, principalmente na forma de DataFrames.
    * **`numpy`**: Para operações numéricas, especialmente útil para cálculos de `sample_weights` e manipulação de arrays.
    * **`sklearn.model_selection`**:
        * `train_test_split`: Para dividir os dados em conjuntos de treino e teste.
        * `GridSearchCV`: Para otimização de hiperparâmetros do modelo.
    * **`sklearn.ensemble.RandomForestClassifier`**: A classe principal para a implementação do modelo Random Forest.
    * **`sklearn.metrics`**: Contém diversas funções para avaliar a performance do modelo, como:
        * `confusion_matrix`: Para criar a matriz de confusão.
        * `accuracy_score`: Para calcular a acurácia.
        * `classification_report`: Para gerar um relatório detalhado com precisão, recall, F1-score por classe.
        * `roc_curve`, `auc`: Para gerar e calcular a área sob a Curva ROC.
        * `balanced_accuracy_score`: Acurácia ponderada para classes desbalanceadas.
        * `f1_score`: Métrica F1, que considera precisão e recall.
        * `precision_recall_curve`: Para gerar a curva Precision-Recall.
    * **`sklearn.calibration.CalibratedClassifierCV`**: Para calibrar as probabilidades do modelo, tornando-as mais confiáveis.
    * **`matplotlib.pyplot`**: Para a criação de gráficos estáticos e visualizações.
    * **`sklearn.tree.plot_tree`**: Para visualizar uma árvore de decisão individual do Random Forest.
    * **`seaborn`**: Para criar visualizações estatísticas mais elaboradas e esteticamente agradáveis.
    * **`os`**: Para interagir com o sistema operacional, como criar diretórios para salvar os gráficos.

---

## 2. Pré-processamento de Dados e Engenharia de Features

O código realiza um pré-processamento extenso e uma engenharia de features cuidadosa.

* **Carregamento dos Dados:**
    * Os dados são carregados de um arquivo CSV (`dados_limpos.csv`). O script tenta primeiro um caminho no ambiente Kaggle (`/kaggle/input/dataset-clean/dados_limpos.csv`) e, se não encontrado, tenta carregar localmente.
    * Uma mensagem é impressa indicando a origem do dataset carregado.

* **Seleção e Limpeza Inicial:**
    * São selecionadas colunas específicas para features (`colunas_features`) e a coluna alvo (`coluna_target`).
    * Linhas com valores ausentes (`NaN`) nas colunas cruciais selecionadas são removidas usando `df_limpo.dropna(subset=colunas_necessarias, inplace=True)`.

* **Engenharia de Features:**
    * **Mapeamento Ordinal:** Diversas colunas categóricas ordinais são convertidas para representações numéricas usando mapeamentos predefinidos:
        * `'Nível de ensino alcançado'` -> `formacao_academica_encoded` (e.g., 'Estudante de Graduação': 0, 'Doutorado ou Phd': 4)
        * `'Tempo de experiência na área de dados'` -> `experiencia_profissional_encoded` (e.g., 'Menos de 1 ano': 0, 'Mais de 10 anos': 5)
        * `'Nível de senioridade'` -> `senioridade_encoded` (e.g., 'Júnior': 0, 'Sênior': 2)
        * `'Faixa salarial mensal'` -> `faixa_salarial_encoded` (e.g., 'Menos de R$ 1.000/mês': 0, 'Acima de R$ 40.001/mês': 12)
    * **Criação da Variável Alvo Binária:**
        * A variável alvo `salario_alto` é criada a partir da `faixa_salarial_encoded`. É definida como `1` se `faixa_salarial_encoded > 5` (correspondendo a salários acima de R$ 8.000/mês) e `0` caso contrário.
    * **Codificação One-Hot:**
        * Variáveis categóricas nominais (`'Área de formação acadêmica'`, `'UF onde mora'`, `'Setor de atuação da empresa'`) são transformadas em múltiplas colunas binárias (0 ou 1) usando `pd.get_dummies()`. Isso evita que o modelo interprete uma ordem inexistente nessas categorias.
    * **Remoção Final de NaNs:** Após os mapeamentos, `dropna()` é usado novamente para garantir que não haja NaNs nas colunas codificadas que serão usadas no modelo.

* **Definição das Features (X) e Target (y):**
    * `X`: Contém as colunas de features processadas (codificadas ordinalmente e via one-hot).
    * `y`: Contém a variável alvo binária `salario_alto`.

* **Verificação de Dados e Balanceamento das Classes:**
    * O código verifica se há dados suficientes para o treinamento e se existem pelo menos duas classes na variável alvo.
    * A distribuição das classes (Salário Baixo/Médio vs. Salário Alto) é impressa, mostrando o percentual de cada uma. Isso é crucial para entender o desbalanceamento.

* **Balanceamento dos Dados (Tratamento de Classes Desbalanceadas):**
    * Em vez de usar técnicas de reamostragem como SMOTE, o script opta por duas estratégias:
        1.  **`class_weight` no Modelo:** O hiperparâmetro `class_weight` do `RandomForestClassifier` (e usado no `GridSearchCV`) pode ser configurado como `'balanced'` ou `'balanced_subsample'` para que o modelo penalize mais os erros na classe minoritária.
        2.  **`sample_weights` no Treinamento:** Pesos são calculados para cada amostra (`sample_weights`) com base na frequência das classes. Amostras da classe minoritária recebem um peso maior. Esses pesos são passados diretamente para o método `fit` do `GridSearchCV` e do `CalibratedClassifierCV`.
            ```python
            class_weights_calc = {0: 1.0, 1: class_counts[0] / class_counts[1]}
            sample_weights = np.array([class_weights_calc[cls] for cls in y])
            ```

* **Divisão em Conjuntos de Treino e Teste:**
    * Os dados (`X`, `y`) e os `sample_weights` são divididos em conjuntos de treino e teste usando `train_test_split`.
    * `test_size=0.3`: 30% dos dados são reservados para o conjunto de teste, e 70% para o treino.
    * `random_state=42`: Garante que a divisão seja a mesma toda vez que o código for executado, permitindo reprodutibilidade.
    * `stratify=y`: Assegura que a proporção das classes na variável alvo `y` seja mantida tanto no conjunto de treino quanto no de teste. Isso é especialmente importante para dados desbalanceados.
    * Os tamanhos dos conjuntos resultantes (`X_train`, `X_test`, `y_train`, `y_test`) são impressos.

---

## 3. Construção e Treinamento do Modelo Random Forest

* **Otimização de Hiperparâmetros com `GridSearchCV`:**
    * Uma grade de hiperparâmetros (`param_grid`) é definida para o `RandomForestClassifier`. Os parâmetros testados incluem:
        * `n_estimators`: Número de árvores na floresta (100, 200, 300). Mais árvores geralmente melhoram o desempenho, mas aumentam o custo computacional.
        * `max_depth`: Profundidade máxima de cada árvore (None - sem limite, 10, 20). Controla a complexidade das árvores; None pode levar a overfitting se não controlado por outros parâmetros.
        * `min_samples_split`: Número mínimo de amostras necessárias para dividir um nó interno (5, 10, 15). Ajuda a controlar o overfitting.
        * `min_samples_leaf`: Número mínimo de amostras que um nó folha deve ter (3, 5, 7). Também ajuda a controlar o overfitting.
        * `class_weight`: Estratégia para lidar com classes desbalanceadas ('balanced', 'balanced_subsample').
    * Um modelo base `RandomForestClassifier` é instanciado com `random_state=42` (para reprodutibilidade) e `n_jobs=-1` (para usar todos os processadores disponíveis).
    * `GridSearchCV` é instanciado para testar todas as combinações de hiperparâmetros da `param_grid`.
        * `estimator=rf_base`: O modelo a ser otimizado.
        * `cv=5`: Utiliza validação cruzada de 5 folds. Os dados de treino são divididos em 5 partes; o modelo é treinado em 4 e validado na 5ª, repetindo o processo 5 vezes.
        * `scoring='balanced_accuracy'`: A métrica usada para avaliar qual combinação de hiperparâmetros é a melhor. A acurácia balanceada é preferível à acurácia simples em casos de desbalanceamento.
        * `verbose=1`: Mostra mensagens durante o processo de busca.
    * O `GridSearchCV` é treinado usando `grid_search.fit(X_train, y_train, sample_weight=sample_weights_train)`. Note o uso de `sample_weights_train` aqui.
    * Os melhores parâmetros encontrados pelo `GridSearchCV` são impressos e o melhor estimador (`best_rf_model`) é armazenado.

---

## 4. Calibração do Modelo

* **Objetivo:** As probabilidades brutas de modelos como Random Forest podem não ser bem calibradas (ex: uma probabilidade prevista de 0.7 não significa necessariamente 70% de chance real). A calibração ajusta essas probabilidades para que sejam mais confiáveis.
* **Implementação:**
    * `CalibratedClassifierCV` é usado para calibrar o `best_rf_model` encontrado pelo `GridSearchCV`.
    * `base_estimator=best_rf_model`: O modelo a ser calibrado.
    * `method='isotonic'`: O método de calibração. A regressão isotônica é um método não paramétrico que geralmente funciona bem. Alternativamente, 'sigmoid' (regressão logística) poderia ser usado.
    * `cv=5`: Usa validação cruzada de 5 folds para a calibração.
    * O modelo calibrado (`calibrated_model`) é treinado usando `calibrated_model.fit(X_train, y_train, sample_weight=sample_weights_train)`, novamente utilizando os pesos das amostras.

---

## 5. Realização de Previsões e Otimização do Limiar de Classificação

* **Previsão de Probabilidades:**
    * O modelo calibrado é usado para prever as probabilidades para a classe positiva (salário alto) no conjunto de teste:
        ```python
        y_pred_proba_test = calibrated_model.predict_proba(X_test)[:, 1]
        ```
    * `predict_proba` retorna um array com as probabilidades para cada classe. `[:, 1]` seleciona as probabilidades da classe positiva (índice 1). Essas probabilidades são cruciais porque o limiar de decisão padrão de 0.5 nem sempre é o ideal, especialmente em problemas com classes desbalanceadas ou quando os custos de erros falso positivo e falso negativo são diferentes.

* **Avaliação com Diferentes Limiares:**
    * O código testa uma série de limiares de classificação (`thresholds = [0.3, 0.4, 0.5, 0.6, 0.7]`).
    * Para cada limiar:
        * As probabilidades são convertidas em predições de classe: `(y_pred_proba_test >= threshold).astype(int)`.
        * São calculadas e impressas diversas métricas: Acurácia, Acurácia Balanceada, F1-Score, Matriz de Confusão (TN, FP, FN, TP), e Precisão/Recall para cada classe.
    * **Seleção do Melhor Limiar:** O limiar que resulta na maior `balanced_accuracy` é escolhido como o "melhor limiar".
        ```python
        best_threshold_idx = max(range(len(results)), key=lambda i: results[i]['balanced_accuracy'])
        best_threshold = results[best_threshold_idx]['threshold']
        ```
    * As predições finais no conjunto de teste (`y_pred_final`) são feitas usando este melhor limiar.

---

## 6. Avaliação Final do Modelo

* Com as predições finais (`y_pred_final`) obtidas usando o limiar otimizado, um `classification_report` completo é gerado e impresso.
* Este relatório fornece:
    * **Precisão (Precision):** Das vezes que o modelo previu uma classe, quantas estavam corretas. (TP / (TP + FP))
    * **Recall (Sensibilidade):** Das instâncias reais de uma classe, quantas o modelo conseguiu identificar corretamente. (TP / (TP + FN))
    * **F1-Score:** Média harmônica da precisão e do recall. É uma boa métrica geral, especialmente se houver desbalanceamento.
    * **Support:** Número de ocorrências reais de cada classe.
    * **Accuracy (Acurácia Geral):** Proporção de predições corretas no total.
    * **Macro Avg:** Média aritmética das métricas (precisão, recall, F1) para cada classe, sem ponderação.
    * **Weighted Avg:** Média das métricas ponderada pelo suporte de cada classe.

---

## 7. Análise de Importância das Features

* **Cálculo:** A importância de cada feature é extraída do `best_rf_model` (o modelo Random Forest otimizado, antes da calibração, pois `CalibratedClassifierCV` não expõe `feature_importances_` diretamente do `base_estimator` de forma simples, mas o `best_rf_model` é o estimador treinado).
    ```python
    importances = best_rf_model.feature_importances_
    feature_names = X.columns
    indices = np.argsort(importances)[::-1] # Ordena da mais para a menos importante
    ```
* **Valor da Informação:** Entender quais features são mais influentes para as previsões do modelo é crucial para:
    * Interpretabilidade do modelo.
    * Seleção de features (possivelmente removendo as menos importantes para simplificar o modelo).
    * Obter insights sobre o problema em questão.
* **Visualização:**
    * Um gráfico de barras horizontais mostra as **20 features mais importantes**.
    * Para uma análise mais detalhada, são gerados gráficos de barras **por grupo de features** (prefixo do nome da feature, ex: 'Área de formação acadêmica_'), caso haja mais de 20 features no total. Isso ajuda a organizar a visualização quando há muitas features (especialmente após o one-hot encoding).
    * Um gráfico de barras horizontais focado nas **Top 3 features mais importantes** é criado, com os valores de importância anotados nas barras.

---

## 8. Visualizações Geradas

O script gera e salva diversas visualizações para ajudar na compreensão e avaliação do modelo. Todas são salvas no diretório `/kaggle/working/`.

* **Configuração dos Gráficos:** Um estilo (`seaborn-v0_8-whitegrid`) e tamanhos de fonte/figura padrão são definidos para consistência.
* **Gráficos:**
    1.  **Matriz de Confusão (`matriz_confusao_otimizada.png`):**
        * Visualiza o desempenho do modelo no conjunto de teste usando o limiar otimizado. Mostra Verdadeiros Positivos (TP), Verdadeiros Negativos (TN), Falsos Positivos (FP) e Falsos Negativos (FN).
    2.  **Curva ROC (`curva_roc_otimizada.png`):**
        * Plota a Taxa de Verdadeiros Positivos (TPR) contra a Taxa de Falsos Positivos (FPR) para diferentes limiares de classificação.
        * A área sob a curva (AUC) é uma medida da capacidade do modelo de distinguir entre as classes. Um valor maior é melhor.
        * Uma linha vertical indica o melhor limiar encontrado.
    3.  **Curva Precision-Recall (`precision_recall_curve.png`):**
        * Mostra a relação entre precisão e recall para diferentes limiares. É particularmente útil para problemas com classes desbalanceadas.
    4.  **Importância das Features (`importancia_features_top20.png`, `importancia_features_grupo_*.png`, `top3_features.png`):**
        * Conforme descrito na seção anterior, visualiza a relevância de cada feature.
    5.  **Distribuição das Probabilidades Preditas (`distribuicao_probabilidades.png`):**
        * Um histograma das probabilidades previstas para a classe "Salário Alto" no conjunto de teste.
        * Uma linha vertical marca o melhor limiar, ajudando a visualizar como ele separa as predições.
    6.  **Visualização de uma Árvore do Random Forest (`arvore_exemplo_melhorada.png`, `arvore_exemplo_simplificada.png`):**
        * Mostra a estrutura de uma única árvore de decisão do ensemble Random Forest (a primeira árvore, `estimators_[0]`).
        * Duas versões são salvas: uma mais detalhada (`max_depth=4`) e uma mais simplificada (`max_depth=3`) para facilitar a interpretação. É útil para entender como as decisões são tomadas em um nível micro.
    7.  **Análise de Interação entre Formação e Experiência (`interacao_formacao_experiencia.png`):**
        * Um heatmap que mostra a probabilidade média de ter "Salário Alto" para diferentes combinações de `formacao_academica_encoded` e `experiencia_profissional_encoded`. Isso ajuda a identificar interações entre essas duas features importantes.
    8.  **Gráfico de Dispersão para as Duas Features Mais Importantes (`dispersao_top2_features.png`):**
        * Se houver pelo menos duas features, um gráfico de dispersão é criado usando as duas features mais importantes do conjunto de teste. Os pontos são coloridos pela probabilidade prevista de "Salário Alto", permitindo visualizar como essas duas features, em conjunto, se relacionam com a previsão.

-------------------------------------------

### Modelo 2 Análise de Disparidade Salarial de Profissionais de Dados no Brasil Utilizando o Arvore de decisão por classificação
### *Justificativa1-2*

O modelo escolhido foi o Gradient Boosting Classifier, uma técnica de ensemble baseada em árvores de decisão. A escolha se justifica porque o problema envolve múltiplas variáveis categóricas, relações não-lineares e a necessidade de interpretar a influência de fatores como formação acadêmica e experiência profissional sobre faixas salariais. O Gradient Boosting é reconhecido por sua eficácia em tarefas de classificação com dados tabulares e mistos, como é o caso do dataset analisado

### *Processo de Amostragem de Dados (Particionamento e Cross-Validation)1-2*

## Processo de Amostragem de Dados (Particionamento e Cross-Validation)

### 1. Particionamento dos Dados (Train-Test Split)

- **Divisão Estratificada:**  
  O conjunto de dados foi dividido em 70% para treinamento e 30% para teste, utilizando `train_test_split` com o parâmetro `stratify` baseado na variável alvo (faixa salarial agrupada).  
  Isso garante que a proporção de cada classe salarial seja mantida tanto no treino quanto no teste, evitando viés na avaliação do modelo.

- **Reprodutibilidade:**  
  O parâmetro `random_state=42` foi utilizado para garantir que a divisão dos dados seja sempre a mesma em diferentes execuções, permitindo reprodutibilidade dos resultados.

---

### 2. Cross-Validation Estratificada (Stratified K-Fold)

- **Validação Cruzada Estratificada:**  
  Durante a otimização de hiperparâmetros (`RandomizedSearchCV`), foi empregada a validação cruzada estratificada (`StratifiedKFold`) com 3 folds.  
  Em cada iteração, o conjunto de treino é novamente dividido em 3 subconjuntos, mantendo a proporção das classes em cada fold. O modelo é treinado em dois folds e avaliado no terceiro, repetindo o processo para todos os folds.

- **Vantagens da Estratificação:**  
  - Garante que todas as classes estejam representadas de forma proporcional em cada fold, o que é crucial para problemas com classes desbalanceadas.
  - Reduz o risco de variações indesejadas nos resultados devido à distribuição das classes.


3. **Estratificação:**  
   Mantém a distribuição das faixas salariais em todas as etapas, tanto no split inicial quanto na validação cruzada, assegurando comparabilidade e evitando viés de classe.


### **Capacidade de Capturar Interações Complexas**

Modelos de árvores, especialmente ensembles como o Gradient Boosting, capturam automaticamente interações complexas entre variáveis sem a necessidade de especificá-las manualmente. Isso é fundamental para o contexto, pois a relação entre formação acadêmica, experiência e salário não é linear nem independente: o impacto de um fator depende do outro. O modelo constrói sucessivas árvores que corrigem os erros das anteriores, ajustando-se a padrões e interações sutis presentes nos dados


### **Fornecimento de Importância das Features**

O Gradient Boosting permite extrair a importância relativa de cada variável para a predição, facilitando a interpretação dos fatores que mais influenciam o salário. O código calcula e reporta métricas como o coeficiente de Cramer's V para variáveis categóricas antes do treinamento, e a própria biblioteca do modelo possibilita gerar rankings de importância das features após o ajuste. Isso é essencial para análises orientadas a dados e para justificar decisões baseadas nos resultados do modelo


### **Robustez e Generalização**

O Gradient Boosting é robusto a outliers e a diferentes escalas de variáveis, além de apresentar boa capacidade de generalização quando parametrizado corretamente. O pipeline do código inclui validação cruzada estratificada, balanceamento de classes e busca de hiperparâmetros (RandomizedSearchCV), o que reduz o risco de overfitting e melhora a performance em dados não vistos. Isso garante que as conclusões sobre disparidade salarial sejam confiáveis e replicáveis em outros conjuntos de dados semelhantes

### **Bom Desempenho em Problemas de Classificação**

Modelos baseados em Gradient Boosting frequentemente apresentam desempenho superior em benchmarks de classificação com dados tabulares, especialmente quando há múltiplas classes e desbalanceamento, como no caso das faixas salariais. O modelo atingiu acurácia de 52,7% e acurácia balanceada de 40,1%, valores considerados competitivos para um problema de alta complexidade e múltiplas categorias. Além disso, o modelo lida bem com variáveis categóricas codificadas via OneHotEncoder e com a necessidade de interpretar resultados para diferentes grupos

### 

### *Parâmetros utilizados1-2*

## Parâmetros Utilizados no Modelo GradientBoostingClassifier

Abaixo estão os principais hiperparâmetros definidos após otimização com RandomizedSearchCV:

| Parâmetro           | Valor   | Descrição                                                                                           |
|---------------------|---------|-----------------------------------------------------------------------------------------------------|
| `subsample`         | 0.8     | Proporção de amostras usadas em cada árvore (80%). Ajuda a reduzir overfitting e aumenta robustez. |
| `n_estimators`      | 100     | Número de árvores no ensemble. Equilibra desempenho e custo computacional.                          |
| `min_samples_split` | 2       | Mínimo de amostras para dividir um nó. Permite divisões detalhadas, capturando padrões sutis.      |
| `min_samples_leaf`  | 2       | Mínimo de amostras em cada folha. Evita que folhas pequenas capturem apenas ruído.                 |
| `max_depth`         | 6       | Profundidade máxima das árvores. Limita a complexidade e controla overfitting.                     |
| `learning_rate`     | 0.2     | Taxa de aprendizado. Controla o quanto cada árvore corrige os erros das anteriores.                |

Esses parâmetros foram escolhidos para equilibrar desempenho, capacidade de generalização e evitar overfitting, garantindo que o modelo seja capaz de capturar padrões relevantes dos dados salariais sem se ajustar demais ao conjunto de treino.


### *Explicação do Código:1-2*

### 1. Contexto do Modelo

* **Problema:** O modelo visa classificar profissionais em diferentes **faixas salariais** (variável alvo) com base em um conjunto de características categóricas, como nível de ensino, área de formação, tempo de experiência, etc. Trata-se de um problema de **classificação multiclasse**.
* **Gradient Boosting Classifier:** É um algoritmo de aprendizado de máquina poderoso que pertence à família de modelos de *ensemble boosting*. Ele constrói modelos (geralmente árvores de decisão) de forma sequencial, onde cada novo modelo tenta corrigir os erros cometidos pelo modelo anterior. O resultado final é uma combinação ponderada de todos os modelos, o que geralmente leva a uma melhor performance e robustez em comparação com modelos individuais.

---

### 2. Análise do Código Bloco a Bloco

#### **Importações de Bibliotecas**

O código começa importando diversas bibliotecas essenciais para manipulação de dados, visualização, pré-processamento, modelagem e avaliação:

* `pandas` (pd): Para manipulação e análise de dados tabulares (DataFrames).
* `numpy` (np): Para operações numéricas eficientes, especialmente com arrays.
* `matplotlib.pyplot` (plt) e `seaborn` (sns): Para criação de gráficos e visualizações de dados.
* `sklearn.model_selection`: Contém funções para divisão de dados (`train_test_split`), otimização de hiperparâmetros (`GridSearchCV`, `RandomizedSearchCV`) e validação cruzada (`StratifiedKFold`).
* `sklearn.preprocessing`: Inclui ferramentas para transformação de features, como `LabelEncoder` (para codificar a variável alvo) e `OneHotEncoder` (para codificar variáveis categóricas).
* `sklearn.compose`: Permite a criação de transformadores complexos para diferentes tipos de colunas (`ColumnTransformer`).
* `sklearn.pipeline`: Embora `Pipeline` seja importado, não é explicitamente utilizado para construir o pipeline do modelo neste trecho final, mas o pré-processador (`ColumnTransformer`) age de forma similar para as features.
* `sklearn.metrics`: Fornece métricas para avaliação de modelos de classificação, como `classification_report`, `confusion_matrix`, `roc_curve`, `auc`, `accuracy_score`, `balanced_accuracy_score`.
* `sklearn.ensemble.GradientBoostingClassifier`: A implementação do modelo de Gradient Boosting.
* `collections.Counter`: Para contagem de itens (não utilizado explicitamente no fluxo principal, mas útil para EDA).
* `os`: Para interagir com o sistema operacional (ex: verificar existência de arquivos).
* `warnings`: Para controlar mensagens de aviso.
* `joblib`: Para salvar e carregar modelos treinados.
* `sklearn.inspection.permutation_importance`: Para avaliar a importância das features (importado, mas não usado no trecho final).
* `scipy.stats.chi2_contingency`: Para o teste qui-quadrado, usado no cálculo do V de Cramer.
* `matplotlib.cm`: Para mapas de cores (importado, mas não usado diretamente).
* `scipy.sparse`: Para manipulação de matrizes esparsas, que podem ser resultado do `OneHotEncoder`.
* `time`: Para medir o tempo de execução de trechos do código.

Configurações iniciais também são definidas para visualizações (`warnings.filterwarnings`, `plt.style.use`, `sns.set_palette`, `plt.rcParams`).

#### **Funções Auxiliares Definidas**

* `safe_execution(func, error_message, *args, **kwargs)`: Uma função wrapper para executar outras funções e capturar exceções, imprimindo uma mensagem de erro personalizada.
* `cramers_v(x, y)`: Calcula o coeficiente V de Cramer, uma medida de associação entre duas variáveis categóricas.
* `detect_outliers(df, column)`: Define uma função para detectar outliers usando o método do Intervalo Interquartil (IQR). Esta função é definida mas não explicitamente chamada para remover outliers do dataframe principal no fluxo de pré-processamento do modelo.
* `group_salary_ranges(df, salary_column)`: Agrupa faixas salariais originais em categorias mais amplas para reduzir o número de classes da variável alvo.

#### **Carregamento e Exploração Inicial dos Dados**

* **Carregamento:** Os dados são carregados de um arquivo CSV (`dados_limpos.csv`). O código tenta primeiro um caminho (`/kaggle/input/dataset-clean/dados_limpos.csv`) e, se não encontrado, tenta um caminho local (`dados_limpos.csv`).
    ```python
    file_path = '/kaggle/input/dataset-clean/dados_limpos.csv'
    if not os.path.exists(file_path):
        file_path = 'dados_limpos.csv'
    df = pd.read_csv(file_path)
    ```
* **Informações Básicas:** São impressas informações sobre o dataset:
    * Número de registros e colunas (`df.shape`).
    * Lista das colunas (`df.columns.tolist()`).
* **Exploração da Variável Alvo Original:** A distribuição da coluna original `Faixa salarial mensal` é calculada e impressa usando `value_counts()`.
* **Visualização da Distribuição Salarial Original:** Um gráfico de barras (`sns.countplot`) é gerado para mostrar a distribuição das faixas salariais originais e salvo como `distribuicao_faixas_salariais_originais.png`.

#### **Pré-processamento dos Dados**

* **Agrupamento de Faixas Salariais:** A função `group_salary_ranges` é chamada para criar uma nova coluna `Faixa salarial agrupada`, que será a variável alvo do modelo. Isso é feito para simplificar o problema, reduzindo a granularidade e o desbalanceamento entre as classes.
    ```python
    df = group_salary_ranges(df, 'Faixa salarial mensal')
    ```
* **Visualização da Distribuição Salarial Agrupada:** Um novo gráfico de barras é gerado e salvo (`distribuicao_faixas_salariais_agrupadas.png`) para mostrar a distribuição das novas faixas salariais agrupadas.
* **Análise de Correlação (V de Cramer):** O coeficiente V de Cramer é calculado entre as variáveis categóricas selecionadas (`categorical_cols`) e a nova variável alvo `Faixa salarial agrupada`. Isso ajuda a entender a força da relação entre as features e o target. Os resultados são impressos e visualizados em um gráfico de barras salvo como `correlacao_variaveis_faixa_salarial.png`.
    ```python
    categorical_cols = ['Nível de ensino alcançado', 'Área de formação acadêmica', ...]
    # ...
    corr_with_target[col] = cramers_v(df[col], df['Faixa salarial agrupada'])
    ```
* **Seleção de Features e Target:**
    * **Features (X):** As colunas definidas em `categorical_cols` são selecionadas como variáveis preditoras.
        ```python
        features = df[categorical_cols]
        ```
    * **Target (y):** A coluna `Faixa salarial agrupada` é definida como a variável alvo.
        ```python
        target = df['Faixa salarial agrupada']
        ```
* **Codificação da Variável Alvo:** A variável alvo (`target`) é categórica e é transformada em valores numéricos usando `LabelEncoder`. Um mapeamento dos códigos para os rótulos originais é criado e impresso.
    ```python
    le_target = LabelEncoder()
    y = le_target.fit_transform(target)
    target_mapping = dict(zip(range(len(le_target.classes_)), le_target.classes_))
    ```
* **Tratamento de Variáveis Categóricas (Features):** As features categóricas são transformadas usando `OneHotEncoder` dentro de um `ColumnTransformer`. O `handle_unknown='ignore'` garante que, se novas categorias aparecerem no conjunto de teste, elas não causarão erro e serão codificadas como todas as colunas do OHE zeradas para aquela feature.
    ```python
    preprocessor = ColumnTransformer(
        transformers=[
            ('cat', OneHotEncoder(handle_unknown='ignore'), categorical_features)
        ])
    ```
* **Normalização/Padronização:** Não há etapas explícitas de normalização (ex: MinMaxScaler) ou padronização (ex: StandardScaler) aplicadas às features numéricas resultantes do One-Hot Encoding. Para árvores de decisão e ensembles baseados em árvores como Gradient Boosting, a normalização de features não é estritamente necessária, pois esses modelos são menos sensíveis à escala das features.

#### **Divisão dos Dados**

* Os dados (features e target codificado) são divididos em conjuntos de **treino** e **teste** na proporção 70/30. A função `train_test_split` é utilizada com `stratify=y` para garantir que a proporção das classes da variável alvo seja mantida em ambos os conjuntos, o que é importante para dados desbalanceados. `random_state=42` garante a reprodutibilidade da divisão.
    ```python
    X_train, X_test, y_train, y_test = train_test_split(
        features, y, test_size=0.3, random_state=42, stratify=y
    )
    ```
* O pré-processador (OneHotEncoder) é ajustado (`fit_transform`) **apenas** nos dados de treino (`X_train`) e depois aplicado (`transform`) nos dados de teste (`X_test`). Isso evita o vazamento de dados (data leakage) do conjunto de teste para o processo de treinamento.
    ```python
    X_train_transformed = preprocessor.fit_transform(X_train)
    # ... mais tarde ...
    X_test_transformed = preprocessor.transform(X_test)
    ```

#### **Balanceamento de Classes (Oversampling)**

* Como as classes da variável alvo podem ser desbalanceadas (algumas faixas salariais podem ter muito menos amostras que outras), uma técnica de **oversampling manual** é aplicada ao conjunto de **treinamento**.
* O código primeiro converte `X_train_transformed` (que pode ser uma matriz esparsa) para uma matriz densa.
* Para cada classe minoritária no conjunto de treinamento, amostras são reamostradas **com reposição** (`replace=True`) usando `sklearn.utils.resample` até que o número de amostras naquela classe atinja o tamanho da classe majoritária.
* Isso resulta em `X_train_resampled` e `y_train_resampled` onde todas as classes têm o mesmo número de instâncias no conjunto de treino.
    ```python
    # ... (código para encontrar majority_size e iterar pelas classes)
    resampled_features, resampled_targets = resample(
        class_features, class_targets,
        replace=True,
        n_samples=n_samples, # n_samples é majority_size
        random_state=42
    )
    # ...
    X_train_resampled = np.vstack(X_resampled_list)
    y_train_resampled = np.concatenate(y_resampled_list)
    ```
* A distribuição das classes após o balanceamento é impressa.

#### **Criação e Treinamento do Modelo (Gradient Boosting)**

* **Instanciação do Modelo:** Um `GradientBoostingClassifier` é instanciado.
    ```python
    gb_clf = GradientBoostingClassifier(random_state=42)
    ```
* **Otimização de Hiperparâmetros:** O código oferece três opções para definir/otimizar os hiperparâmetros do modelo:
    1.  `GridSearchCV` com um grid reduzido de parâmetros.
    2.  `RandomizedSearchCV` com uma distribuição de parâmetros (opção escolhida automaticamente no script).
    3.  Usar um conjunto pré-definido de parâmetros otimizados.

    A **Opção 2 (RandomizedSearchCV)** é executada por padrão:
    * `param_dist`: Um dicionário define o espaço de busca dos hiperparâmetros (`n_estimators`, `learning_rate`, `max_depth`, `min_samples_split`, `min_samples_leaf`, `subsample`).
    * `cv = StratifiedKFold(n_splits=3, ...)`: Validação cruzada estratificada com 3 folds é usada para avaliar cada combinação de hiperparâmetros.
    * `RandomizedSearchCV` explora `n_iter=20` combinações aleatórias de hiperparâmetros do `param_dist`.
    * `scoring='balanced_accuracy'`: A métrica usada para selecionar o melhor modelo é a acurácia balanceada, que é mais apropriada para dados desbalanceados (embora o oversampling já tenha sido feito, é uma boa prática).
    * O modelo é treinado (`.fit()`) nos dados de treino balanceados (`X_train_resampled`, `y_train_resampled`).
        ```python
        random_search = RandomizedSearchCV(
            gb_clf, param_dist, n_iter=20, cv=cv,
            scoring='balanced_accuracy', n_jobs=-1, verbose=1, random_state=42
        )
        random_search.fit(X_train_resampled, y_train_resampled)
        best_gb = random_search.best_estimator_
        ```
    * Os melhores hiperparâmetros encontrados e o tempo de execução são impressos.

* **Hiperparâmetros Selecionados (Exemplo da Saída):**
    Da saída fornecida, os melhores parâmetros encontrados pelo `RandomizedSearchCV` foram:
    `{'subsample': 0.8, 'n_estimators': 100, 'min_samples_split': 2, 'min_samples_leaf': 2, 'max_depth': 6, 'learning_rate': 0.2}`
    Estes são:
    * `subsample`: Fração de amostras usadas para ajustar as árvores individuais.
    * `n_estimators`: Número de árvores (estágios de boosting) a serem construídas.
    * `min_samples_split`: Número mínimo de amostras necessárias para dividir um nó interno.
    * `min_samples_leaf`: Número mínimo de amostras necessárias em um nó folha.
    * `max_depth`: Profundidade máxima das árvores de decisão individuais.
    * `learning_rate`: Taxa de aprendizado, encolhe a contribuição de cada árvore.

* **Treinamento do Melhor Modelo:** O `best_gb` (o `GradientBoostingClassifier` com os melhores hiperparâmetros encontrados) já foi treinado pelo `RandomizedSearchCV` nos dados de treino balanceados. Se a opção de parâmetros pré-definidos fosse escolhida, o `.fit()` seria chamado explicitamente.

#### **Realização de Previsões**

* Os dados de teste (`X_test`) são transformados usando o pré-processador já ajustado (`preprocessor.transform(X_test)`). Se a saída for uma matriz esparsa, ela é convertida para densa.
* As previsões são feitas no conjunto de teste transformado (`X_test_transformed`) usando o modelo treinado (`best_gb.predict()`).
    ```python
    X_test_transformed = preprocessor.transform(X_test)
    if scipy.sparse.issparse(X_test_transformed):
        X_test_transformed = X_test_transformed.toarray()
    y_pred = best_gb.predict(X_test_transformed)
    ```

#### **Avaliação do Modelo**

* **Métricas de Desempenho:**
    * **Acurácia:** (`accuracy_score`) A proporção de previsões corretas.
    * **Acurácia Balanceada:** (`balanced_accuracy_score`) A média das taxas de recall obtidas em cada classe. É útil para alvos desbalanceados, pois a acurácia simples pode ser enganosa.
    * **Relatório de Classificação:** (`classification_report`) Fornece as principais métricas de classificação (precision, recall, F1-score, support) para cada classe. `zero_division=0` evita avisos caso alguma métrica resulte em divisão por zero.
    * **Matriz de Confusão:** (`confusion_matrix`) Mostra o número de previsões corretas e incorretas para cada classe. É visualizada usando `sns.heatmap` e salva como `matriz_confusao.png`.
* **Interpretação (baseada na saída fornecida):**
    * Acurácia no teste: `0.5273` (52.73%)
    * Acurácia Balanceada no teste: `0.4015` (40.15%)
    * O relatório de classificação mostra que o modelo tem desempenho variado entre as classes. Por exemplo:
        * A classe "R$ 8.001/mês a R$ 16.000/mês" tem o melhor F1-score (0.66), com recall de 0.72.
        * A classe "Acima de R$ 30.000/mês" tem o pior desempenho (F1-score de 0.11).
    * A Acurácia Balanceada ser consideravelmente menor que a Acurácia simples sugere que o modelo ainda tem dificuldades com as classes minoritárias, mesmo após o oversampling (o desbalanceamento original no conjunto de teste ainda afeta a avaliação).

#### **Visualização da Árvore**

* Para um `GradientBoostingClassifier`, visualizar uma única árvore não é tão informativo quanto para um `DecisionTreeClassifier`, pois o modelo é um ensemble de muitas árvores. O código não tenta visualizar as árvores individuais do ensemble.
* A visualização mais relevante para o desempenho do modelo fornecida é a **matriz de confusão**.

#### **Salvando o Modelo e Componentes**

* O melhor modelo treinado (`best_gb`), o pré-processador (`preprocessor`) e o mapeamento do target (`target_mapping`) são salvos em arquivos `.pkl` usando `joblib.dump`. Isso permite que sejam recarregados e reutilizados posteriormente sem a necessidade de retreinar.
    ```python
    joblib.dump(best_gb, 'modelo_gradient_boosting_disparidade_salarial_otimizado.pkl')
    joblib.dump(preprocessor, 'preprocessador_otimizado.pkl')
    joblib.dump(target_mapping, 'target_mapping.pkl')
    ```

---

### 3. Estrutura da Explicação

Esta análise seguiu a estrutura solicitada, utilizando Markdown, cabeçalhos, listas e blocos de código para clareza.

---

### 4. Tom e Nível de Detalhe

A explicação buscou ser clara, tecnicamente precisa e detalhada, explicando o propósito de cada etapa do código.

---

### 5. Conclusão

* **Resumo:** O notebook desenvolve um modelo `GradientBoostingClassifier` para prever faixas salariais. As etapas incluem carregamento de dados, extenso pré-processamento (agrupamento de faixas salariais, codificação de variáveis categóricas, balanceamento de classes por oversampling), otimização de hiperparâmetros com `RandomizedSearchCV`, treinamento, avaliação e salvamento do modelo.
* **Possíveis Melhorias e Próximos Passos:**
    * **Engenharia de Features:** Explorar a criação de novas features a partir das existentes.
    * **Tratamento de Outliers:** A função `detect_outliers` foi definida, mas não aplicada. Avaliar o impacto da remoção ou tratamento de outliers nas features numéricas (se houvesse, ou se fossem criadas).
    * **Técnicas de Balanceamento Alternativas:** Experimentar outras técnicas como SMOTE (Synthetic Minority Over-sampling Technique) ou undersampling da classe majoritária, e avaliar seu impacto.
    * **Seleção de Features:** Utilizar técnicas como `permutation_importance` (que foi importada) ou RFE (Recursive Feature Elimination) para selecionar as features mais relevantes e potencialmente simplificar o modelo.
    * **Outros Modelos:** Comparar o desempenho do Gradient Boosting com outros algoritmos de classificação (ex: Random Forest, SVM, Redes Neurais).
    * **Análise de Erros:** Investigar mais a fundo por que o modelo tem dificuldade com certas classes (ex: "Acima de R$ 30.000/mês") e se há padrões nos erros.
    * **Validação Cruzada Mais Robusta:** Embora 3 folds tenham sido usados para otimização, uma validação cruzada mais extensa (e.g., 5 ou 10 folds) no processo de avaliação final do modelo escolhido poderia fornecer uma estimativa mais robusta do desempenho.
    * **Interpretabilidade do Modelo:** Usar ferramentas como SHAP (SHapley Additive exPlanations) para entender melhor as previsões do modelo Gradient Boosting e a importância das features de forma mais granular.
    * 
-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

# Resultados


*   [Resultados obtidos com os Modelos 1º pergunta orietada a dados](#resultados-obtidos-com-os-modelos-1º-pergunta-orietada-a-dados)
*   [Resultados obtidos com o modelo 1 da 1º pergunta orietada a dados](#resultados-obtidos-com-o-modelo-1-da-1º-pergunta-orietada-a-dados)
	*   [top3_features](#top3_features)
	*   [precision_recall_curve](#precision_recall_curve)
 	*   [matriz_confusao_otimizada](#matriz_confusao_otimizada) 
	*   [interacao_formacao_experiencia](#interacao_formacao_experiencia)
	*   [importancia_features_top20](#importancia_features_top20)
	*   [importancia_features_grupo_senioridade](#importancia_features_grupo_senioridade)
	*   [importancia_features_grupo_formacao](#importancia_features_grupo_formacao)
	*   [importancia_features_grupo_experiencia](#importancia_features_grupo_experiencia)
	*   [importancia_features_grupo_Área de formação acadêmica](#importancia_features_grupo_área-de-formação-acadêmica)
	*   [distribuicao_probabilidades](#distribuicao_probabilidades)
	*   [dispersao_top2_features](#dispersao_top2_features)
	*   [curva_roc_otimizada](#curva_roc_otimizada)
	*   [arvore_exemplo_simplificada](#arvore_exemplo_simplificada)
	*   [arvore_exemplo_melhorada](#arvore_exemplo_melhorada)

*   [Resultados obtidos com o modelo 2 da 1º pergunta orietada a dados](#resultados-obtidos-com-o-modelo-2-da-1º-pergunta-orietada-a-dados) 
	*   [matriz_confusao 1-2](#matriz_confusao_1_2)
	*   [distribuicao_faixas_salariais_originais 1-2](#distribuicao_faixas_salariais_originais_1_2)
 	*   [distribuicao_faixas_salariais_agrupadas 1-2](#distribuicao_faixas_salariais_agrupadas_1_2) 
	*   [correlacao_variaveis_faixa_salarial 1-2](#correlacao_variaveis_faixa_salarial_1_2)


# Resultados obtidos com os Modelos 1º pergunta orietada a dados

## Resultados obtidos com o modelo 1 da 1º pergunta orietada a dados


| Classe          | Precisão | Recall | F1-Score | Suporte |
|-----------------|----------|--------|----------|---------|
| Salário Baixo/Médio    | 0.84     | 0.84   | 0.84     | 568     |
| Salário Alto | 0.79     | 0.78   | 0.78     | 422     |
| accuracy |  |  | **0.82** | **990** |
| macro avg | **0.81** | **0.81** | **0.81** | **990** |
| weighted avg | **0.81** | **0.82** | **0.82** | **990** |

- Acurácia do Modelo: 0.82
- Acurácia do Modelo no Conjunto de Treinamento: -
- Acurácia do Modelo no Conjunto de Teste: -
- Diferença de Acurácia (Treino - Teste): -

## Métricas de Desempenho:

Com o limiar de classificação otimizado em 0.6, o modelo apresentou os seguintes resultados principais no conjunto de teste:

* **Acurácia Geral:** `0.82` (ou 82%)
* **Acurácia Balanceada:** `0.8106` (ou 81.06%)
* **F1-Score (Macro Avg):** `0.81`
* **F1-Score (Weighted Avg):** `0.82`

**Métricas por Classe (com limiar otimizado de 0.6):**

* **Salário Baixo/Médio (Classe 0):**
    * Precisão: `0.84`
    * Recall: `0.84`
    * F1-Score: `0.84`
    * Suporte (Número de amostras reais): 568
* **Salário Alto (Classe 1):**
    * Precisão: `0.79`
    * Recall: `0.78`
    * F1-Score: `0.78`
    * Suporte (Número de amostras reais): 422

**Matriz de Confusão (com limiar otimizado de 0.6):**
* Verdadeiros Negativos (TN - Previu Baixo/Médio, Real Baixo/Médio): 478
* Falsos Positivos (FP - Previu Alto, Real Baixo/Médio): 90
* Falsos Negativos (FN - Previu Baixo/Médio, Real Alto): 93
* Verdadeiros Positivos (TP - Previu Alto, Real Alto): 329

**Explicação das Métricas:**

* **Acurácia Geral:** Percentual de previsões corretas que o modelo fez no total. Neste caso, 82% das vezes o modelo acertou se um profissional teria um salário "Alto" ou "Baixo/Médio".
* **Acurácia Balanceada:** Média da proporção de acertos para cada classe individualmente. É uma métrica importante quando as classes têm tamanhos diferentes (desbalanceadas), como neste caso (57.35% Salário Baixo/Médio vs. 42.65% Salário Alto). Um valor de `0.8106` indica um bom equilíbrio no desempenho entre as classes.
* **Precisão (por classe):**
    * Para "Salário Baixo/Médio" (`0.84`): Das vezes que o modelo previu que um profissional teria um salário "Baixo/Médio", ele acertou em 84% dos casos.
    * Para "Salário Alto" (`0.79`): Das vezes que o modelo previu que um profissional teria um salário "Alto", ele acertou em 79% dos casos.
* **Recall (Sensibilidade, por classe):**
    * Para "Salário Baixo/Médio" (`0.84`): Dos profissionais que realmente têm salário "Baixo/Médio", o modelo conseguiu identificar corretamente 84% deles.
    * Para "Salário Alto" (`0.78`): Dos profissionais que realmente têm salário "Alto", o modelo conseguiu identificar corretamente 78% deles.
* **F1-Score (por classe e médias):** Média harmônica entre precisão e recall. É útil para ter uma única medida que resume a performance em ambas as métricas. Valores mais altos são melhores.
    * Um F1-Score de `0.84` para "Salário Baixo/Médio" e `0.78` para "Salário Alto" indicam um bom equilíbrio entre precisão e recall para ambas as classes, sendo ligeiramente melhor para a classe majoritária.
    * As médias "Macro Avg" (`0.81`) e "Weighted Avg" (`0.82`) fornecem um resumo geral do F1-Score considerando todas as classes.
* **Matriz de Confusão:** Mostra os acertos e erros do modelo em detalhe:
    * **TN (478):** O modelo previu corretamente 478 profissionais como "Salário Baixo/Médio".
    * **FP (90):** O modelo previu erroneamente 90 profissionais como "Salário Alto" quando na verdade eram "Salário Baixo/Médio".
    * **FN (93):** O modelo previu erroneamente 93 profissionais como "Salário Baixo/Médio" quando na verdade eram "Salário Alto".
    * **TP (329):** O modelo previu corretamente 329 profissionais como "Salário Alto".

## Interpretação dos Resultados:

O modelo Random Forest demonstrou um desempenho geral **bom** na tarefa de classificar profissionais de dados entre faixas salariais "Alto" e "Baixo/Médio".

* **Pontos Fortes:**
    * A acurácia geral de 82% e a acurácia balanceada de aproximadamente 81% indicam que o modelo é consistentemente bom em suas previsões, mesmo com um leve desbalanceamento nas classes originais.
    * O modelo apresenta um bom equilíbrio entre precisão e recall para a classe "Salário Baixo/Médio" (ambos `0.84`). Isso significa que ele é confiável ao prever essa classe e também consegue identificar a maioria dos pertencentes a ela.
    * A otimização do limiar para `0.6` (em vez do padrão `0.5`) foi crucial para alcançar a melhor acurácia balanceada, mostrando a importância de ajustar o ponto de corte da probabilidade para as necessidades específicas do problema e a distribuição das classes.

* **Pontos Fracos e Áreas para Melhoria:**
    * O desempenho para a classe "Salário Alto" (Precisão `0.79`, Recall `0.78`) é ligeiramente inferior ao da classe "Salário Baixo/Médio". Isso significa que há um pouco mais de erro ao prever salários altos, tanto em termos de previsões incorretas dessa classe (afetando a precisão) quanto em não conseguir identificar todos os que de fato têm salário alto (afetando o recall). Especificamente, 93 profissionais de salário alto foram classificados erroneamente como de salário baixo/médio (Falsos Negativos).
    * Ainda existem 90 casos onde o modelo previu "Salário Alto" mas era "Salário Baixo/Médio" (Falsos Positivos). Dependendo do objetivo de negócio, esses erros podem ter custos diferentes.

## Principais Insights e Observações:

* **Distribuição das Classes:** O dataset original apresentava um leve desbalanceamento, com 57.35% dos profissionais na categoria "Salário Baixo/Médio" e 42.65% em "Salário Alto". O uso de `class_weight='balanced_subsample'` nos hiperparâmetros do modelo e a otimização do limiar baseada na `balanced_accuracy` foram estratégias importantes para lidar com isso.
* **Busca de Hiperparâmetros:** O `GridSearchCV` testou 162 combinações de parâmetros em 5 validações cruzadas (totalizando 810 ajustes de modelo) para encontrar a configuração ótima: `{'class_weight': 'balanced_subsample', 'max_depth': None, 'min_samples_leaf': 7, 'min_samples_split': 15, 'n_estimators': 100}`. Isso indica um esforço robusto para otimizar o modelo.
* **Otimização do Limiar de Classificação:** A avaliação com diferentes limiares (`0.3` a `0.7`) mostrou que `0.6` forneceu a melhor `Acurácia Balanceada` (`0.8106`). Isso é um passo crucial, pois o limiar padrão de `0.5` nem sempre é o ideal, especialmente em classes desbalanceadas ou quando os custos de diferentes tipos de erros são assimétricos.
* **Impacto das Features:** Embora não detalhado nestes resultados numéricos, o código Python gera gráficos de importância de features. As features com maior impacto no modelo (como nível de ensino, tempo de experiência, área de formação, senioridade) seriam os principais impulsionadores da disparidade salarial identificada.
* **Salvamento de Gráficos:** Todos os gráficos gerados pela análise foram salvos no diretório `/kaggle/working/`, permitindo uma exploração visual mais aprofundada dos resultados.
* **Tempo de Treinamento/Inferência:** O log indica "Fitting 5 folds for each of 162 candidates, totalling 810 fits", o que, dependendo do tamanho do dataset e da complexidade, pode levar um tempo considerável para a busca de hiperparâmetros. O tempo de inferência para o modelo final (depois de treinado) em 990 amostras de teste costuma ser rápido para Random Forests.


### top3_features
![top3_features](https://github.com/user-attachments/assets/02f25d1b-4639-4cd9-a357-7a89297bff03)

O gráfico apresentado é um **diagrama de barras horizontais** que ilustra as **três características (features) mais influentes** que o modelo de machine learning utilizou para fazer suas previsões sobre a faixa salarial dos profissionais de dados. O título "Top 3 Features Mais Importantes" já nos indica seu propósito principal.

**Como Ler o Gráfico:**

* **Eixo Vertical (Features):** No lado esquerdo, temos o nome das três features mais relevantes identificadas pelo modelo:
    * `senioridade_encoded`
    * `experiencia_profissional_encoded`
    * `formacao_academica_encoded`
    *(Estas são as versões codificadas (transformadas em números) das características originais de nível de senioridade, tempo de experiência e formação acadêmica.)*

* **Eixo Horizontal (Importância Relativa):** Na parte inferior, temos a escala de "Importância Relativa". Esta escala vai de 0.00 até um valor um pouco acima de 0.40. Quanto maior a barra, maior a importância relativa daquela característica para as decisões do modelo.

* **Barras e Valores:** Cada barra colorida representa uma feature, e seu comprimento corresponde à sua importância. Os números ao final de cada barra indicam o valor exato dessa importância:
    * **`senioridade_encoded`:** A barra azul, a mais longa, tem uma importância relativa de aproximadamente **0.4053**. Isso significa que o nível de senioridade do profissional foi o fator individual mais forte que o modelo usou para diferenciar as faixas salariais.
    * **`experiencia_profissional_encoded`:** A barra laranja, a segunda mais longa, tem uma importância de **0.3588**. O tempo de experiência profissional é a segunda característica mais decisiva.
    * **`formacao_academica_encoded`:** A barra verde, a menor entre as três, possui uma importância de **0.0952**. Embora ainda esteja entre as três primeiras, a formação acadêmica teve um peso consideravelmente menor na definição da faixa salarial em comparação com a senioridade e a experiência, segundo este modelo.

**O que isso significa?**

Este gráfico nos diz que, para o modelo treinado, o **nível de senioridade** de um profissional de dados é o indicador mais poderoso para prever sua faixa salarial. Em seguida, vem o **tempo de experiência na área**. A **formação acadêmica**, apesar de relevante, aparece com uma influência menor quando comparada diretamente com os outros dois fatores dentro deste top 3.


### precision_recall_curve
![precision_recall_curve (1)](https://github.com/user-attachments/assets/c74124a4-f6b4-4592-9011-bba7013e93f4)

O gráfico apresentado é uma **Curva Precision-Recall**. Este tipo de gráfico é uma ferramenta visual importante para avaliar o desempenho de um modelo de classificação, especialmente quando as classes que o modelo tenta prever são desbalanceadas (ou seja, uma classe tem muito mais exemplos que a outra).

**Como Ler o Gráfico:**

* **Título:** "Curva Precision-Recall" indica o que o gráfico representa.
* **Eixo Vertical (Precision / Precisão):** Este eixo mede a "Precisão" do modelo e varia de aproximadamente 0.4 (40%) a 1.0 (100%).
    * **O que é Precisão?** De todas as vezes que o modelo previu um resultado positivo (por exemplo, "Salário Alto"), qual a porcentagem dessas previsões estava realmente correta? Uma precisão alta significa que quando o modelo diz que algo é positivo, ele geralmente está certo.
* **Eixo Horizontal (Recall / Revocação / Sensibilidade):** Este eixo mede o "Recall" do modelo e varia de 0.0 (0%) a 1.0 (100%).
    * **O que é Recall?** De todos os casos que eram *realmente* positivos (por exemplo, todos os profissionais que *realmente* têm "Salário Alto"), qual a porcentagem que o modelo conseguiu identificar corretamente? Um recall alto significa que o modelo encontra a maioria dos casos positivos existentes.
* **A Linha Azul:** A linha azul no gráfico traça a relação entre a precisão e o recall do modelo em diferentes "limiares de decisão".
    * **Limiar de Decisão:** Pense nisso como o nível de confiança que o modelo precisa ter para classificar algo como positivo. Se o limiar for muito alto, o modelo será muito cauteloso (alta precisão, mas pode perder alguns casos positivos, resultando em baixo recall). Se o limiar for muito baixo, o modelo identificará mais casos positivos (alto recall), mas também cometerá mais erros ao classificar casos negativos como positivos (baixa precisão).

**Interpretando a Curva:**

* **Trade-off entre Precisão e Recall:** A curva geralmente mostra um "trade-off" (uma troca) entre precisão e recall. Idealmente, gostaríamos que ambas as métricas fossem 100% (canto superior direito do gráfico), mas na prática, aumentar uma muitas vezes leva à diminuição da outra. Isso é visível no gráfico: à medida que o Recall aumenta (movendo-se para a direita no eixo horizontal), a Precisão tende a diminuir (a linha azul geralmente desce).
* **Formato da Curva:**
    * No início (lado esquerdo), quando o Recall é baixo (o modelo está identificando poucos dos verdadeiros positivos), a Precisão é alta (próxima de 1.0). Isso sugere que para os poucos casos que ele classifica como positivos, ele está muito certo.
    * À medida que o modelo tenta capturar mais dos verdadeiros positivos (Recall aumenta), a Precisão começa a cair. Vemos isso pela descida da linha azul. Por exemplo, quando o Recall está em torno de 0.8, a Precisão já caiu para perto de 0.7.
    * A queda se torna mais acentuada no final direito da curva, onde para alcançar um Recall muito alto (perto de 1.0), a Precisão cai significativamente para cerca de 0.4.
* **O que é um "bom" resultado?** Uma curva que se mantém o mais próximo possível do canto superior direito (alta precisão e alto recall simultaneamente) indica um modelo com melhor desempenho. Quanto mais a curva "abraça" o canto superior direito, melhor.

**O que este gráfico nos diz sobre o modelo?**

Este gráfico específico mostra que o modelo pode alcançar uma precisão muito alta (perto de 100%) se estivermos dispostos a aceitar um recall baixo (identificar apenas uma pequena fração dos verdadeiros positivos). Por outro lado, se quisermos que o modelo encontre quase todos os verdadeiros positivos (recall perto de 100%), a precisão cairá consideravelmente (para cerca de 40-50%).

A escolha do "melhor" ponto na curva (ou seja, o melhor limiar de decisão) depende do problema específico e de qual erro é mais custoso: classificar um negativo como positivo (erro de precisão) ou não conseguir identificar um positivo (erro de recall).

### matriz_confusao_otimizada
![matriz_confusao_otimizada (1)](https://github.com/user-attachments/assets/44b373ea-b840-4d47-afd7-804967449a49)

O gráfico apresentado é uma **Matriz de Confusão**. Este é um tipo de tabela que ajuda a visualizar o quão bem um modelo de machine learning está performando em uma tarefa de classificação. No caso deste modelo, ele está classificando profissionais entre duas categorias de salário: "Salário Baixo/Médio" e "Salário Alto". O título nos informa que estes resultados são do "Conjunto de Teste" (dados que o modelo não viu durante o treinamento) e que foi utilizado um "Limiar Otimizado" para a classificação.

**Como Ler o Gráfico:**

A matriz é dividida em quatro quadrantes principais, comparando os valores *verdadeiros* (a realidade) com os valores *previstos* pelo modelo:

* **Eixo Vertical (Rótulo "Verdadeiro"):** Mostra a classificação real dos profissionais.
    * Linha de cima: Profissionais que *realmente* têm "Salário Baixo/Médio".
    * Linha de baixo: Profissionais que *realmente* têm "Salário Alto".

* **Eixo Horizontal (Rótulo "Previsto"):** Mostra o que o modelo *previu* para esses profissionais.
    * Coluna da esquerda: O modelo previu "Salário Baixo/Médio".
    * Coluna da direita: O modelo previu "Salário Alto".

**Interpretando os Quadrantes:**

1.  **Quadrante Superior Esquerdo (Valor: 478):**
    * **Verdadeiro:** Salário Baixo/Médio
    * **Previsto:** Salário Baixo/Médio
    * **Significado:** O modelo acertou! Ele classificou corretamente 478 profissionais que realmente têm salário baixo/médio como tendo salário baixo/médio. Estes são os **Verdadeiros Negativos (TN)**, assumindo "Salário Alto" como a classe positiva.

2.  **Quadrante Superior Direito (Valor: 90):**
    * **Verdadeiro:** Salário Baixo/Médio
    * **Previsto:** Salário Alto
    * **Significado:** O modelo errou. Ele classificou 90 profissionais que realmente têm salário baixo/médio como se tivessem salário alto. Estes são os **Falsos Positivos (FP)** – o modelo "positivou" erroneamente para salário alto.

3.  **Quadrante Inferior Esquerdo (Valor: 93):**
    * **Verdadeiro:** Salário Alto
    * **Previsto:** Salário Baixo/Médio
    * **Significado:** O modelo errou. Ele classificou 93 profissionais que realmente têm salário alto como se tivessem salário baixo/médio. Estes são os **Falsos Negativos (FN)** – o modelo "negou" erroneamente a presença de um salário alto.

4.  **Quadrante Inferior Direito (Valor: 329):**
    * **Verdadeiro:** Salário Alto
    * **Previsto:** Salário Alto
    * **Significado:** O modelo acertou! Ele classificou corretamente 329 profissionais que realmente têm salário alto como tendo salário alto. Estes são os **Verdadeiros Positivos (TP)**.

**Cores:**
A intensidade da cor azul nos quadrantes geralmente corresponde ao número de instâncias. Quadrantes com números maiores (como 478 e 329, que são os acertos) são mais escuros, enquanto quadrantes com números menores (como 90 e 93, que são os erros) são mais claros.

**O que este gráfico nos diz sobre o modelo?**

* **Acertos:** O modelo acertou um bom número de previsões, como indicado pelos valores na diagonal principal (478 e 329).
* **Tipos de Erros:**
    * Ele cometeu 90 erros do tipo "Falso Positivo" (achou que era salário alto, mas não era).
    * Ele cometeu 93 erros do tipo "Falso Negativo" (não identificou um salário alto que era real).
* **Desempenho Geral:** A matriz de confusão permite uma análise detalhada de onde o modelo está acertando e onde está errando. Idealmente, os números na diagonal principal (acertos) seriam os maiores possíveis, e os números fora da diagonal (erros) seriam os menores possíveis.

### interacao_formacao_experiencia
![interacao_formacao_experiencia (1)](https://github.com/user-attachments/assets/c6c03e66-554e-42db-a435-e5e909bb9857)

O gráfico apresentado é um **mapa de calor (heatmap)**. Ele mostra visualmente como a combinação do **nível de formação acadêmica** e do **tempo de experiência profissional** influencia a **probabilidade de um profissional ter um salário considerado alto**.

**Como Ler o Gráfico:**

* **Título:** "Probabilidade de Salário Alto por Formação Acadêmica e Experiência Profissional" indica claramente o que o gráfico está medindo.
* **Eixo Vertical (Nível de Formação):** Lista os diferentes níveis de escolaridade, desde "Estudante de Graduação" no topo até "Doutorado ou Phd" na base.
* **Eixo Horizontal (Tempo de Experiência):** Apresenta faixas de tempo de experiência profissional, começando com "Menos de 1 ano" à esquerda e indo até "de 7 a 10 anos" à direita.
* **Células e Números:** Cada "quadradinho" (célula) no gráfico representa a intersecção de um nível de formação específico com uma faixa de tempo de experiência. O número dentro de cada célula (por exemplo, 0.01, 0.61, 0.94) é a **probabilidade estimada** de um profissional com aquela combinação de formação e experiência ter um salário alto. Uma probabilidade de 0.01 significa 1% de chance, enquanto 0.94 significa 94% de chance.
* **Escala de Cores (Barra à Direita):** A barra vertical à direita é a legenda das cores. As cores no mapa de calor correspondem a essas probabilidades:
    * **Cores escuras (roxo/azul escuro):** Indicam uma baixa probabilidade de ter salário alto.
    * **Cores claras (verde, amarelo):** Indicam uma alta probabilidade de ter salário alto.
    Quanto mais clara/amarela a cor, maior a chance.

**Interpretando as Tendências e Insights do Gráfico:**

1.  **Impacto da Experiência (Movendo da Esquerda para a Direita):**
    * Para qualquer nível de formação, de modo geral, **quanto maior o tempo de experiência, maior a probabilidade de ter um salário alto.** Isso é visível porque, ao seguir uma linha horizontal (mesmo nível de formação), as cores tendem a ficar mais claras/amarelas à medida que você se move para a direita.
    * Por exemplo, para um "Graduação/Bacharelado":
        * Com "Menos de 1 ano" de experiência, a probabilidade é baixa (0.06 ou 6%).
        * Com "de 7 a 10 anos" de experiência, a probabilidade sobe consideravelmente (0.74 ou 74%).

2.  **Impacto da Formação Acadêmica (Movendo de Cima para Baixo):**
    * Para qualquer faixa de experiência (especialmente após alguns anos), **quanto maior o nível de formação acadêmica, maior a probabilidade de ter um salário alto.** Isso é notado porque, ao seguir uma coluna vertical (mesmo tempo de experiência), as cores geralmente se tornam mais claras/amarelas à medida que você desce.
    * Por exemplo, com "de 3 a 4 anos" de experiência:
        * Um "Estudante de Graduação" tem 0.23 (23%) de probabilidade.
        * Um "Doutorado ou Phd" tem 0.89 (89%) de probabilidade.

3.  **Interação entre Formação e Experiência (O Ponto Crucial):**
    * O gráfico demonstra que não é apenas um fator isolado, mas a **combinação** de formação e experiência que mais fortemente influencia a probabilidade de um salário alto.
    * Profissionais com **níveis mais altos de formação E mais tempo de experiência** (canto inferior direito do gráfico) são os que apresentam as maiores probabilidades de terem salários altos (cores mais amarelas, com probabilidades como 0.91, 0.92, 0.94).
    * Por outro lado, aqueles com **baixa formação E pouca experiência** (canto superior esquerdo) têm as menores probabilidades (cores mais escuras, com probabilidades como 0.01, 0.06).
    * É interessante notar que, em alguns casos, muita experiência pode compensar um nível de formação um pouco menor. Por exemplo, um "Estudante de Graduação" com "de 7 a 10 anos" de experiência (0.67) tem uma probabilidade maior de salário alto do que um "Mestrado" com "Menos de 1 ano" de experiência (0.04).


### importancia_features_top20
![importancia_features_top20](https://github.com/user-attachments/assets/cbfc487f-4a48-45e1-8a0a-b5ccdf0b2bb5)

O gráfico apresentado é um **diagrama de barras horizontais** que mostra as **20 características (features) consideradas mais importantes** pelo modelo Random Forest para fazer suas previsões sobre a faixa salarial. O título "Importância das 20 Features Mais Relevantes (Random Forest)" resume seu objetivo.

**Como Ler o Gráfico:**

* **Eixo Vertical (Features):** No lado esquerdo, estão listados os nomes das 20 features que mais influenciaram o modelo. Elas estão ordenadas da menos importante (no topo das 20) para a mais importante (na base das 20).
    * Vemos features como `senioridade_encoded`, `experiencia_profissional_encoded`, `formacao_academica_encoded` (que já vimos serem as top 3), e outras como `UF onde mora_SP` (indicando se a pessoa mora em São Paulo), `Setor de atuação da empresa_Finanças ou Bancos`, `Área de formação acadêmica_Computação / Engenharia de Software / Sistemas de Informação / TI`, entre outras.
* **Eixo Horizontal (Importância Relativa):** Na parte inferior, a escala de "Importância Relativa" varia de 0.00 a pouco mais de 0.40. Quanto maior a barra para uma feature, maior sua importância para as decisões tomadas pelo modelo.
* **Barras Azuis:** Cada barra azul representa uma feature, e seu comprimento é proporcional à sua importância relativa.

**Interpretando as Informações do Gráfico:**

1.  **As Campeãs de Importância:**
    * As três barras na parte inferior do gráfico (`senioridade_encoded`, `experiencia_profissional_encoded` e `formacao_academica_encoded`) são significativamente mais longas que todas as outras. Isso confirma que o **nível de senioridade**, o **tempo de experiência profissional** e o **nível de formação acadêmica codificado** são, de longe, os fatores mais decisivos que o modelo utiliza para prever a faixa salarial.
    * `senioridade_encoded` é a mais importante, com um valor de importância relativa em torno de 0.40.
    * `experiencia_profissional_encoded` vem em seguida, com importância em torno de 0.35.
    * `formacao_academica_encoded` tem uma importância próxima a 0.10.

2.  **As Demais Features Relevantes:**
    * Após as três primeiras, há uma queda acentuada na importância. As 17 features restantes têm uma influência consideravelmente menor, com barras muito mais curtas.
    * Entre estas, encontramos:
        * **Localização:** `UF onde mora_SP` (morar em São Paulo) aparece como a quarta feature mais importante, embora com um peso bem menor que as três primeiras. Outras UFs como RJ, PR, RS, DF também figuram na lista, indicando que a localização geográfica tem alguma influência.
        * **Setor de Atuação da Empresa:** Características como `Setor de atuação da empresa_Finanças ou Bancos`, `Setor de atuação da empresa_Tecnologia/Fábrica de Software`, `Setor de atuação da empresa_Area de Consultoria` também são consideradas pelo modelo, sugerindo que o setor onde o profissional trabalha impacta a previsão salarial.
        * **Área de Formação Específica:** Além do nível de formação (já no top 3), a área específica da formação também contribui, como `Área de formação acadêmica_Computação / Engenharia de Software / Sistemas de Informação / TI` e `Área de formação acadêmica_Economia/ Administração / Contabilidade / Finanças/ Negócios`.

3.  **O Conceito de "Importância Relativa":**
    * Os valores no eixo horizontal não são, por exemplo, percentagens diretas do salário, mas sim uma medida de quanto cada feature contribuiu para reduzir a impureza (ou aumentar a precisão) nas árvores de decisão que compõem o modelo Random Forest. A soma de todas as importâncias de todas as features (não apenas as 20 mostradas) seria 1.0 (ou 100%).

**O que este gráfico nos diz sobre o modelo?**

Este gráfico é fundamental para entender "o que o modelo está pensando". Ele revela que, embora muitas características sejam consideradas, um pequeno grupo delas (senioridade, experiência e nível de formação) domina o processo de decisão para prever salários. As outras 17 features mostradas, como localização, setor da empresa e área de formação específica, adicionam nuances e refinamentos à previsão, mas têm um papel secundário em comparação com os três principais fatores.

### importancia_features_grupo_senioridade
![importancia_features_grupo_senioridade](https://github.com/user-attachments/assets/88a8e6a4-5bff-4e58-a613-523fe4915bed)

**Como Ler o Gráfico:**

* **Eixo Vertical (Feature):** No lado esquerdo, vemos apenas uma característica listada: `senioridade_encoded`. Este é o nome da feature que representa o nível de senioridade do profissional, após ter sido codificada (transformada em um formato numérico que o modelo pode entender).
* **Eixo Horizontal (Importância Relativa):** Na parte inferior, a escala de "Importância Relativa" vai de 0.00 até um valor um pouco acima de 0.40.
* **Barra Verde:** Há uma única e longa barra verde que corresponde à feature `senioridade_encoded`. O comprimento desta barra indica o quão importante essa característica é para as previsões de faixa salarial feitas pelo modelo.

**Interpretando as Informações do Gráfico:**

1.  **Foco na Senioridade Codificada:**
    * O gráfico isola a feature `senioridade_encoded`. Isso sugere que a informação original sobre o nível de senioridade (por exemplo, Júnior, Pleno, Sênior) foi transformada em uma única variável numérica (`senioridade_encoded`) para o modelo.

2.  **Alta Importância Confirmada:**
    * A barra se estende até um valor de importância relativa de aproximadamente **0.4053** (este valor exato foi visto em outros gráficos de importância geral, como o "Top 3 Features").
    * Este valor é bastante alto, especialmente quando comparado com a importância de muitas outras características individuais (como os estados ou setores de atuação vistos em gráficos anteriores).

3.  **O que significa "Grupo senioridade" neste contexto?**
    * Diferentemente dos gráficos de "Grupo UF onde mora" ou "Grupo Setor de atuação da empresa", onde várias features dentro do grupo eram comparadas (por exemplo, diferentes UFs ou diferentes setores), aqui o "Grupo senioridade" parece se referir apenas a esta única feature consolidada.
    * Isso reforça que a senioridade, como um todo, foi tratada como um conceito único e poderoso pelo modelo.

**O que este gráfico nos diz sobre o modelo?**

Este gráfico serve para enfatizar de forma isolada e clara o **peso significativo que a senioridade (codificada) tem nas previsões do modelo**. Ele reitera que, de todas as informações fornecidas ao modelo, o nível de senioridade de um profissional é um dos indicadores mais fortes e influentes para determinar sua faixa salarial.


### importancia_features_grupo_formacao
![importancia_features_grupo_formacao](https://github.com/user-attachments/assets/e9180d58-b603-4e09-9f57-a94ecc4d824f)

**Como Ler o Gráfico:**

* **Eixo Vertical (Feature):** No lado esquerdo, é listada apenas uma característica: `formacao_academica_encoded`. Este é o nome da feature que representa o nível de formação acadêmica do profissional, após ter sido codificada (ou seja, transformada em um valor numérico que o modelo pode processar).
* **Eixo Horizontal (Importância Relativa):** Na parte inferior, a escala de "Importância Relativa" varia de 0.00 até 0.10.
* **Barra Verde:** Existe uma única e proeminente barra verde que corresponde à feature `formacao_academica_encoded`. O comprimento desta barra indica o peso ou a influência que esta característica tem nas previsões de faixa salarial feitas pelo modelo.

**Interpretando as Informações do Gráfico:**

1.  **Foco na Formação Acadêmica Codificada:**
    * O gráfico isola a feature `formacao_academica_encoded`. Isso sugere que a informação original sobre o nível de formação acadêmica (por exemplo, Graduação, Pós-graduação, Mestrado, Doutorado, etc.) foi consolidada e transformada em uma única variável numérica (`formacao_academica_encoded`) que foi utilizada pelo modelo.

2.  **Importância Significativa:**
    * A barra se estende até um valor de importância relativa de aproximadamente **0.0952**. Embora este valor seja menor do que os observados para `senioridade_encoded` (próximo a 0.4053) e `experiencia_profissional_encoded` (próximo a 0.3588) em outros gráficos, ele ainda representa a terceira característica mais importante no geral para o modelo.
    * Isso indica que, após a senioridade e a experiência, o nível de formação acadêmica é o próximo fator mais influente nas previsões salariais.

3.  **O que significa "Grupo formacao" neste contexto?**
    * Assim como no gráfico do "Grupo senioridade", o "Grupo formacao" aqui se refere a esta única feature consolidada, `formacao_academica_encoded`.
    * Isso não é uma comparação entre diferentes aspectos da formação, mas sim uma maneira de destacar a importância total atribuída ao conceito de "nível de formação acadêmica" da forma como foi processado e incluído no modelo.

**O que este gráfico nos diz sobre o modelo?**

Este gráfico simples, mas direto, serve para reforçar que o **nível de formação acadêmica (codificado) dos profissionais é uma variável com impacto considerável nas previsões do modelo** sobre suas faixas salariais. Embora não seja tão dominante quanto a senioridade ou a experiência profissional, a formação acadêmica ainda se destaca como um dos principais fatores levados em conta pelo modelo.

### importancia_features_grupo_experiencia
![importancia_features_grupo_experiencia](https://github.com/user-attachments/assets/bffd0e4f-bc56-42d1-802c-ea1b22b872b7)

**Como Ler o Gráfico:**

* **Eixo Vertical (Feature):** À esquerda, é apresentada apenas uma característica: `experiencia_profissional_encoded`. Este é o nome da feature que representa o tempo ou nível de experiência profissional, após ter sido codificada (transformada em um valor numérico que o modelo pode utilizar).
* **Eixo Horizontal (Importância Relativa):** Na parte inferior, a escala de "Importância Relativa" se estende de 0.00 até um valor um pouco acima de 0.35.
* **Barra Verde:** Há uma única e muito longa barra verde. Seu comprimento corresponde diretamente à importância da feature `experiencia_profissional_encoded` para as previsões de faixa salarial feitas pelo modelo.

**Interpretando as Informações do Gráfico:**

1.  **Foco na Experiência Profissional Codificada:**
    * O gráfico isola a feature `experiencia_profissional_encoded`. Isso indica que a informação original sobre o tempo de experiência profissional (por exemplo, "Menos de 1 ano", "de 1 a 2 anos", etc.) foi transformada em uma única variável numérica (`experiencia_profissional_encoded`) para ser usada pelo modelo.

2.  **Importância Muito Elevada:**
    * A barra se estende até um valor de importância relativa de aproximadamente **0.3588**. Este valor é substancial e, conforme visto em gráficos anteriores (como o "Top 3 Features"), posiciona a experiência profissional como a segunda característica mais importante para o modelo, ficando atrás apenas da senioridade.

3.  **Significado de "Grupo experiencia" neste Contexto:**
    * Assim como nos gráficos de "Grupo senioridade" e "Grupo formacao", o "Grupo experiencia" aqui se refere a esta única feature consolidada.
    * Não se trata de uma comparação entre diferentes facetas da experiência, mas sim de uma forma de destacar a importância total atribuída ao conceito de "experiência profissional" da maneira como foi processado e incluído no modelo.

**O que este gráfico nos diz sobre o modelo?**

Este gráfico, embora simples por apresentar uma única barra, serve para enfatizar de forma clara e inequívoca o **peso extremamente significativo que a experiência profissional (codificada) tem nas previsões do modelo**. Ele confirma que, entre todas as informações fornecidas, o nível de experiência profissional de um indivíduo é um dos indicadores mais fortes e decisivos para determinar sua faixa salarial.

### importancia_features_grupo_Área de formação acadêmica
![importancia_features_grupo_Área de formação acadêmica](https://github.com/user-attachments/assets/17e5dd69-f141-4fc0-b0e5-fbb180912aeb)

O gráfico apresentado é um **gráfico de barras horizontais** que ilustra a **importância relativa** de diferentes subcategorias dentro do grupo "Área de formação acadêmica" para um modelo de machine learning. O título "Importância das Features: Grupo Área de formação acadêmica" indica que o gráfico foca em detalhar a relevância de cada área específica de formação.

**Como interpretar o gráfico:**

* **Eixo Y (Vertical):** Lista as diferentes áreas de formação acadêmica que foram consideradas como features (características) pelo modelo. Por exemplo, "Área de formação acadêmica_Ciências Sociais", "Área de formação acadêmica_Marketing / Publicidade / Comunicação / Jornalismo", etc.
* **Eixo X (Horizontal):** Representa a "Importância Relativa" de cada uma dessas áreas. Quanto maior a barra, maior a importância relativa daquela área de formação para as previsões feitas pelo modelo. Os valores no eixo X (ex: 0.000, 0.002, ..., 0.012) indicam a magnitude dessa importância.
* **Barras:** O comprimento de cada barra horizontal é proporcional à importância relativa da área de formação correspondente.

**Análise das Features Apresentadas (da mais importante para a menos importante, visualmente):**

1.  **Área de formação acadêmica_Economia/ Administração / Contabilidade / Finanças/ Negócios:** É a área com a **maior importância relativa** (aproximadamente 0.011).
2.  **Área de formação acadêmica_Computação / Engenharia de Software / Sistemas de Informação/ TI:** Possui a segunda maior importância (aproximadamente 0.009).
3.  **Área de formação acadêmica_Outras Engenharias:** Apresenta uma importância considerável (aproximadamente 0.007).
4.  **Área de formação acadêmica_Outra opção:** Segue com uma importância relativa em torno de 0.005.
5.  **Área de formação acadêmica_Estatística/ Matemática / Matemática Computacional/ Ciências Atuariais:** Mostra uma importância de aproximadamente 0.0035.
6.  **Área de formação acadêmica_Química / Física:** Tem uma importância menor (aproximadamente 0.0015).
7.  **Área de formação acadêmica_Ciências Biológicas/ Farmácia/ Medicina/ Área da Saúde:** Apresenta uma importância similar à anterior (aproximadamente 0.0015).
8.  **Área de formação acadêmica_Marketing / Publicidade / Comunicação / Jornalismo:** Possui uma baixa importância relativa (aproximadamente 0.001).
9.  **Área de formação acadêmica_Ciências Sociais:** É a área com a **menor importância relativa** entre as listadas (muito próxima de 0.0005).

### distribuicao_probabilidades
![distribuicao_probabilidades (1)](https://github.com/user-attachments/assets/f7ed3668-f41f-486f-87bd-dbac9fcd74f1)

O gráfico apresentado é um **histograma** com uma curva de estimativa de densidade do kernel (KDE) sobreposta, intitulado "Distribuição das Probabilidades Preditas". Ele mostra como as probabilidades preditas pelo modelo para a classe "Salário Alto" estão distribuídas.

**Como interpretar o gráfico:**

* **Eixo X (Horizontal):** "Probabilidade de Salário Alto". Este eixo varia de 0.0 a 1.0 e representa a confiança do modelo de que uma determinada instância pertence à classe "Salário Alto".
    * Um valor próximo de 0.0 significa que o modelo prevê uma baixa probabilidade de a instância ter um salário alto.
    * Um valor próximo de 1.0 significa que o modelo prevê uma alta probabilidade de a instância ter um salário alto.
* **Eixo Y (Vertical):** "Contagem". Este eixo indica o número de previsões (instâncias) que caem em cada intervalo de probabilidade (as barras do histograma).
* **Barras do Histograma:** Cada barra representa um intervalo de probabilidades preditas, e a altura da barra mostra quantas previsões do modelo caíram nesse intervalo específico.
* **Curva Azul:** É uma estimativa de densidade do kernel (KDE), que fornece uma representação suavizada da distribuição das probabilidades preditas. Ajuda a visualizar a forma geral da distribuição.
* **Linha Tracejada Vermelha Vertical:** Identificada na legenda como "Limiar Ótimo = 0.6". Este é um limiar (threshold) escolhido para classificar as instâncias.
    * Previsões com probabilidade de salário alto **maior ou igual a 0.6** seriam classificadas como pertencentes à classe "Salário Alto".
    * Previsões com probabilidade **menor que 0.6** seriam classificadas como "Não Salário Alto" (ou a classe oposta).

**Análise da Distribuição:**

* **Concentração nas Extremidades:** Observa-se uma alta concentração de previsões com probabilidades muito baixas (próximas de 0.0). A barra mais alta do histograma está no extremo esquerdo, indicando que muitas instâncias receberam uma probabilidade muito baixa de terem um salário alto.
* **Outro Pico em Altas Probabilidades:** Há também um acúmulo significativo de previsões com probabilidades altas, especialmente entre 0.9 e 1.0, embora menor que o pico em 0.0.
* **Menor Contagem no Meio:** Existem menos previsões com probabilidades na faixa intermediária (por exemplo, entre 0.3 e 0.5, e entre 0.6 e 0.7, excluindo o limiar). Isso sugere que o modelo, em muitos casos, está razoavelmente "decidido" sobre a classe, atribuindo probabilidades mais extremas.
* **Impacto do Limiar (0.6):**
    * A maioria das previsões à esquerda do limiar de 0.6 seriam classificadas como "Não Salário Alto".
    * As previsões à direita do limiar (probabilidade >= 0.6) seriam classificadas como "Salário Alto". O gráfico mostra que um número considerável de instâncias se qualifica para esta classe com base neste limiar, especialmente aquelas com probabilidades entre 0.9 e 1.0.


### dispersao_top2_features
![dispersao_top2_features](https://github.com/user-attachments/assets/99eb2c9f-d3ef-47d7-b337-5431c00d0571)

O gráfico apresentado é um **diagrama de dispersão (scatter plot)** intitulado "Relação entre as Duas Features Mais Importantes: senioridade_encoded vs experiencia_profissional_encoded". Ele visualiza como as duas características consideradas mais importantes pelo modelo – senioridade e experiência profissional (ambas codificadas numericamente) – se relacionam com a probabilidade predita de um indivíduo ter um salário alto.

**Como interpretar o gráfico:**

* **Eixo X (Horizontal):** "senioridade_encoded". Representa os diferentes níveis de senioridade, que foram convertidos para um formato numérico (codificado). Valores maiores neste eixo provavelmente correspondem a níveis de senioridade mais altos.
* **Eixo Y (Vertical):** "experiencia_profissional_encoded". Representa os diferentes níveis de experiência profissional, também codificados numericamente. Valores maiores neste eixo provavelmente indicam mais anos ou níveis de experiência.
* **Pontos no Gráfico:** Cada ponto representa uma combinação específica de `senioridade_encoded` e `experiencia_profissional_encoded` observada nos dados.
* **Escala de Cores (Barra Lateral):** "Probabilidade de Salário Alto". Esta barra de cores, variando do azul (0.0) ao vermelho (1.0), indica a probabilidade predita pelo modelo de um indivíduo ter um salário alto.
    * **Pontos azuis/roxos:** Baixa probabilidade de salário alto.
    * **Pontos vermelhos/laranjas:** Alta probabilidade de salário alto.

**Análise das Relações e Padrões Visíveis:**

* **Impacto da Senioridade:** Observa-se uma tendência clara de que, à medida que `senioridade_encoded` aumenta (movendo da esquerda para a direita no gráfico), a cor dos pontos tende a mudar de azul para vermelho. Isso sugere que níveis mais altos de senioridade estão associados a uma maior probabilidade de ter um salário alto.
    * Por exemplo, os pontos com `senioridade_encoded = 2.00` são predominantemente vermelhos ou laranjas, indicando altas probabilidades de salário alto.
    * Em contraste, os pontos com `senioridade_encoded = 0.00` são todos azuis ou roxos, indicando baixas probabilidades.

* **Impacto da Experiência Profissional:** Similarmente, para um dado nível de senioridade, um aumento em `experiencia_profissional_encoded` (movendo de baixo para cima no gráfico) também tende a aumentar a probabilidade de salário alto.
    * Por exemplo, para `senioridade_encoded = 2.00`:
        * Com `experiencia_profissional_encoded = 0.0`, o ponto é laranja claro (probabilidade moderada-alta).
        * Com `experiencia_profissional_encoded = 4.0`, o ponto é vermelho escuro (probabilidade muito alta).

* **Combinação de Fatores:** O efeito mais forte (maior probabilidade de salário alto) é observado quando ambos, senioridade e experiência profissional, são altos. O ponto no canto superior direito (`senioridade_encoded = 2.00`, `experiencia_profissional_encoded = 4.0`) é o mais vermelho, indicando a maior probabilidade predita de salário alto.

* **Valores Codificados:** Os valores nos eixos parecem ser discretos (ex: 0.00, 1.00, 2.00 para senioridade; 0.0, 1.0, 2.0, 3.0, 4.0 para experiência). Isso é consistente com a ideia de que estas são features categóricas que foram codificadas numericamente para uso no modelo.

### curva_roc_otimizada
![curva_roc_otimizada (1)](https://github.com/user-attachments/assets/2bd509b0-24c8-46ad-9bb0-b18203609795)

O gráfico apresentado é uma **Curva ROC (Receiver Operating Characteristic)**, uma ferramenta fundamental para avaliar o desempenho de modelos de classificação binária. O título "Curva ROC com Limiar Otimizado" indica que, além da curva em si, um limiar específico considerado ótimo é destacado.

**Como interpretar o gráfico:**

* **Eixo X (Horizontal): Taxa de Falsos Positivos (FPR - False Positive Rate)**
    * Também conhecida como (1 - Especificidade).
    * Representa a proporção de instâncias negativas que foram incorretamente classificadas como positivas pelo modelo.
    * Valores mais baixos de FPR são melhores (menos alarmes falsos).

* **Eixo Y (Vertical): Taxa de Verdadeiros Positivos (TPR - True Positive Rate)**
    * Também conhecida como Sensibilidade ou Recall.
    * Representa a proporção de instâncias positivas que foram corretamente classificadas como positivas pelo modelo.
    * Valores mais altos de TPR são melhores (mais acertos corretos dos positivos).

* **Curva ROC (Laranja):**
    * Esta curva ilustra o desempenho do modelo de classificação em todos os limiares de classificação possíveis. Cada ponto na curva ROC representa um par (FPR, TPR) correspondente a um determinado limiar.
    * Um modelo ideal teria uma curva que sobe rapidamente em direção ao canto superior esquerdo do gráfico (TPR = 1, FPR = 0). Quanto mais a curva se aproxima desse canto, melhor o desempenho do modelo.

* **AUC (Area Under the Curve) = 0.88:**
    * A Área Sob a Curva ROC (AUC) é uma medida agregada do desempenho do modelo em todos os limiares.
    * A AUC varia de 0 a 1:
        * AUC = 0.5: O modelo não tem capacidade de discriminação (equivalente a um classificador aleatório).
        * AUC > 0.5: O modelo tem alguma capacidade de discriminação.
        * AUC = 1.0: O modelo é um classificador perfeito.
    * Um valor de **AUC = 0.88** indica um bom desempenho do modelo, significando que há uma probabilidade de 88% de que o modelo classifique corretamente uma instância positiva escolhida aleatoriamente como mais provável de ser positiva do que uma instância negativa escolhida aleatoriamente.

* **Linha Diagonal Tracejada (Azul Escuro):**
    * Representa o desempenho de um classificador aleatório (que não tem poder de discriminação). A Curva ROC de um bom modelo deve estar significativamente acima desta linha.

* **Linha Vertical Tracejada (Verde): Limiar Ótimo = 0.6**
    * Esta linha vertical indica um limiar específico (threshold) de 0.6 que foi escolhido como "ótimo" para este modelo, possivelmente com base em algum critério de otimização (como maximizar o índice de Youden, ou balancear TPR e FPR de acordo com as necessidades do problema).
    * O ponto onde esta linha verde intercepta a Curva ROC laranja mostra o desempenho do modelo (o par TPR e FPR) quando este limiar de 0.6 é usado para classificar as instâncias. Visualmente, para este limiar de 0.6, o FPR é baixo (aproximadamente 0.08) e o TPR é considerável (aproximadamente 0.65).

**Análise do Desempenho:**

* A Curva ROC laranja está bem acima da linha diagonal, e o valor de AUC de 0.88 confirma que o modelo tem um bom poder de discriminação entre as classes positiva e negativa.
* A escolha do "Limiar Ótimo = 0.6" resulta em uma baixa taxa de falsos positivos (poucos negativos classificados erroneamente como positivos) e uma taxa de verdadeiros positivos razoavelmente alta (uma boa proporção dos positivos reais são identificados corretamente). A adequação deste limiar depende do contexto específico do problema e dos custos associados a falsos positivos versus falsos negativos.


### arvore_exemplo_simplificada
![arvore_exemplo_simplificada](https://github.com/user-attachments/assets/a4d395fd-d40a-43e0-a655-1cc5eece761e)

O gráfico apresentado é uma **visualização de uma única árvore de decisão**, extraída de um modelo mais complexo chamado **Random Forest**. Um Random Forest é um conjunto (ou "floresta") de múltiplas árvores de decisão, onde cada árvore contribui para a predição final. Esta visualização simplificada nos ajuda a entender como uma dessas árvores toma decisões para classificar os dados.

---

**Como interpretar os componentes da árvore:**

* **Nós (Retângulos):** Cada retângulo é um nó na árvore.
    * **Nós de Decisão (Nós Internos):** São os retângulos que têm ramificações (setas) saindo deles. Eles contêm uma condição baseada em uma das *features* (características) dos dados.
        * **Condição de Divisão:** A primeira linha no nó de decisão (ex: `experiencia_profissional_encoded <= 1.5`). Esta é a pergunta que a árvore faz sobre uma amostra de dados. Se a condição for verdadeira, a amostra segue para o galho da esquerda; se for falsa, para o galho da direita.
        * `gini`: O **Índice de Gini** é uma medida de impureza do nó. Um valor de Gini igual a 0 significa que o nó é perfeitamente puro (todas as amostras nesse nó pertencem à mesma classe). Quanto maior o Gini, mais misturadas estão as classes no nó.
        * `samples`: O número de amostras de treinamento que alcançaram este nó.
        * `value`: Mostra a distribuição das amostras entre as diferentes classes possíveis dentro daquele nó. Por exemplo, `value = [100, 632, 267, 722]` no segundo nó da esquerda indica como as amostras estão distribuídas entre as classes (o número de classes e sua ordem dependeriam da codificação do problema).
        * `class`: Indica a classe majoritária entre as amostras presentes naquele nó. Se este fosse um nó folha, essa seria a predição da árvore para as amostras que chegam até ele.
    * **Nós Folha (Nós Terminais):** São os nós no final das ramificações, onde não há mais divisões. Eles representam a predição final para qualquer amostra que percorra o caminho até eles.
        * Neste gráfico, os nós cinzas com `(...)` no final indicam que a árvore continua, mas foi **truncada ou simplificada** para esta visualização, não mostrando todos os detalhes das ramificações mais profundas.
        * Os nós coloridos que não possuem mais divisões (como o nó mais à direita `Setor de atuação da empresa_Finanças ou Bancos <= 0.5`) também são nós folha para os caminhos que terminam ali na visualização.

* **Cores dos Nós:** As diferentes cores dos nós (neste caso, laranja e azul) geralmente representam a classe predominante naquele nó, ajudando a visualizar como a árvore está tentando separar as diferentes classes.

---

**Exemplo de Caminho de Decisão:**

Vamos seguir um caminho hipotético:

1.  **Nó Raiz (Topo):** A primeira decisão é baseada em `experiencia_profissional_encoded <= 1.5`.
    * **Se VERDADEIRO** (experiência profissional codificada é menor ou igual a 1.5): A amostra segue para o nó da esquerda, cuja próxima decisão é `senioridade_encoded <= 1.5`.
    * **Se FALSO** (experiência profissional codificada é maior que 1.5): A amostra segue para o nó da direita, cuja próxima decisão é `UF onde mora_MG <= 0.5` (provavelmente perguntando se a UF onde mora é Minas Gerais ou não, baseado na codificação).

2.  Suponha que `experiencia_profissional_encoded <= 1.5` foi **VERDADEIRO**. Chegamos ao nó que pergunta `senioridade_encoded <= 1.5`.
    * Se `senioridade_encoded <= 1.5` for **VERDADEIRO**: A amostra vai para o nó mais à esquerda, `Setor de atuação da empresa_Marketing <= 0.5`. A classe predominante neste nó é "Salário Baixo/Médio".
    * ... e assim por diante, até que a amostra chegue a um nó folha (ou um nó truncado `(...)` nesta visualização).


### arvore_exemplo_melhorada
![arvore_exemplo_melhorada](https://github.com/user-attachments/assets/410ea2af-736a-4cbf-9541-d0edb1ac49d1)

O gráfico apresentado é uma **visualização de uma única árvore de decisão**, extraída de um modelo mais complexo chamado **Random Forest**. Um Random Forest é um conjunto (ou "floresta") de múltiplas árvores de decisão, onde cada árvore contribui para a predição final. Esta visualização nos ajuda a entender como uma dessas árvores toma decisões para classificar os dados.

---

**Como interpretar os componentes da árvore:**

* **Nós (Retângulos):** Cada retângulo é um nó na árvore.
    * **Nós de Decisão (Nós Internos):** São os retângulos que têm ramificações (setas) saindo deles. Eles contêm uma condição baseada em uma das *features* (características) dos dados.
        * **Condição de Divisão:** A primeira linha no nó de decisão (ex: `experiencia_profissional_encoded <= 1.5`). Esta é a pergunta que a árvore faz sobre uma amostra de dados. Se a condição for verdadeira, a amostra segue para o galho da esquerda; se for falsa, para o galho da direita.
        * `gini`: O **Índice de Gini** é uma medida de impureza do nó. Um valor de Gini igual a 0 significa que o nó é perfeitamente puro (todas as amostras nesse nó pertencem à mesma classe). Quanto maior o Gini, mais misturadas estão as classes no nó.
        * `samples`: O número de amostras de treinamento que alcançaram este nó.
        * `value`: Mostra a distribuição das amostras entre as diferentes classes possíveis dentro daquele nó. Por exemplo, `value = [100,632, 267,722]` no segundo nó da esquerda (contando o nó raiz como o primeiro nível) indica como as 1801 amostras (`samples = 1801`) estão distribuídas entre as classes. A classe predominante, "Salário Baixo/Médio", é determinada por essa distribuição.
        * `class`: Indica a classe majoritária entre as amostras presentes naquele nó. Se este fosse um nó folha, essa seria a predição da árvore para as amostras que chegam até ele.
    * **Nós Folha (Nós Terminais):** São os nós no final das ramificações, onde não há mais divisões. Eles representam a predição final para qualquer amostra que percorra o caminho até eles.
        * Neste gráfico, os nós cinzas com `(...)` no final indicam que a árvore continua, mas foi **truncada ou simplificada** para esta visualização, não mostrando todos os detalhes das ramificações mais profundas.
        * Os nós coloridos que não possuem mais divisões (como o nó mais à direita na segunda linha de profundidade: `Setor de atuação da empresa_Finanças ou Bancos <= 0.5`) também são nós folha para os caminhos que terminam ali na visualização, se não tiverem mais ramificações abaixo deles.

* **Cores dos Nós:** As diferentes cores dos nós (neste caso, laranja e azul) geralmente representam a classe predominante naquele nó, ajudando a visualizar como a árvore está tentando separar as diferentes classes. Por exemplo, nós laranjas podem predominantemente representar "Salário Baixo/Médio", enquanto nós azuis podem representar "Salário Alto".

---

**Exemplo de Caminho de Decisão:**

Vamos seguir um caminho hipotético:

1.  **Nó Raiz (Topo):** A primeira decisão é baseada em `experiencia_profissional_encoded <= 1.5`.
    * **Se VERDADEIRO** (experiência profissional codificada é menor ou igual a 1.5): A amostra segue para o nó da esquerda, cuja próxima decisão é `senioridade_encoded <= 1.5`.
    * **Se FALSO** (experiência profissional codificada é maior que 1.5): A amostra segue para o nó da direita, cuja próxima decisão é `UF onde mora_MG <= 0.5`.

2.  Suponha que `experiencia_profissional_encoded <= 1.5` foi **VERDADEIRO**. Chegamos ao nó que pergunta `senioridade_encoded <= 1.5`.
    * Se `senioridade_encoded <= 1.5` for **VERDADEIRO**: A amostra vai para o nó mais à esquerda na linha seguinte, `Setor de atuação da empresa_Marketing <= 0.5`. A classe predominante neste nó é "Salário Baixo/Médio".
    * ... e assim por diante, até que a amostra chegue a um nó folha (ou um nó truncado `(...)` nesta visualização). A classe indicada no nó final alcançado seria a predição dessa árvore específica para a amostra.




## Resultados obtidos com o modelo 2 da 1º pergunta orietada a dados

### Modelo Árvore de Decisão Classificatória

| Classe          | Precisão | Recall | F1-Score | Suporte |
|-----------------|----------|--------|----------|---------|
| Acima de R$ 30.000/mês    | 0.12     | 0.10   | 0.11     | 10     |
| Até R$ 2.000/mês | 0.28     | 0.41   | 0.33     | 56     | 
| R$ 16.001/mês a R$ 30.000/mês  | 0.40     | 0.31   | 0.35     | 59     |
| R$ 2.001/mês a R$ 4.000/mês | 0.42     | 0.42   | 0.42     | 160     |
| R$ 4.001/mês a R$ 8.000/mês | 0.57     | 0.45   | 0.50     | 352     |
| R$ 8.001/mês a R$ 16.000/mês | 0.61     | 0.72   | 0.66     | 353     |
| accuracy |  |  | **0.53** | **990** |
| macro avg | **0.40** | **0.40** | **0.40** | **990** |
| weighted avg | **0.53** | **0.53** | **0.52** | **990** |

- Acurácia do Modelo: 0.53
- Acurácia do Modelo no Conjunto de Treinamento: -
- Acurácia do Modelo no Conjunto de Teste: -
- Diferença de Acurácia (Treino - Teste): -


### matriz_confusao 1_2
![matriz_confusao](https://github.com/user-attachments/assets/ac19812f-ecd2-47b0-a08b-f8b7b0db1732)

**Como interpretar a Matriz de Confusão:**

* **Eixo Vertical (Real):** Indica a classe verdadeira à qual cada instância pertence.
* **Eixo Horizontal (Predito):** Indica a classe que o modelo previu para cada instância.
* **Células da Matriz:**
    * **Diagonal Principal (do canto superior esquerdo ao canto inferior direito):** Os números nestas células representam as **classificações corretas**. Por exemplo, o valor na célula onde "Real" é "R$ 8.001/mês a R$ 16.000/mês" e "Predito" também é "R$ 8.001/mês a R$ 16.000/mês" indica quantas vezes o modelo acertou essa classe. Quanto maiores os valores na diagonal, melhor o desempenho para aquelas classes específicas.
    * **Fora da Diagonal Principal:** Os números nestas células representam **erros de classificação** (confusões).
        * Um valor em uma célula onde a classe "Real" é X e a classe "Predita" é Y (e X ≠ Y) significa que o modelo classificou erroneamente instâncias da classe X como pertencentes à classe Y.
* **Escala de Cores:** A barra de cores à direita (geralmente um gradiente) indica a magnitude dos valores nas células. Cores mais escuras (neste caso, azul mais intenso) correspondem a contagens mais altas, facilitando a identificação visual de onde ocorrem a maioria das classificações e misclassificações.

**Análise da Matriz de Confusão Específica (baseada na imagem):**

1.  **Desempenho por Classe (Diagonal):**
    * **Acima de R$ 30.000/mês:** Apenas **1** instância foi classificada corretamente.
    * **Até R$ 2.000/mês:** **23** instâncias foram classificadas corretamente.
    * **R$ 16.001/mês a R$ 30.000/mês:** **18** instâncias foram classificadas corretamente.
    * **R$ 2.001/mês a R$ 4.000/mês:** **68** instâncias foram classificadas corretamente.
    * **R$ 4.001/mês a R$ 8.000/mês:** **158** instâncias foram classificadas corretamente.
    * **R$ 8.001/mês a R$ 16.000/mês:** **254** instâncias foram classificadas corretamente. Esta é a classe com o maior número de acertos.

2.  **Principais Erros de Classificação (Fora da Diagonal):**
    * **Classe "Acima de R$ 30.000/mês" (Real):**
        * Foi frequentemente confundida com outras classes, especialmente com "R$ 8.001/mês a R$ 16.000/mês" (**7** vezes) e "R$ 16.001/mês a R$ 30.000/mês" (**2** vezes). Isso indica que o modelo tem muita dificuldade em identificar corretamente os salários mais altos.
    * **Classe "Até R$ 2.000/mês" (Real):**
        * Foi confundida principalmente com "R$ 2.001/mês a R$ 4.000/mês" (**20** vezes) e "R$ 4.001/mês a R$ 8.000/mês" (**11** vezes).
    * **Classe "R$ 16.001/mês a R$ 30.000/mês" (Real):**
        * A maior confusão foi com "R$ 8.001/mês a R$ 16.000/mês" (**34** vezes).
    * **Classe "R$ 2.001/mês a R$ 4.000/mês" (Real):**
        * Confundida com "Até R$ 2.000/mês" (**36** vezes) e "R$ 4.001/mês a R$ 8.000/mês" (**42** vezes).
    * **Classe "R$ 4.001/mês a R$ 8.000/mês" (Real):**
        * Confundida com "R$ 2.001/mês a R$ 4.000/mês" (**69** vezes) e "R$ 8.001/mês a R$ 16.000/mês" (**104** vezes).

**Observações Gerais:**

* O modelo parece ter um melhor desempenho para a classe **"R$ 8.001/mês a R$ 16.000/mês"**, que possui o maior número de classificações corretas na diagonal.
* Há uma tendência de confusão entre faixas salariais adjacentes, o que é esperado, pois a distinção entre elas pode ser sutil.
* A classe **"Acima de R$ 30.000/mês"** é a que apresenta o pior desempenho em termos de acertos, sendo frequentemente subestimada pelo modelo. Isso pode ser devido a um menor número de amostras nessa classe nos dados de treinamento (desbalanceamento de classes) ou à dificuldade intrínseca de separar essa faixa das demais com as features disponíveis.


### distribuicao_faixas_salariais_originais 1_2
![distribuicao_faixas_salariais_originais](https://github.com/user-attachments/assets/9f135a05-dc93-4d26-8b6c-45c32f05a136)

O gráfico apresentado é um **gráfico de barras horizontais** intitulado "Distribuição de Faixas Salariais Originais". Ele mostra a frequência (ou contagem) de cada faixa salarial presente nos dados originais, antes de qualquer agrupamento ou processamento dessas faixas.

**Como interpretar o gráfico:**

* **Eixo Vertical (Faixa Salarial):** Lista as diferentes categorias de faixas salariais mensais que foram reportadas ou coletadas. Cada barra horizontal corresponde a uma dessas faixas.
* **Eixo Horizontal (Contagem):** Indica o número de vezes que cada faixa salarial aparece no conjunto de dados. O comprimento da barra é diretamente proporcional a essa contagem.
* **Barras:** Cada barra representa uma faixa salarial específica. Quanto mais longa a barra, maior o número de indivíduos ou registros que se enquadram naquela faixa salarial.

**Análise da Distribuição Apresentada:**

Observando o gráfico, podemos extrair as seguintes informações sobre a distribuição das faixas salariais originais:

* **Faixas Mais Comuns:**
    * A faixa salarial **"de R$8.001/mês a R$ 12.000/mês"** é a mais frequente, com uma contagem significativamente maior que as outras (aproximadamente 790 ocorrências).
    * Seguida por **"de R$4.001/mês a R$ 6.000/mês"** (aproximadamente 630-640 ocorrências).
    * E depois **"de R$6.001/mês a R$ 8.000/mês"** (aproximadamente 540 ocorrências).

* **Faixas Menos Comuns:**
    * Várias faixas salariais têm contagens muito baixas, indicando que são raras no conjunto de dados. Estas incluem, por exemplo:
        * "de R$101/mês a R$ 2.000/mês" (contagem muito próxima de zero, quase imperceptível).
        * "Acima de R$ 40.001/mês".
        * "Menos de R$ 1.000/mês".
        * "de R$30.001/mês a R$ 40.000/mês".
        * "de R$25.001/mês a R$ 30.000/mês".

* **Desbalanceamento:** O gráfico demonstra claramente um desbalanceamento entre as diferentes faixas salariais. Algumas poucas faixas concentram a maioria dos registros, enquanto muitas outras são representadas por um número pequeno de instâncias. Este desbalanceamento é uma característica importante dos dados e frequentemente leva à necessidade de agrupar faixas salariais (como visto no código do notebook) para criar classes mais equilibradas e significativas para modelos de machine learning.


### distribuicao_faixas_salariais_agrupadas 1_2
![distribuicao_faixas_salariais_agrupadas](https://github.com/user-attachments/assets/0844c00b-371f-49c3-82d2-505ec0830728)

O gráfico apresentado é um **gráfico de barras horizontais** intitulado "Distribuição de Faixas Salariais Agrupadas". Ele ilustra a frequência (ou contagem) de cada faixa salarial **após** estas terem sido agrupadas em categorias mais amplas. Este agrupamento é uma etapa comum de pré-processamento de dados, realizada para simplificar o problema de classificação, reduzir o número de classes e, potencialmente, lidar com classes minoritárias no conjunto de dados original.

**Como interpretar o gráfico:**

* **Eixo Vertical (Faixa Salarial):** Lista as novas categorias de faixas salariais agrupadas. Cada barra horizontal corresponde a uma dessas faixas consolidadas.
* **Eixo Horizontal (Contagem):** Indica o número de vezes que cada faixa salarial agrupada aparece no conjunto de dados. O comprimento da barra é diretamente proporcional a essa contagem.
* **Barras:** Cada barra representa uma faixa salarial agrupada específica. Quanto mais longa a barra, maior o número de indivíduos ou registros que se enquadram naquela faixa salarial consolidada.

**Análise da Distribuição Apresentada:**

Observando o gráfico, podemos notar o seguinte sobre a distribuição das faixas salariais após o agrupamento:

* **Faixas Mais Comuns (Agrupadas):**
    * A faixa **"R$8.001/mês a R$ 16.000/mês"** é a mais frequente entre as agrupadas (com uma contagem de aproximadamente 1180).
    * Seguida de perto pela faixa **"R$4.001/mês a R$ 8.000/mês"** (com uma contagem de aproximadamente 1170).
    * A faixa **"R$2.001/mês a R$ 4.000/mês"** aparece em seguida, com uma contagem consideravelmente menor (aproximadamente 530).

* **Faixas Menos Comuns (Agrupadas):**
    * A faixa **"Acima de R$ 30.000/mês"** é a menos frequente, com uma contagem muito baixa em comparação com as outras (menos de 50).
    * As faixas **"Até R$ 2.000/mês"** e **"R$16.001/mês a R$ 30.000/mês"** possuem contagens intermediárias, mas ainda significativamente menores que as duas faixas mais populosas (ambas em torno de 180-200).

* **Impacto do Agrupamento:**
    * Comparando com uma distribuição de faixas salariais originais (que tipicamente teria mais categorias e maior granularidade), este gráfico mostra um número reduzido de classes.
    * Embora o agrupamento possa ter tornado algumas classes mais balanceadas (especialmente as duas primeiras), ainda existe um desbalanceamento notável, com a categoria de salário mais alto ("Acima de R$ 30.000/mês") sendo uma classe minoritária clara. Este desbalanceamento é uma consideração importante para o treinamento do modelo de machine learning.


### correlacao_variaveis_faixa_salarial 1_2
![correlacao_variaveis_faixa_salarial](https://github.com/user-attachments/assets/18aea812-9bdf-42a8-ae94-46dd2d18a141)

O gráfico apresentado é um **gráfico de barras verticais** intitulado "Correlação (Cramer's V) com Faixa Salarial Agrupada". Ele exibe a força da associação entre diversas variáveis categóricas (features) e a variável alvo, que é a "Faixa Salarial Agrupada". A medida de associação utilizada é o **Coeficiente V de Cramer**.

**Como interpretar o gráfico:**

* **Eixo Vertical (Coeficiente de Cramer's V):** Este eixo mostra o valor do Coeficiente V de Cramer, que varia de 0 a 1.
    * Um valor próximo de **0** indica uma associação fraca ou inexistente entre a feature e a faixa salarial agrupada.
    * Um valor próximo de **1** indica uma associação forte entre a feature e a faixa salarial agrupada.
* **Eixo Horizontal (Features):** Este eixo lista as diferentes variáveis categóricas que foram analisadas em relação à faixa salarial agrupada. As legendas estão rotacionadas para facilitar a leitura.
* **Barras:** Cada barra representa uma feature. A altura da barra é proporcional ao valor do Coeficiente V de Cramer para aquela feature, indicando visualmente a força de sua associação com a faixa salarial agrupada. As barras estão ordenadas da maior para a menor associação.

**Análise das Associações Apresentadas (da mais forte para a mais fraca):**

1.  **Nível de senioridade:** Apresenta a associação **mais forte** com a faixa salarial agrupada, com um Coeficiente V de Cramer de aproximadamente **0.55**. Isso sugere que o nível de senioridade do profissional é o indicador mais forte da sua faixa salarial entre as features analisadas.
2.  **Tempo de experiência na área de dados:** Possui a segunda associação mais forte, com um coeficiente em torno de **0.30**.
3.  **Nível de ensino alcançado:** Mostra uma associação moderada, com um coeficiente de aproximadamente **0.23**.
4.  **Cargo atual:** Apresenta uma associação de cerca de **0.19**.
5.  **Setor de atuação da empresa:** A associação é mais fraca, com um coeficiente em torno de **0.09**.
6.  **UF onde mora:** Mostra uma associação semelhante à anterior, com um coeficiente de aproximadamente **0.08**.
7.  **Área de formação acadêmica:** Apresenta uma associação de cerca de **0.07**.
8.  **Gênero do profissional:** A associação é bastante fraca, com um coeficiente em torno de **0.04**.
9.  **Cor/Raça/Etnia:** Apresenta a associação **mais fraca** entre as features listadas, com um coeficiente também em torno de **0.04**.

**Importância da Análise:**

Este tipo de análise é útil por várias razões:

* **Entendimento dos Dados:** Ajuda a entender quais características dos profissionais estão mais relacionadas com suas faixas salariais.
* **Seleção de Features:** Features com associações muito baixas com a variável alvo podem, em alguns casos, ser consideradas menos importantes para um modelo preditivo e, potencialmente, descartadas para simplificar o modelo ou reduzir o ruído. No entanto, mesmo features com baixa correlação individual podem ser úteis em combinação com outras.
* **Direcionamento de Análises Futuras:** Pode indicar quais aspectos merecem uma investigação mais aprofundada.

----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

# _Interpretação dos modelos_

*   [Interpretação dos modelo 1º pergunta orientada a dados](#interpretação-dos-modelo-1º-pergunta-orientada-a-dados)
	*   [Interpretação do modelo 1_1](#interpretação-do-modelo-1_1)
	*    [Interpretação do modelo 2_1](#interpretação-do-modelo-2_1)

## Interpretação dos modelo 1º pergunta orientada a dados

## Interpretação do modelo 1_1

### I. Especificação do Modelo e Parâmetros Chave

#### a. Tipo de Modelo de Machine Learning
O modelo de machine learning implementado no código Python é um **`RandomForestClassifier`**. Este é um modelo de ensemble que utiliza múltiplas árvores de decisão para realizar classificações, combinando as previsões de cada árvore para obter um resultado final mais robusto e preciso.

#### b. Principais Hiperparâmetros do Modelo Final Treinado
O modelo final (`best_rf_model` no código) foi obtido após um processo de otimização de hiperparâmetros utilizando `GridSearchCV`. Os principais hiperparâmetros do `best_rf_model` são:

1.  **`n_estimators`: 100**
    * **Relevância**: Define o número de árvores de decisão que compõem a floresta. Um número maior de árvores geralmente leva a um desempenho melhor e mais estável, mas também aumenta o custo computacional. 100 é um valor comum e razoável.

2.  **`max_depth`: `None`**
    * **Relevância**: Controla a profundidade máxima de cada árvore individual. Se `None`, os nós são expandidos até que todas as folhas sejam puras ou até que todas as folhas contenham menos amostras do que `min_samples_split`. Neste modelo, a profundidade é efetivamente limitada por `min_samples_leaf` e `min_samples_split`.

3.  **`min_samples_split`: 15**
    * **Relevância**: Especifica o número mínimo de amostras que um nó deve ter para poder ser dividido. Ajuda a controlar a complexidade da árvore e previne o overfitting, evitando que a árvore crie divisões baseadas em poucas amostras.

4.  **`min_samples_leaf`: 7**
    * **Relevância**: Define o número mínimo de amostras que devem estar presentes em um nó folha (um nó terminal). Assim como `min_samples_split`, este parâmetro ajuda a suavizar o modelo e a evitar o overfitting, garantindo que cada decisão final seja baseada em um número suficiente de exemplos.

5.  **`class_weight`: `'balanced_subsample'`**
    * **Relevância**: Este parâmetro é crucial para lidar com classes desbalanceadas. `'balanced_subsample'` ajusta os pesos das classes de forma inversamente proporcional às suas frequências, mas os pesos são calculados para cada subamostra de bootstrap usada para treinar cada árvore. Isso ajuda o modelo a dar mais importância à classe minoritária durante o treinamento.

6.  **`random_state`: 42**
    * **Relevância**: Garante a reprodutibilidade dos resultados. Ao fixar o `random_state`, a aleatoriedade envolvida na construção do Random Forest (como a seleção de amostras para bootstrap e a seleção de features em cada divisão) será a mesma em diferentes execuções.

7.  **`n_jobs`: -1**
    * **Relevância**: Utiliza todos os processadores disponíveis para paralelizar o treinamento das árvores, o que pode acelerar significativamente o processo de treinamento.

Estes parâmetros foram selecionados pelo `GridSearchCV` como a melhor combinação para maximizar a métrica `balanced_accuracy`, indicando um foco em obter um bom desempenho em ambas as classes da variável alvo (salário alto vs. salário baixo/médio).

---

### II. Fatores Preditivos Dominantes: Uma Análise de 'Feature Importances'

#### a. Importância Global das Features
O modelo `RandomForestClassifier` calcula a importância de cada feature com base em quão bem ela contribui para a pureza dos nós nas árvores de decisão (geralmente usando a redução média da impureza de Gini). As features mais importantes identificadas pelo modelo (`best_rf_model.feature_importances_`), ordenadas da mais para a menos importante, são:

1.  **`senioridade_encoded`**: Importância relativa de aproximadamente **0.4053**
2.  **`experiencia_profissional_encoded`**: Importância relativa de aproximadamente **0.3588**
3.  **`formacao_academica_encoded`**: Importância relativa de aproximadamente **0.0952**
4.  **`UF onde mora_SP`**: Importância relativa de aproximadamente **0.0125**
5.  **`Área de formação acadêmica_Economia/ Administração / Contabilidade / Finanças/ Negócios`**: Importância relativa de aproximadamente **0.0110**
6.  **`Área de formação acadêmica_Computação / Engenharia de Software / Sistemas de Informação/ TI`**: Importância relativa de aproximadamente **0.0087**
7.  **`Setor de atuação da empresa_Tecnologia/Fábrica de Software`**: Importância relativa de aproximadamente **0.0083**
8.  **`UF onde mora_RJ`**: Importância relativa de aproximadamente **0.0077**
9.  **`Setor de atuação da empresa_Finanças ou Bancos`**: Importância relativa de aproximadamente **0.0076**
10. **`Área de formação acadêmica_Outras Engenharias`**: Importância relativa de aproximadamente **0.0068**

*(As demais features apresentam importâncias progressivamente menores.)*

#### b. Classificação de 'Formação Acadêmica' e 'Experiência Profissional'
Conforme a lista acima:
* **`experiencia_profissional_encoded`** é a **segunda feature mais importante** (0.3588).
* **`formacao_academica_encoded`** (que representa o nível de ensino alcançado) é a **terceira feature mais importante** (0.0952).
* Além do nível de formação, as **áreas específicas de formação acadêmica** (como `Área de formação acadêmica_Economia/ Administração...` e `Área de formação acadêmica_Computação...`) também aparecem entre as 10 mais importantes, embora com pesos individuais menores que o nível de formação geral.

#### c. Interpretação das Importâncias no Contexto da Disparidade Salarial
As importâncias das features revelam que, para este modelo, os fatores mais determinantes para prever se um profissional de dados terá um salário "alto" ou "baixo/médio" são, nesta ordem:

1.  **Nível de Senioridade (`senioridade_encoded`)**: Este é o fator de maior impacto. O modelo aprendeu que o nível hierárquico do profissional (Júnior, Pleno, Sênior) é o principal diferenciador salarial. Isso está alinhado com a expectativa de mercado, onde a senioridade reflete uma combinação de experiência, responsabilidade e impacto.
2.  **Tempo de Experiência na Área de Dados (`experiencia_profissional_encoded`)**: O segundo fator mais crucial. O número de anos de experiência prática na área de dados influencia fortemente a faixa salarial. O `report.md` já indicava, na seção "Descrição de dados", que a correlação entre Experiência Total e Salário era de 0.54, sugerindo uma relação positiva.
3.  **Nível de Ensino Alcançado (`formacao_academica_encoded`)**: Embora menos influente que senioridade e experiência, a formação acadêmica ainda é o terceiro fator mais importante. Isso sugere que possuir níveis mais altos de educação formal (como Mestrado ou Doutorado) contribui para alcançar salários mais elevados, conforme também indicado na análise exploratória do `report.md` (onde Doutorado tinha a maior mediana salarial).

As demais features, como a localização (especialmente morar em SP ou RJ) e o setor/área de formação específicos, adicionam nuances à previsão, mas têm um peso significativamente menor. Isso indica que, embora esses fatores possam influenciar, o modelo considera senioridade, experiência e nível de formação como os pilares principais da disparidade salarial.

---

### III. Desvendando a Lógica do Modelo: 'Regras de Raciocínio' e Caminhos de Decisão

Sendo um `RandomForestClassifier`, a lógica do modelo é uma agregação das decisões de 100 árvores de decisão. Para elucidar as 'regras de raciocínio', podemos visualizar uma árvore individual do ensemble. O código fornecido gera visualizações de uma árvore (`arvore_exemplo_melhorada.png` e `arvore_exemplo_simplificada.png`). Analisando a `arvore_exemplo_simplificada.png` (com `max_depth=3`):

#### a. Exemplo de Caminhos de Decisão (Decision Paths)
(Baseado na estrutura típica de `plot_tree` e nas features mais importantes)

* **Nó Raiz (Decisão Inicial):** Geralmente a feature mais importante globalmente, ou uma muito importante, como `experiencia_profissional_encoded`.
    * Exemplo: `experiencia_profissional_encoded <= 1.5` (corresponde a menos de 1 a 2 anos de experiência).

* **Caminho 1 (Baixa Experiência):** Se `experiencia_profissional_encoded <= 1.5` é **Verdadeiro**:
    * Próxima Decisão: `senioridade_encoded <= 1.5` (corresponde a Júnior ou Pleno).
        * Se **Verdadeiro** (Júnior/Pleno com pouca experiência):
            * Última Decisão (neste nível de profundidade): `formacao_academica_encoded <= 0.5` (Estudante de Graduação ou Graduação).
                * Se **Verdadeiro**: Leva a um nó folha com alta probabilidade de "Salário Baixo/Médio".
                * Se **Falso** (Pós-graduação ou superior, mas Júnior/Pleno com pouca experiência): Ainda pode levar a "Salário Baixo/Médio", mas talvez com uma probabilidade ligeiramente menor ou com mais amostras da classe "Salário Alto" em comparação ao nó anterior.
        * Se **Falso** (Sênior, mas com pouca experiência - caso menos comum): A árvore faria outra divisão, talvez por `UF onde mora_SP`. Se não for SP, pode ainda levar a "Salário Baixo/Médio", mas se for SP, poderia pender para "Salário Alto" dependendo das amostras.

* **Caminho 2 (Alta Experiência):** Se `experiencia_profissional_encoded <= 1.5` é **Falso** (mais de 1-2 anos de experiência):
    * Próxima Decisão: `senioridade_encoded <= 1.5` (Júnior ou Pleno).
        * Se **Verdadeiro** (Júnior/Pleno com mais experiência):
            * Última Decisão: `formacao_academica_encoded <= 2.5` (Até Pós-graduação).
                * Se **Verdadeiro**: Pode levar a "Salário Alto", mas com menor probabilidade do que um Sênior.
                * Se **Falso** (Mestrado/Doutorado, Pleno com mais experiência): Maior probabilidade de "Salário Alto".
        * Se **Falso** (Sênior com mais experiência):
            * Última Decisão: `UF onde mora_SP <= 0.5`.
                * Se **Falso** (Mora em SP, Sênior com mais experiência): Alta probabilidade de "Salário Alto".
                * Se **Verdadeiro** (Não mora em SP, Sênior com mais experiência): Provavelmente "Salário Alto", mas com menor proporção de amostras dessa classe do que se morasse em SP.

#### b. Como as 'Regras' Ajudam a Entender as Decisões
Esses caminhos ilustram que o modelo não avalia as features isoladamente. Ele aprende combinações de condições. Por exemplo:
* **Pouca experiência + Baixa senioridade + Baixa formação** => Quase certamente Salário Baixo/Médio.
* **Muita experiência + Alta senioridade + Localização em SP** => Alta chance de Salário Alto.
* Casos intermediários são resolvidos por divisões subsequentes que consideram outras features (como setor de atuação, área de formação específica, etc., visíveis na árvore mais profunda).

A árvore mostra que o impacto da `formacao_academica_encoded` é frequentemente avaliado *após* a experiência e a senioridade já terem sido consideradas, o que está alinhado com suas importâncias relativas.

---

### IV. A Interação entre Formação Acadêmica e Experiência Profissional na Disparidade Salarial: Insights Orientados pelo Modelo

#### a. Evidências de Efeitos de Interação
A pergunta central é sobre a **interação** entre formação e experiência. O modelo Random Forest é inerentemente bom em capturar interações, pois os caminhos de decisão são sequências de condições.

1.  **Importância das Features:** O fato de `experiencia_profissional_encoded` (0.3588) e `formacao_academica_encoded` (0.0952) serem ambas importantes sugere que ambas contribuem, mas a experiência tem um peso maior. No entanto, a importância individual não revela totalmente a interação.

2.  **Caminhos de Decisão (Seção III):** As árvores consistentemente usam tanto experiência quanto formação para segmentar os dados. A ordem em que aparecem e as condições subsequentes indicam uma interação. Por exemplo, o "valor" de uma alta formação pode ser diferente dependendo se o profissional já tem muita ou pouca experiência.

3.  **Gráfico de Interação Específico (`interacao_formacao_experiencia.png`):** O código Python gera um heatmap da "Probabilidade de Salário Alto por Formação Acadêmica e Experiência Profissional". Este gráfico é a evidência mais direta da interação:
    * **Pouca Experiência ("Menos de 1 ano"):** A probabilidade de salário alto é baixa para todos os níveis de formação (0.01 para Estudante, 0.02 para Graduação, até 0.04 para Mestrado). Aqui, a formação não consegue compensar a falta de experiência.
    * **Muita Experiência ("de 7 a 10 anos"):** A probabilidade de salário alto é significativamente maior e varia mais acentuadamente com a formação. Um Estudante de Graduação com 7-10 anos de experiência tem 0.67 de probabilidade, enquanto um Doutorado com a mesma experiência tem 0.94.
    * **Impacto Diferencial da Formação:**
        * Com "de 1 a 2 anos" de experiência, passar de "Graduação" (0.20) para "Doutorado" (0.53) aumenta a probabilidade em 0.33.
        * Com "de 7 a 10 anos" de experiência, passar de "Graduação" (0.74) para "Doutorado" (0.94) aumenta a probabilidade em 0.20. Embora o aumento absoluto seja menor, o ponto de partida já é mais alto. O gráfico mostra que para atingir as probabilidades mais altas (>0.90), é necessária uma combinação de alta formação (Mestrado/Doutorado) E alta experiência (7-10 anos).
    * **Limiares de Experiência:**
        * Com **Mestrado ou Doutorado**, a probabilidade de salário alto ultrapassa 0.50 (torna-se mais provável ter salário alto) já com "de 1 a 2 anos" de experiência.
        * Com **Graduação/Bacharelado**, isso só ocorre com "de 3 a 4 anos" de experiência.
        * Com **Pós-graduação (lato sensu)**, também a partir de "de 3 a 4 anos", mas com probabilidades ligeiramente maiores que apenas Graduação.

#### b. Como o Modelo Sugere a Interação
O modelo não apenas considera os efeitos principais da formação e da experiência, mas o `heatmap de interação` (derivado das previsões do modelo em combinações dessas features) e os caminhos de decisão das árvores internas mostram que o efeito de uma variável no salário depende do nível da outra.
* **Formação se torna mais crítica com mais experiência para atingir os salários mais altos:** Ter muitos anos de experiência com apenas graduação leva a uma boa chance de salário alto (ex: 0.74), mas para se aproximar de 100% de chance, um Mestrado ou Doutorado parece ser necessário.
* **Experiência pode compensar (até certo ponto) menor formação:** Um "Estudante de Graduação" com 7-10 anos de experiência (0.67 de probabilidade) tem uma chance maior de salário alto do que um "Doutorado" com menos de 1 ano de experiência (0.03).

---

### V. Síntese: Conectando a Interpretação do Modelo à Pergunta Central da Pesquisa

#### a. Resumo das Principais Descobertas
O modelo `RandomForestClassifier` identificou que o **nível de senioridade**, o **tempo de experiência profissional** e o **nível de formação acadêmica** são os três fatores mais importantes para prever se um profissional de dados no Brasil terá um salário acima ou abaixo de R$ 8.000/mês. A lógica do modelo, visualizada através de árvores de decisão e um heatmap de interação, demonstra que esses fatores não atuam isoladamente.

#### b. Relação com a Pergunta Orientadora
A pergunta central é: "Como fatores como formação acadêmica e experiência profissional interagem para influenciar a disparidade salarial entre profissionais de dados no Brasil?"

A interpretação do modelo fornece as seguintes respostas:

1.  **Ambos são Cruciais, mas a Experiência (e a Senioridade que dela deriva) Pesa Mais Inicialmente:** A experiência profissional (e a senioridade, que está altamente correlacionada com ela) tem um impacto mais forte e imediato na diferenciação salarial do que o nível de formação isoladamente.
2.  **A Formação Acadêmica Potencializa o Retorno da Experiência:** O modelo sugere que, embora a experiência seja vital, níveis mais altos de formação acadêmica (especialmente Mestrado e Doutorado) permitem que os profissionais capitalizem melhor sobre sua experiência acumulada para alcançar os patamares salariais mais elevados. A diferença salarial entre níveis de formação se torna mais evidente para profissionais mais experientes.
3.  **Interação Não Linear e Contextual:** Não há uma regra simples como "X anos de experiência + Y nível de formação = Z salário". O `heatmap de interação` mostra que o impacto de um ano adicional de experiência é diferente para um graduado versus um doutor, e o "valor" de um diploma avançado se manifesta de forma mais acentuada quando combinado com experiência substancial. Profissionais com alta formação mas pouca experiência não necessariamente comandam salários altos imediatamente, enquanto experiência considerável pode, até certo ponto, compensar uma formação menos avançada.

#### c. Limitações da Interpretação e do Modelo
1.  **Variáveis Codificadas:** A interpretação de `_encoded` features requer sempre a referência aos mapeamentos originais. A "distância" entre os valores codificados (ex: 0, 1, 2) pode não refletir linearmente o impacto real.
2.  **Causalidade vs. Correlação:** O modelo identifica correlações e padrões preditivos, mas não estabelece causalidade. Por exemplo, ter um Doutorado e alta experiência leva a um salário alto, ou profissionais que já estão em posições de alto salário são mais propensos a buscar Doutorado?
3.  **Outras Variáveis Não Incluídas ou Menos Importantes no Modelo:** Habilidades técnicas específicas (linguagens de programação, ferramentas), tipo de contrato (CLT, PJ), tamanho da empresa, e outros fatores mencionados no `report.md` como influenciadores da disparidade salarial, tiveram menos peso neste modelo específico ou não foram detalhadamente explorados nas features. A granularidade dessas features pode ser importante.
4.  **Simplificação da Variável Alvo:** A binarização do salário ("Alto" vs. "Baixo/Médio") simplifica o problema, mas perde nuances das faixas salariais intermediárias e extremas.
5.  **Interpretabilidade do Ensemble:** Embora uma árvore possa ser visualizada, a lógica completa do Random Forest (100 árvores) é mais complexa. A importância das features e o heatmap de interação fornecem boas aproximações, mas não capturam todas as sutilezas. Técnicas como SHAP poderiam oferecer insights mais granulares por instância.
6.  **Representatividade dos Dados:** A qualidade e representatividade do dataset original (`dados_limpos.csv`) são cruciais. Se houver vieses nos dados, o modelo os aprenderá.
-------------------------------------------------------------------------------------------------------------------------


## Interpretação do modelo 2_1

### I. Especificação do Modelo e Parâmetros Chave

a.  **Tipo de Modelo de Machine Learning:**
    O modelo implementado no código é um **`GradientBoostingClassifier`** da biblioteca `sklearn.ensemble`. Este é um modelo de ensemble que constrói árvores de decisão de forma sequencial, onde cada nova árvore tenta corrigir os erros cometidos pelas árvores anteriores.

b.  **Principais Hiperparâmetros do Modelo Final Treinado e Relevância:**
    O modelo final foi otimizado usando `RandomizedSearchCV`. Com base na saída do notebook, os melhores hiperparâmetros encontrados foram:
    * **`subsample`: 0.8**
        * *Relevância*: Esta é a fração de amostras a ser usada para ajustar cada árvore individual. Um valor menor que 1.0 introduz estocasticidade, o que pode ajudar a reduzir a variância e prevenir o overfitting. 80% das amostras são usadas para cada árvore.
    * **`n_estimators`: 100**
        * *Relevância*: O número de árvores (estágios de boosting) a serem construídas. Um número maior de árvores geralmente leva a um melhor desempenho, até um certo ponto, mas também aumenta o tempo de treinamento.
    * **`min_samples_split`: 2**
        * *Relevância*: O número mínimo de amostras necessárias para dividir um nó interno de uma árvore. Um valor pequeno como 2 permite que as árvores cresçam bastante, capturando detalhes finos, mas pode levar a overfitting se não controlado por outros parâmetros como `max_depth` ou `min_samples_leaf`.
    * **`min_samples_leaf`: 2**
        * *Relevância*: O número mínimo de amostras que um nó folha (terminal) deve ter. Este parâmetro ajuda a suavizar o modelo e reduzir o overfitting, garantindo que cada decisão final seja baseada em pelo menos 2 amostras.
    * **`max_depth`: 6**
        * *Relevância*: A profundidade máxima de cada árvore de decisão individual. Limitar a profundidade ajuda a controlar a complexidade do modelo e a prevenir o overfitting, pois árvores muito profundas podem memorizar o ruído nos dados de treinamento.
    * **`learning_rate`: 0.2**
        * *Relevância*: Também conhecido como "encolhimento" (shrinkage), este parâmetro reduz a contribuição de cada árvore. Taxas de aprendizado menores geralmente requerem um `n_estimators` maior, mas podem levar a uma melhor generalização. Um valor de 0.2 é relativamente alto, sugerindo uma convergência mais rápida.
    * **`random_state`: 42** (usado na instanciação inicial e no `RandomizedSearchCV`)
        * *Relevância*: Garante a reprodutibilidade dos resultados. O modelo se comportará da mesma maneira em execuções subsequentes.

### II. Fatores Preditivos Dominantes: Uma Análise de 'Feature Importances'

a.  **Feature Importances Globais do Modelo:**
    O notebook `modelo-1-2-arvore-classificatoria-v5.ipynb` **não calcula explicitamente nem exibe as `feature_importances_` do modelo `GradientBoostingClassifier` treinado (`best_gb`)**. A análise de importância de features no notebook é realizada *antes* da modelagem, utilizando o **Coeficiente V de Cramer** para medir a associação entre as variáveis categóricas e a faixa salarial agrupada.
    Embora o V de Cramer meça a força da associação bivariada e não a importância que o modelo GBT aprendeu, ele pode nos dar uma indicação dos atributos que provavelmente serão influentes.

    Com base na análise de V de Cramer realizada no notebook, as features mais associadas à "Faixa salarial agrupada" (em ordem decrescente de importância) foram:
    1.  **Nível de senioridade**: 0.5506
    2.  **Tempo de experiência na área de dados**: 0.2984
    3.  **Nível de ensino alcançado**: 0.2277
    4.  **Cargo atual**: 0.1862
    5.  **Setor de atuação da empresa**: 0.0938
    6.  **UF onde mora**: 0.0787
    7.  **Área de formação acadêmica**: 0.0698
    8.  **Gênero do profissional**: 0.0437
    9.  **Cor/Raça/Etnia**: 0.0428

b.  **Classificação de 'Formação Acadêmica' e 'Experiência Profissional':**
    * **Experiência Profissional**: Representada diretamente por "Tempo de experiência na área de dados" (importância V de Cramer: 0.2984, 2º lugar) e fortemente correlacionada com "Nível de senioridade" (importância V de Cramer: 0.5506, 1º lugar). Claramente, a experiência profissional é um dos fatores mais dominantes.
    * **Formação Acadêmica**: Representada por "Nível de ensino alcançado" (importância V de Cramer: 0.2277, 3º lugar) e "Área de formação acadêmica" (importância V de Cramer: 0.0698, 7º lugar). O nível de ensino alcançado tem uma associação moderada, enquanto a área específica de formação tem uma associação mais fraca com a faixa salarial agrupada, segundo o V de Cramer.

c.  **Interpretação no Contexto da Disparidade Salarial:**
    A análise de V de Cramer sugere que a **experiência** (manifestada como tempo na área e senioridade) é o principal fator associado à variação salarial. Isso está alinhado com a expectativa de que profissionais mais experientes e em níveis hierárquicos mais altos tendem a receber salários maiores. O **nível de escolaridade** também é um fator relevante, indicando que maior qualificação formal está associada a melhores salários. A área de formação específica parece ter um papel menos preponderante. O `report.md` corrobora isso ao mencionar que "profissionais que possuem certificações específicas em grandes empresas costumam receber remunerações mais altas" e que a "experiência, formação acadêmica, setor de atuação e habilidades técnicas" influenciam as diferenças salariais. O modelo GBT, se treinado com essas features, provavelmente aprenderia a dar pesos significativos a elas.

### III. Desvendando a Lógica do Modelo: 'Regras de Raciocínio' e Caminhos de Decisão

a.  **Elucidando a Lógica do `GradientBoostingClassifier`:**
    Um `GradientBoostingClassifier` constrói um ensemble de árvores de decisão. Cada árvore é treinada para corrigir os erros residuais das árvores anteriores. A previsão final é uma combinação ponderada das previsões de todas as árvores.
    * **Extração de Regras Explícitas:** Extrair regras if-then simples de um modelo GBT com muitas árvores (100 neste caso, com `max_depth=6`) é complexo. Não há uma única "árvore" que represente o modelo.
    * **Caminhos de Decisão:** Cada árvore individual possui caminhos de decisão. Por exemplo, uma árvore poderia ter um caminho como:
        * `IF Nível de senioridade_encoded <= 1.5 (Júnior ou Pleno) AND Tempo de experiência_encoded <= 2.5 (até ~4 anos) THEN predict_class_A`
        * `ELSE IF Nível de senioridade_encoded > 1.5 (Sênior) AND Nível de ensino_encoded >= 3 (Mestrado ou Doutorado) THEN predict_class_B`
        O GBT agrega muitos desses caminhos de forma ponderada.
    * **Interpretabilidade via SHAP/LIME:** O notebook fornecido não implementa técnicas como SHAP ou LIME. Essas ferramentas seriam ideais para entender as contribuições de cada feature para previsões específicas (LIME) ou para o comportamento geral do modelo (SHAP). Sem elas, a interpretação da lógica detalhada do GBT é limitada.
    * **Compreensão Baseada na Importância (V de Cramer como Proxy):** Podemos inferir que o modelo provavelmente usa "Nível de senioridade" e "Tempo de experiência" para fazer as primeiras e mais impactantes divisões nos dados, pois estas foram as features com maior associação com o alvo. Subsequentemente, "Nível de ensino" e "Cargo atual" seriam usados para refinar essas divisões.

b.  **Como as 'Regras' Ajudam a Entender as Decisões:**
    Se tivéssemos as regras ou os valores SHAP, poderíamos ver explicitamente como o modelo pondera a formação acadêmica versus a experiência. Por exemplo:
    * Um profissional com "Doutorado" (alta formação) mas "Menos de 1 ano" de experiência (baixa experiência) poderia ser classificado em uma faixa salarial mais baixa do que um profissional com "Graduação" mas "7-10 anos" de experiência.
    * O modelo aprenderia limiares para cada feature (e suas interações) que melhor separam as faixas salariais. Por exemplo, a partir de `X` anos de experiência, o impacto de ter um mestrado no salário pode aumentar significativamente.

### IV. A Interação entre Formação Acadêmica e Experiência Profissional na Disparidade Salarial: Insights Orientados pelo Modelo

a.  **Evidências de Efeitos de Interação:**
    * **Implícito no GBT:** Modelos baseados em árvores como o Gradient Boosting são inerentemente capazes de capturar efeitos de interação entre features. Uma divisão em uma feature (ex: experiência) cria subgrupos, e dentro desses subgrupos, o efeito de outra feature (ex: formação) pode ser diferente. O modelo GBT, ao construir árvores sequencialmente, pode aprender interações complexas.
    * **Ausência de Termos Explícitos:** O código não cria explicitamente features de interação (ex: `experiencia * formacao`). No entanto, o `OneHotEncoder` transforma features categóricas em múltiplas colunas binárias, e o GBT pode então aprender interações entre essas colunas binárias e outras features.
    * **Análise do `report.md`:** O `report.md` na seção "Analises exploratorias de dados" -> "1º Pergunta orientada a dados" -> "Analise exploratoria de dados bases integradas" menciona gráficos como "Salário Médio Estimado vs. Anos de Experiência por Nível de Ensino" e "Relação 3D entre Salário, Experiência e Nível de Ensino". Essas visualizações exploratórias já sugerem uma interação:
        * "As linhas [de salário médio] tendem a se divergir mais à medida que os anos de experiência aumentam. Isso significa que a diferença salarial entre os níveis de ensino se torna mais pronunciada para profissionais mais experientes." (Interpretação do gráfico de linhas no `report.md`).
        * "Para alcançar os salários mais altos, geralmente é necessária uma combinação de alto nível de ensino *e* experiência substancial." (Interpretação do gráfico 3D no `report.md`).
    * **O Modelo GBT provavelmente aprendeu essas interações observadas na EDA.** Por exemplo, o modelo pode ter aprendido que o "retorno" de um doutorado é maior para alguém com 5 anos de experiência do que para alguém com 1 ano.

b.  **Limiares e Criticidade:**
    * O modelo GBT aprende os limiares ótimos para cada divisão nas árvores. Ele poderia, por exemplo, identificar que abaixo de 2 anos de experiência, o nível de formação tem um impacto menor no salário, mas acima de 5 anos de experiência, ter um mestrado ou doutorado se torna um diferenciador mais crítico para alcançar faixas salariais mais altas.
    * Da mesma forma, para cargos de alta senioridade, um nível de formação avançado pode ser um requisito ou um fator que impulsiona significativamente o salário, enquanto para cargos juniores, a experiência prática inicial pode ser mais valorizada que a diferença entre uma graduação e uma pós-graduação.

### V. Síntese: Conectando a Interpretação do Modelo à Pergunta Central da Pesquisa

a.  **Principais Descobertas da Interpretação do Modelo (com base no GBT e proxy de V de Cramer):**
    1.  O modelo `GradientBoostingClassifier` foi treinado para prever faixas salariais agrupadas.
    2.  A experiência profissional (especialmente "Nível de senioridade" e "Tempo de experiência") e o "Nível de ensino alcançado" são os fatores mais fortemente associados (e provavelmente os mais importantes para o modelo GBT) com a disparidade salarial.
    3.  O GBT é capaz de capturar interações complexas entre formação e experiência implicitamente através de sua estrutura baseada em árvores.

b.  **Relação com a Pergunta Orientadora:**
    A pergunta é: "Como fatores como formação acadêmica e experiência profissional interagem para influenciar a disparidade salarial?"
    * **Influência Direta:** Tanto a formação acadêmica quanto a experiência profissional influenciam diretamente a faixa salarial. Maior experiência e maior nível de formação tendem a levar a salários mais altos.
    * **Interação:** O modelo GBT, ao aprender com os dados, implicitamente modela essa interação. A EDA no `report.md` sugere que o valor da formação acadêmica no salário pode ser potencializado pela experiência. Ou seja, um diploma avançado pode render mais (em termos salariais) para alguém que já acumulou alguns anos de experiência, em comparação com um recém-formado com o mesmo diploma. Da mesma forma, a progressão na carreira através da experiência pode ser mais rápida ou levar a tetos salariais mais altos para aqueles com formação mais robusta. O modelo GBT aprenderia a "premiar" essas combinações favoráveis.

c.  **Limitações da Interpretação/Modelo:**
    1.  **Ausência de `feature_importances_` Diretas:** A falta do cálculo explícito da importância das features do modelo GBT treinado no notebook limita a confirmação direta de quais features o *modelo* considerou mais importantes, dependendo-se do V de Cramer como proxy.
    2.  **Interpretabilidade do GBT:** Modelos GBT são caixas-pretas em maior grau que árvores de decisão únicas. Sem ferramentas como SHAP ou LIME, entender *exatamente* como as interações são modeladas é desafiador.
    3.  **Agrupamento da Variável Alvo:** A variável "Faixa salarial agrupada" simplifica o problema, mas pode mascarar nuances dentro das faixas agrupadas. As interações podem ser diferentes para distinguir salários muito altos versus moderadamente altos, por exemplo.
    4.  **Causalidade vs. Correlação:** O modelo identifica associações e padrões preditivos, mas não estabelece causalidade. Por exemplo, maior experiência leva a maior salário, ou pessoas que recebem maiores salários permanecem mais tempo na área? Provavelmente um ciclo virtuoso, mas o modelo não distingue isso.
    5.  **Features Não Utilizadas ou Latentes:** Outros fatores mencionados no `report.md`, como "habilidades técnicas específicas" ou "qualidade da instituição de ensino", não foram explicitamente modelados como features de entrada e podem interagir com formação e experiência.

-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

# Análise comparativa dos modelos

# Análise comparativa dos modelos da 1º pergunta orientada a dados

## Discussão de Forças e Fragilidades de Cada Modelo

#### Modelo A: `RandomForestClassifier` (Classificação Binária)

* **Fonte do Código:** `new-model1-versao12 (1).ipynb`

##### Forças do Modelo A:

* **Capacidade de Modelar Interações Complexas:**
    * O Random Forest é inerentemente bom em capturar interações não lineares entre features sem a necessidade de especificá-las manualmente. Isso é crucial para a 1ª pergunta orientada a dados do `report.md`, que foca na interação entre formação e experiência. O heatmap de interação gerado no código (`interacao_formacao_experiencia.png`) demonstra essa capacidade.
    * *Conexão com Objetivos:* Contribui diretamente para "compreender os fatores que influenciam a variação salarial" e "identificar padrões e tendências".

* **Fornecimento de Importância das Features:**
    * O modelo fornece uma métrica clara de importância das features, ajudando a identificar quais fatores (formação, experiência, senioridade, etc.) são mais determinantes para a classificação da faixa salarial. No `report.md` (e confirmado pelo código do Modelo A), as top 3 features foram senioridade (`senioridade_encoded`), experiência (`experiencia_profissional_encoded`) e formação (`formacao_academica_encoded`), o que está alinhado com as hipóteses do estudo.
    * *Conexão com Objetivos:* Auxilia na "Identificação de Fatores Relevantes" e na "interpretação dos resultados".

* **Robustez e Generalização:**
    * Sendo um ensemble (bagging), é geralmente robusto a outliers (até certo ponto) e menos propenso a overfitting do que uma única árvore de decisão. A otimização de hiperparâmetros (`min_samples_leaf`, `min_samples_split`) e a validação cruzada no `GridSearchCV` (cv=5) visam melhorar a generalização.
    * *Conexão com Objetivos:* A construção de um "sistema inteligente" confiável requer boa generalização para "auxiliar na equiparação salarial" de forma consistente.

* **Bom Desempenho em Problemas de Classificação Binária:**
    * O Random Forest é um algoritmo forte para tarefas de classificação. A transformação do problema em binário ("Salário Alto" vs. "Salário Baixo/Médio") simplifica a tarefa e foca na distinção de um limiar salarial chave (R$ 8.000/mês, conforme engenharia de features no código).
    * O uso de `sample_weights` e `class_weight='balanced_subsample'`, junto com a otimização do limiar de decisão e a calibração das probabilidades, são boas práticas que melhoram a confiabilidade em cenários com leve desbalanceamento.
    * A acurácia balanceada de 0.8106 no teste, conforme o `report.md`, é um bom resultado para este problema binário.
    * *Conexão com Objetivos:* Permite "aplicar por meio de algoritmos de aprendizado de máquina, a previsão da variação salarial com base nos fatores identificados" de forma eficaz para o problema binário definido.

* **Interpretabilidade Parcial e Visualizações:**
    * Embora ensembles sejam caixas-pretas, a importância das features e a capacidade de visualizar árvores individuais (como feito no código, ex: `arvore_exemplo_simplificada.png`) oferecem alguma interpretabilidade. O heatmap de interação (`interacao_formacao_experiencia.png`) é uma excelente forma de visualizar o efeito combinado de formação e experiência.
    * *Conexão com Objetivos:* Ajuda na "interpretação dos resultados" e na "geração de insights para o mercado".

##### Fragilidades do Modelo A:

* **Variável Alvo Binária Simplificada:**
    * A conversão da "Faixa salarial mensal" em apenas duas classes ("Salário Alto" vs. "Salário Baixo/Médio" com corte em R$ 8.000) perde a granularidade das disparidades salariais. Profissionais ganhando R$ 8.500 e R$ 30.000 estão ambos na mesma classe "Salário Alto", o que limita a profundidade da análise de "variação salarial".
    * *Impacto na Investigação:* Dificulta a compreensão das nuances da disparidade dentro das categorias "Alto" e "Baixo/Médio", que é um dos focos do `report.md`.

* **Interpretabilidade Limitada do Ensemble:**
    * Embora a importância das features seja útil, entender *como* o modelo combina centenas de árvores para chegar a uma decisão específica para um indivíduo é complexo. Explicar as "regras" exatas do modelo para um stakeholder não técnico é desafiador.
    * *Impacto na Investigação:* Pode ser difícil "desenvolver um sistema inteligente para *compreender* os fatores que influenciam a variação salarial" em profundidade apenas com as saídas do Random Forest.

* **Tratamento Ordinal de Features Chave:**
    * `formacao_academica_encoded` e `experiencia_profissional_encoded` são tratadas como numéricas ordinais. Embora haja uma ordem, o modelo de árvore pode tratar os intervalos entre os valores codificados como equidistantes, o que pode não ser verdade (o "salto" de Graduação para Pós pode não ser o mesmo que de Pós para Mestrado em termos de impacto salarial). Isso pode levar a splits subótimos se a relação não for estritamente linear dentro da ordem.
    * *Impacto na Investigação:* A representação da influência dessas variáveis chave pode não ser totalmente precisa, afetando a análise da interação.

* **Sensibilidade a Hiperparâmetros:**
    * Embora o `GridSearchCV` tenha sido usado, Random Forests ainda podem ser sensíveis à escolha da grade de parâmetros. O `max_depth=None` (melhor parâmetro encontrado) pode levar a árvores muito profundas se não bem controlado por `min_samples_leaf` (7) e `min_samples_split` (15).
    * *Impacto na Investigação:* Uma otimização subótima poderia levar a conclusões menos robustas sobre a importância dos fatores.

---

#### Modelo B: `GradientBoostingClassifier` (Classificação Multiclasse)

* **Fonte do Código:** `modelo-1-2-arvore-classificatoria-v5.ipynb`

##### Forças do Modelo B:

* **Análise Granular da Disparidade Salarial:**
    * Ao usar uma variável alvo multiclasse com 6 faixas salariais agrupadas (ex: 'Até R$ 2.000/mês', 'R$ 2.001/mês a R$ 4.000/mês', etc.), o modelo permite uma análise mais detalhada da disparidade salarial do que uma simples classificação binária. É possível ver como os fatores influenciam a probabilidade de pertencer a diferentes níveis de renda.
    * *Conexão com Objetivos:* Alinha-se melhor com "compreender os fatores que influenciam a *variação* salarial" de forma mais ampla, como detalhado no problema do `report.md`.

* **Tratamento Flexível de Features Categóricas com One-Hot Encoding:**
    * Aplicar One-Hot Encoding a todas as features de entrada, incluindo 'Nível de ensino alcançado' e 'Tempo de experiência na área de dados' (que foram tratadas como categóricas antes do OHE no código), evita impor uma relação ordinal que pode não ser linear ou equidistante em seu efeito no salário. Cada categoria (ex: cada nível de ensino, cada faixa de experiência) torna-se uma feature binária independente, permitindo ao modelo aprender seu impacto específico.
    * *Conexão com Objetivos:* Pode levar a uma modelagem mais flexível do impacto das variáveis chave 'formação acadêmica' e 'experiência profissional'.

* **Poder Preditivo do Gradient Boosting:**
    * Gradient Boosting Machines (GBMs) são frequentemente algoritmos de ponta para dados tabulares, capazes de alcançar alta performance através da construção sequencial de árvores que corrigem os erros das anteriores.
    * *Conexão com Objetivos:* Pode levar a uma "previsão da variação salarial com base nos fatores identificados" mais precisa, dentro do contexto multiclasse.

* **Importância das Features e Análise de Associação Inicial:**
    * Assim como o Random Forest, GBMs podem fornecer a importância das features (geralmente baseada no ganho). O código também calcula o V de Cramer para uma análise de correlação inicial entre features e o alvo multiclasse, informando sobre a força da associação antes da modelagem. 'Nível de senioridade' e 'Tempo de experiência' foram identificados como os mais correlacionados com a faixa salarial agrupada.
    * *Conexão com Objetivos:* Ajuda na "Identificação de Fatores Relevantes".

##### Fragilidades do Modelo B:

* **Maior Dificuldade de Interpretação (Multiclasse e Boosting):**
    * Modelos de Boosting são sequenciais e mais complexos de interpretar do que Random Forests. Explicar como as previsões são feitas para 6 classes diferentes é intrinsecamente mais difícil.
    * O `report.md` (baseado na saída do notebook do Modelo B) mostra uma acurácia balanceada de 0.4015 e acurácia geral de 0.5273. Estes valores são mais baixos que os do Modelo A (binário), o que é esperado dada a maior complexidade da tarefa multiclasse. O desempenho foi particularmente baixo para a classe 'Acima de R$ 30.000/mês' (F1-score de 0.11).
    * *Impacto na Investigação:* Torna a "interpretação dos resultados" e a "geração de insights para o mercado" mais desafiadoras, especialmente para classes com baixo desempenho.

* **Sensibilidade a Hiperparâmetros e Risco de Overfitting:**
    * GBMs são conhecidos por serem sensíveis a hiperparâmetros (especialmente `learning_rate` e `n_estimators`). Embora `RandomizedSearchCV` tenha sido usado, a otimização pode ser mais crítica. Há um risco maior de overfitting se não cuidadosamente ajustado, especialmente com o oversampling.
    * *Impacto na Investigação:* Pode levar a um modelo que não generaliza bem para novos dados ou que superestima a importância de certas interações aprendidas no conjunto de treino.

* **Impacto do Oversampling Manual:**
    * O oversampling manual no conjunto de treino para balancear as 6 classes pode introduzir redundância e potencialmente levar a um modelo que se ajusta demais às características das amostras replicadas, especialmente para as classes originalmente minoritárias. A distribuição das classes após o balanceamento mostrou todas as classes com 825 amostras cada.
    * *Impacto na Investigação:* As estimativas de desempenho no conjunto de treino podem ser otimistas, e a importância das features pode ser distorcida se o oversampling não for bem gerenciado.

* **Perda de Informação Ordinal com One-Hot Encoding para 'Nível de Ensino' e 'Experiência':**
    * Ao tratar 'Nível de ensino alcançado' e 'Tempo de experiência na área de dados' como puramente categóricas para o One-Hot Encoding, a informação inerente de ordem (ex: Mestrado > Graduação, 5 anos > 2 anos) é perdida para o modelo, a menos que ele consiga reaprendê-la através das interações e da estrutura das árvores. Isso pode tornar mais difícil para o modelo capturar tendências monotônicas simples.
    * *Impacto na Investigação:* Pode subestimar o impacto progressivo e ordenado dessas variáveis chave, que são centrais para a 1ª pergunta orientada a dados do `report.md`.

---

### Exemplificação de Casos de Superioridade (Imaginação e Extrapolação Fundamentada)

#### Cenários de Superioridade para o Modelo A (RandomForestClassifier - Binário):

1.  **Cenário: Necessidade de uma Ferramenta Rápida para Segmentação de Talentos para Programas de Desenvolvimento.**
    * **Situação:** Uma empresa de RH ou uma grande corporação deseja implementar rapidamente um sistema para identificar, de forma preliminar, quais profissionais de dados em seu banco de talentos ou entre novas contratações têm maior probabilidade de já estar em uma faixa salarial "elevada" (acima de R$8.000) versus aqueles que provavelmente estão abaixo desse patamar. O objetivo é direcionar os de "salário baixo/médio" para programas de desenvolvimento de carreira e os de "salário alto" para posições mais seniores ou de mentoria. A interpretabilidade dos fatores gerais (quais são os 3-5 principais impulsionadores) é importante, mas a distinção binária é o foco.
    * **Por que Modelo A seria superior:**
        * **Simplicidade e Clareza do Alvo:** A classificação binária é mais direta de entender e comunicar. O Modelo A mostrou bom desempenho (acurácia balanceada ~0.81) para esta tarefa simplificada. Para uma triagem inicial, essa distinção pode ser suficiente e mais acionável.
        * **Interpretação dos Fatores Principais:** O Random Forest do Modelo A fornece importâncias de features claras (senioridade, experiência, formação como top 3), que são fáceis de comunicar para justificar a segmentação. O heatmap de interação formação vs. experiência também é um visual poderoso e diretamente relevante para os objetivos do `report.md`.
        * **Robustez e Implementação:** Random Forests são relativamente robustos e fáceis de treinar. A calibração de probabilidades (realizada no Modelo A) também aumenta a confiança nas pontuações usadas para essa segmentação.
    * **Relação com o Problema:** Este cenário se relaciona com a "geração de insights para o mercado" e "auxiliar na equiparação salarial" (ao identificar grupos para desenvolvimento), fornecendo uma ferramenta prática para tomada de decisão em RH. A investigação da interação entre formação e experiência é bem suportada pela visualização gerada.

2.  **Cenário: Análise de Impacto para Políticas de Incentivo à Formação Contínua e Progressão para Senioridade.**
    * **Situação:** Uma associação de profissionais de dados ou um órgão governamental quer entender o impacto marginal de se alcançar um "nível sênior" ou de se obter "formação adicional" (como uma pós-graduação ou mestrado) na probabilidade de um profissional cruzar um limiar salarial específico considerado como um marco de "bem remunerado" (neste caso, R$8.000). O foco não é prever a faixa exata dentro de um espectro, mas sim o "salto" para uma categoria de maior remuneração.
    * **Por que Modelo A seria superior:**
        * **Foco no Limiar Específico:** O Modelo A é treinado especificamente para distinguir acima/abaixo do limiar de R$8.000. A análise das probabilidades calibradas pode mostrar o quão perto um profissional está desse limiar e como mudanças nas features importantes (senioridade, experiência, formação) alteram essa probabilidade.
        * **Visualização de Interação Direta:** O heatmap de "Probabilidade de Salário Alto por Formação Acadêmica e Experiência Profissional" gerado pelo Modelo A é ideal para mostrar como essas duas variáveis, combinadas, afetam a probabilidade de atingir "Salário Alto", informando diretamente políticas de incentivo à qualificação.
        * **Resultados Mais Claros para Decisão Binária:** Para a pergunta "este investimento em formação ou esta promoção para sênior tende a me levar para a faixa acima de R$8k?", o modelo binário oferece uma resposta mais direta e facilmente comunicável.
    * **Relação com o Problema:** Ajuda a "compreender os fatores que influenciam a variação salarial" de forma direcionada a um ponto de corte relevante e a "gerar insights" para o desenvolvimento profissional, alinhado com o objetivo de entender a interação entre formação e experiência.

---

#### Cenários de Superioridade para o Modelo B (GradientBoostingClassifier - Multiclasse):

1.  **Cenário: Desenvolvimento de um Guia Salarial Detalhado para Profissionais de Dados por Nível e Especialização.**
    * **Situação:** Uma plataforma de empregos ou uma consultoria de carreira deseja criar um guia salarial abrangente que não apenas indique se um salário é "alto" ou "baixo", mas que forneça uma estimativa mais granular das faixas salariais prováveis (ex: 'R$4k-R$8k', 'R$8k-R$16k', 'R$16k-R$30k') para diferentes combinações de experiência, formação acadêmica, área de formação, cargo, setor e localização. O objetivo é oferecer um benchmark mais completo.
    * **Por que Modelo B seria superior:**
        * **Granularidade da Previsão:** A capacidade de prever entre 6 faixas salariais agrupadas oferece um detalhamento muito maior da estrutura de remuneração do que uma simples classificação binária. Isso permite identificar não só se alguém ganha bem, mas *quão* bem, dentro de um espectro.
        * **Identificação de Padrões Multiclasse:** O Gradient Boosting, treinado para um alvo multiclasse, pode capturar nuances sobre quais combinações de features levam a faixas salariais intermediárias, não apenas aos extremos. Por exemplo, pode revelar que certos cargos com experiência moderada tendem a se concentrar na faixa de 'R$8k-R$16k', enquanto outros podem saltar mais rapidamente para faixas superiores.
        * **Análise de Transições:** Embora o modelo não seja temporal, as probabilidades para cada classe podem ser usadas para inferir a "próxima faixa salarial mais provável" se um profissional melhorar uma de suas qualificações (ex: ganhar mais experiência ou mudar de área de formação).
    * **Relação com o Problema:** Aborda mais profundamente a "variação salarial" em todo o espectro e pode gerar "insights para profissionais e empresas" sobre expectativas realistas de remuneração em diferentes estágios e especializações, incluindo o impacto da formação e experiência em diferentes níveis de renda.

2.  **Cenário: Investigação de "Gargalos" ou "Saltos" na Progressão Salarial ao Longo da Carreira.**
    * **Situação:** Um estudo socioeconômico quer identificar se existem pontos específicos na carreira de um profissional de dados (em termos de anos de experiência ou transição entre níveis de formação/senioridade) onde ocorrem os maiores "saltos" salariais, ou, inversamente, onde há "gargalos" ou estagnação, dificultando a passagem para faixas salariais mais elevadas.
    * **Por que Modelo B seria superior:**
        * **Múltiplas Faixas como Indicador de Progressão:** As 6 faixas salariais do Modelo B funcionam como degraus. Analisando as features mais importantes para distinguir entre faixas adjacentes (ex: o que diferencia quem está em 'R$4k-R$8k' de quem está em 'R$8k-R$16k'?), pode-se entender melhor os motores da progressão.
        * **Detecção de Limites entre Classes:** O modelo multiclasse pode revelar se, por exemplo, passar de "Graduação" para "Pós-graduação" tem um impacto maior na transição da faixa 'R$X-R$Y' para 'R$Y-R$Z' do que da faixa 'R$Y-R$Z' para 'R$Z-R$W'. Similarmente para anos de experiência.
        * **Flexibilidade do One-Hot Encoding:** Tratar 'Tempo de experiência' e 'Nível de ensino' como one-hot encoded (como no Modelo B) permite que o modelo atribua importâncias e coeficientes diferentes para cada faixa de experiência ou nível de ensino específico, sem assumir uma progressão linear, o que é útil para identificar saltos ou platôs não lineares.
    * **Relação com o Problema:** Este cenário foca em "identificar padrões e tendências" na variação salarial. A análise da interação entre formação e experiência ganha profundidade ao se observar como essa interação se manifesta em diferentes transições de faixas salariais, em vez de apenas um limiar binário.

#### Cenários de Superioridade para o Modelo B (GradientBoostingClassifier - Multiclasse):

1.  **Cenário: Desenvolvimento de um Guia Salarial Detalhado para Profissionais de Dados por Nível e Especialização.**
    * **Situação:** Uma plataforma de empregos ou uma consultoria de carreira deseja criar um guia salarial abrangente que não apenas indique se um salário é "alto" ou "baixo", mas que forneça uma estimativa mais granular das faixas salariais prováveis (ex: 'R\$4k-R\$8k', 'R\$8k-R\$16k', 'R\$16k-R\$30k') para diferentes combinações de experiência, formação acadêmica, área de formação, cargo, setor e localização. O objetivo é oferecer um benchmark mais completo para os profissionais avaliarem sua remuneração e para as empresas definirem faixas salariais competitivas.
    * **Por que Modelo B seria superior:**
        * **Granularidade da Previsão:** A capacidade de prever entre 6 faixas salariais agrupadas (conforme implementado no código do Modelo B) oferece um detalhamento muito maior da estrutura de remuneração do que uma simples classificação binária. Isso permite identificar não só se alguém ganha bem, mas *quão* bem, dentro de um espectro mais amplo.
        * **Identificação de Padrões Multiclasse:** O Gradient Boosting, treinado para um alvo multiclasse, pode capturar nuances sobre quais combinações de features levam a faixas salariais intermediárias, não apenas aos extremos. Por exemplo, pode revelar que certos cargos com experiência moderada tendem a se concentrar na faixa de 'R\$8k-R\$16k', enquanto outros podem saltar mais rapidamente para faixas superiores. Esta granularidade é essencial para um guia salarial detalhado.
        * **Potencial Preditivo do GBM para Dados Tabulares:** Se bem otimizado (como tentado com `RandomizedSearchCV`), Gradient Boosting pode modelar relações complexas e fornecer probabilidades mais refinadas para cada uma das 6 classes, oferecendo um panorama mais completo da distribuição salarial esperada para um perfil específico. O `report.md` indica que o Modelo B teve uma acurácia balanceada de 0.4015 para 6 classes, o que, embora modesto, é um ponto de partida para uma tarefa mais complexa que a binária.
    * **Relação com o Problema:** Aborda mais profundamente a "variação salarial" em todo o espectro e pode gerar "insights para profissionais e empresas" sobre expectativas realistas de remuneração em diferentes estágios e especializações. A análise da interação entre formação e experiência ganha profundidade ao se observar como ela se distribui por múltiplas faixas de renda, não apenas um corte binário.

2.  **Cenário: Investigação de "Gargalos" ou "Saltos" na Progressão Salarial ao Longo da Carreira para Fins de Política Educacional e de Mercado.**
    * **Situação:** Um estudo socioeconômico, ou uma instituição de ensino superior planejando seus cursos, quer identificar se existem pontos específicos na carreira de um profissional de dados (em termos de anos de experiência, tipo de formação, ou transição entre níveis de senioridade) onde ocorrem os maiores "saltos" salariais, ou, inversamente, onde há "gargalos" ou estagnação, dificultando a passagem para faixas salariais mais elevadas. O objetivo é entender onde intervenções (ex: cursos de especialização, programas de aceleração de carreira) seriam mais impactantes.
    * **Por que Modelo B seria superior:**
        * **Múltiplas Faixas como Indicador de Progressão:** As 6 faixas salariais do Modelo B funcionam como degraus em uma escada de progressão. Analisando as features mais importantes para distinguir entre faixas adjacentes (ex: o que diferencia quem está em 'R\$4k-R\$8k' de quem está em 'R\$8k-R\$16k'?), pode-se entender melhor os motores da progressão salarial.
        * **Detecção de Limites e Transições entre Classes:** O modelo multiclasse pode revelar se, por exemplo, passar de "Graduação" para "Pós-graduação" tem um impacto mais significativo na transição da faixa salarial 'A' para 'B' do que da faixa 'B' para 'C'. Similarmente para o acúmulo de anos de experiência – o modelo pode ajudar a identificar se os primeiros anos de experiência promovem saltos entre faixas mais baixas, enquanto a experiência mais avançada é necessária para as faixas superiores.
        * **Flexibilidade do One-Hot Encoding para Variáveis Ordinais:** No Modelo B, 'Tempo de experiência na área de dados' e 'Nível de ensino alcançado' são tratadas como categóricas e passam por One-Hot Encoding. Isso permite que o modelo atribua importâncias e aprenda pesos diferentes para cada faixa de experiência ou nível de ensino específico, sem assumir uma progressão linear ou ordinal estrita em seu impacto. Isso é útil para identificar saltos ou platôs não lineares na remuneração conforme essas variáveis mudam.
    * **Relação com o Problema:** Este cenário foca em "identificar padrões e tendências" na variação salarial de forma dinâmica. A análise da interação entre formação e experiência ganha profundidade ao se observar como essa interação se manifesta em diferentes transições de faixas salariais, em vez de apenas um limiar binário. Os resultados podem informar "políticas públicas, regulamentações e padrões da indústria" mencionados no `report.md` como parte do público-alvo.

