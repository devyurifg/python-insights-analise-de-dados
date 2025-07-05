# Análise de Cancelamentos com Python e Pandas

Você foi contratado por uma empresa com **50.000 clientes** para um projeto de Dados.  
Recentemente, a empresa percebeu que **a maioria dos seus clientes são inativos**, ou seja, já cancelaram o serviço.

Precisando melhorar seus resultados, ela deseja entender **os principais motivos desses cancelamentos** e descobrir **ações mais eficazes para reduzir esse número**.

## Funcionalidades

- Leitura dos dados de cancelamento em formato CSV (`cancelamentos_sample.csv`)
- Análise de motivos de cancelamento, localização e datas
- Agrupamentos e contagens com `pandas`
- **Visualizações interativas** com `plotly.express`, como:
  - Gráficos de barras
  - Gráficos de pizza

## Exemplo de Uso (em Jupyter Notebook)

A análise é feita passo a passo em células. Por exemplo:

```python
# Importando bibliotecas principais
import pandas as pd
import plotly.express as px

# Lendo os dados
df = pd.read_csv('cancelamentos_sample.csv')
df.head()
```

```python
# Analisando os motivos de cancelamento
df['motivo'].value_counts()
```

```python
# Visualizando com gráfico de barras interativo
fig = px.bar(df, x='motivo', title='Motivos de Cancelamento')
fig.show()
```

## Conceitos Envolvidos

- Análise de Dados com Pandas
- Visualizações interativas com Plotly Express
- Limpeza e inspeção de dados
- Agrupamentos e contagem de frequências
- Programação com Jupyter Notebooks

## Tecnologias Usadas

- **Python 3.x**
- Pandas
- Plotly Express
- Jupyter Notebooks

## Autor

[Yuri Ferreira Gomes](https://github.com/devyurifg)
📧 devyurifg@gmail.com
