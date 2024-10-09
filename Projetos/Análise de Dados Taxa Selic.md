Base de dados:
https://basedosdados.org/dataset/3734fdcf-92d4-4a34-82c0-774ca9978c8e?table=7c195a3a-4010-4367-87c8-8c53d0bff627

Import
```
import basedosdados as bd
billing_id = <seu_billing_id> 

query = """ 
	SELECT 
		dados.data as data, 
		dados.valor as valor 
	FROM `basedosdados.br_bcb_taxa_selic.taxa_selic` AS dados 
""" 
bd.read_sql(query = query, billing_project_id = billing_id)
```
### **Projeto Básico: Análise da Evolução da Taxa Selic no Brasil**

#### **Objetivo do Projeto:**

O objetivo deste projeto é analisar a evolução da taxa Selic ao longo dos anos no Brasil, observando suas variações e possíveis relações com eventos econômicos importantes, como inflação. O projeto visa apresentar tendências de forma visual e explicar como mudanças na Selic impactam a economia.

---

### **Etapas do Projeto**

### 1. **Coleta de Dados**

- **Fonte de Dados:** Baixe os dados da **taxa Selic** de fontes confiáveis, como:
    - **Banco Central do Brasil (SGS API)**, que possui dados históricos detalhados da Selic.
    - Alternativamente, você pode utilizar plataformas como Kaggle ou Trading Economics, que também fornecem dados econômicos.
- **Indicador Principal:**
    - **Taxa Selic (% ao ano)**: A taxa básica de juros da economia brasileira.
- **Período de análise:** Escolha um período relevante, como os últimos **10 a 20 anos** (por exemplo, 2000 a 2023), para capturar tendências de curto e longo prazo.

### 2. **Limpeza e Preparação dos Dados**

- **Carregar os dados:** Após obter os dados, você precisará organizá-los em um formato adequado para análise (geralmente em tabelas, como CSV ou Excel).
- **Tratar valores ausentes:** Certifique-se de que não existam valores ausentes ou inconsistentes que possam prejudicar a análise.
- **Filtrar o período de interesse:** Caso o conjunto de dados inclua períodos anteriores ou dados que não sejam relevantes, filtre para o período desejado (por exemplo, de 2000 a 2023).

### 3. **Análise Descritiva dos Dados**

- **Resumo Estatístico:**
    - Calcule métricas básicas como **média**, **mediana**, **valores máximos e mínimos** da taxa Selic ao longo do período analisado.
    - Compare a variação da Selic ano a ano e verifique se há períodos de alta ou queda acentuada.
- **Volatilidade da Selic:** Identifique períodos em que a Selic apresentou maior ou menor volatilidade (mudanças abruptas na taxa) e possíveis fatores econômicos que influenciaram essas variações.

### 4. **Visualização dos Dados**

- **Gráfico de Linhas:** Crie um gráfico de linhas que mostre a evolução da taxa Selic ao longo dos anos, facilitando a visualização de suas tendências de alta e baixa.
- **Gráfico de Barras:** Outra possibilidade é criar um gráfico de barras que compare a taxa Selic ano a ano, destacando as variações mais significativas.
- **Objetivo das visualizações:** As visualizações ajudam a identificar os períodos de alta e baixa da taxa de forma mais clara e permitem ao leitor entender rapidamente como a Selic tem evoluído.

### 5. **Análise de Correlações (opcional)**

- **Relação com a Inflação (IPCA):** Você pode ampliar o projeto coletando dados da **inflação (IPCA)** no mesmo período e analisar a correlação entre a taxa Selic e a inflação.
- **Análise de correlação:** Verifique se há uma relação entre o aumento da Selic e a redução da inflação, ou se o movimento é oposto. Esse tipo de análise pode ajudar a entender o papel da Selic no controle da inflação.
- **Outras variáveis:** Além da inflação, você pode tentar relacionar a Selic com outras variáveis econômicas, como crescimento do PIB ou taxas de câmbio.

### 6. **Conclusões Simples**

- **Tendências identificadas:** Comente sobre os períodos em que a taxa Selic esteve mais alta ou baixa e como esses períodos se relacionam com o contexto econômico do Brasil (como recessões ou crises).
- **Impactos econômicos:** Explique como variações na taxa Selic podem impactar a economia brasileira, como no crédito, consumo e investimentos.
- **Relação com inflação (se aplicável):** Se você incluiu a análise de correlação com a inflação, destaque se a Selic foi eficaz em conter a inflação em determinados períodos e explique o impacto disso.

---

### **Estrutura do Projeto (README.md)**

- **Título:** Análise da Evolução da Taxa Selic no Brasil (2000–2023)
- **Objetivo:** Analisar a variação da taxa Selic ao longo dos últimos anos e identificar suas tendências e impacto na economia.
- **Fontes de Dados:** Banco Central do Brasil ou outras fontes confiáveis de dados econômicos.
- **Ferramentas Utilizadas:**
    - Ferramentas de manipulação de dados (Pandas).
    - Ferramentas de visualização (Matplotlib, Seaborn).
    - (Opcional) Análise de correlação com a inflação (IPCA).
- **Resultados:** Tendências da Selic, principais variações, impacto econômico e possíveis correlações com outras variáveis, como inflação.

---

### **Extensões do Projeto (para aprofundamento futuro)**

- **Dashboards Interativos:** Usar ferramentas como **Streamlit** ou **Dash** para criar um painel interativo onde os usuários possam selecionar diferentes períodos de análise e visualizar as mudanças da Selic.
- **Previsões da Taxa Selic:** Desenvolver modelos preditivos usando técnicas de machine learning ou séries temporais (como ARIMA) para prever a evolução da taxa Selic com base nos dados históricos.

---

Esse planejamento envolve uma análise simples e objetiva da taxa Selic, com foco na compreensão das suas tendências ao longo dos anos. Mesmo sem entrar em detalhes técnicos complexos, você conseguirá desenvolver uma análise relevante para seu portfólio de dados aplicados à economia.