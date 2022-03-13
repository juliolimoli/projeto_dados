# projeto_dados
Projeto final da Let's Code

Autores:

Júlio Limoli </br>
Marcos Peixoto </br>
Victor Araki </br>

## Passo a passo

### 1. Databricks_DE.dbc

Fazer o upload do dataset inicial no DBFS e executar o notebook "Databricks_DE.dbc", ele irá gerar o Data Lake com os dados brutos, um staging table com as conversões de formato e por fim um tabelão Data Warehouse com filtragem inicial de features. O tabelão deve ser baixado em "projeto_dados/bases/application_train_filtered.csv" (Necessário criar a pasta "bases")

### 2. split_DE.ipynb

Utilizar o "split_DE.ipynb" para criar a tabela com separação entre treino e validação. A separação é realizada por uma coluna chamada "Flag_Treino", onde é verdadeira se o dado pertencer ao treino. A tabela criada é nomeada "application_splitado_07.csv" e é armazenada dentro de "/bases/"

### 3. Parte_DS_final

Esse notebook possui os 5 requisitos obrigatórios da parte de Data Science, além de gerar o modelo final utilizado para aplicar no dataset de testes.

**ATENÇÃO:** Devido à seleção de features por RFE o notebook pode demorar mais de 1h para completar. 

## 1. Entrega Data Engineer

1.1 Notebook (Databricks): **Databricks_DE.dbc**

1.2 Arquivo .csv: **dados_modelos.csv**

1.3 Notebook: **split_DE.ipynb**

## 2. Entrega Data Science

2.1 Base com as predições: **resultado_test_student.csv**

2.2 Notebook com a criação do modelo: **parte_DS_final.ipynb**
