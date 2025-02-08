## Configurando o Ambiente para Análise Exploratória de Dados e Predição Para Valores de Aluguéis de Apartamentos em Nova Yorque

Este README fornece instruções para configurar o ambiente no Google Colab e Jupyter Notebook, incluindo como baixar e utilizar o arquivo `teste_indicium_precificacao.cvs` e os requisitos para executar o código de Análise Exploratória de Dados (EDA) e predição.

### 1. Pré-requisitos

* **Conexão com a internet:** Você precisará de uma conexão com a internet para baixar o arquivo `teste_indicium_precificacao.cvs` e instalar as bibliotecas necessárias.
* **Conta do Google:** Para usar o Google Colab, você precisará de uma conta do Google.
* **Anaconda ou Miniconda:** Para usar o Jupyter Notebook, você precisará instalar o Anaconda ou Miniconda.

### 2. Baixando o arquivo `dfbruto.csv`

1. **Faça o download do arquivo:** Clique no seguinte link para baixar o arquivo `teste_indicium_precificacao.cvs`: [https://github.com/henriquecm02/LH_CD_HENRIQUE_COUTO_MACHADO./blob/main/teste_indicium_precificacao.csv](https://github.com/henriquecm02/LH_CD_HENRIQUE_COUTO_MACHADO./blob/main/teste_indicium_precificacao.csv)
   
2. **Salve o arquivo:** Salve o arquivo baixado  em um local acessível no seu computador.

### 3. Google Colab

**Passo 1:** Acesse o Google Colab: [https://colab.research.google.com/](https://colab.research.google.com/)

**Passo 2:** Crie um novo notebook ou abra um existente.

**Passo 3:** Instale as bibliotecas necessárias:

```python
!pip install pandas numpy matplotlib seaborn scikit-learn pickle...
```

**Passo 4:** Carregue o arquivo `teste_indicium_precificacao.cvs` para o Google Colab:

```python
from google.colab import files
uploaded = files.upload()
```

**Passo 5:** Substitua o caminho do arquivo no código com o caminho correto para o seu arquivo no Google Colab:

```python
df = pd.read_csv('teste_indicium_precificacao.cvs', sep=",")
```

**Passo 6:** Execute o código de EDA e predição.

### 4. Jupyter Notebook

**Passo 1:** Instale o Anaconda ou Miniconda: [https://www.anaconda.com/](https://www.anaconda.com/)

**Passo 2:** Crie um novo ambiente virtual (opcional, mas recomendado):

```bash
conda create -n eda_env python=3.8
conda activate eda_env
```

**Passo 3:** Instale as bibliotecas necessárias:

```bash
pip install pandas numpy matplotlib seaborn scikit-learn pickle...
```

**Passo 4:** Crie um novo notebook Jupyter:

```bash
jupyter notebook
```

**Passo 5:** Cole o código de EDA e predição no notebook.

**Passo 6:** Substitua o caminho do arquivo no código com o caminho correto para o seu arquivo no computador:

```python
df = pd.read_csv('teste_indicium_precificacao.cvs', sep=",")
```

**Passo 7:** Execute o código.

### 5. Executando o código

* Certifique-se de que você tenha o arquivo `teste_indicium_precificacao.cvs` no Google Drive ou no diretório local do seu computador.
* Modifique o caminho para o arquivo `teste_indicium_precificacao.cvs` no código para corresponder ao local do seu arquivo.
* Execute cada célula de código no notebook.

### 6. Requisitos

```
pandas==1.5.3
numpy==1.24.2
seaborn==0.12.2
matplotlib==3.7.1
geopandas==0.12.2
missingno==0.5.2
wordcloud==1.9.2
scipy==1.10.1
scikit-learn==1.2.2
joblib==1.3.1
plotly==5.14.1
```

