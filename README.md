# 🏨 Análise de Dados Airbnb RJ

Este projeto tem como objetivo realizar **limpeza, tratamento e transformação de dados** de anúncios do Airbnb no Rio de Janeiro.  
A análise inclui:

- Integração de datasets
- Tratamento de valores ausentes
- Detecção e remoção de outliers utilizando o método **IQR**
- Transformação de variáveis categóricas
- Preparação dos dados para futuras análises e modelagens

---

## 📁 Arquivos do projeto

- `notebook_preprocessamento.ipynb` — código completo do pré-processamento  
- `listings_cleaned.csv` — dataset principal do Airbnb  
- `reviews.csv` — dataset com avaliações  
- `README.md` — documentação do projeto

---

## 🧹 Etapas do Pré-processamento

### ✔️ 1. Carregamento e unificação das bases  
Os datasets `listings_cleaned.csv` e `reviews.csv` são importados e mesclados utilizando a coluna `id`.

### ✔️ 2. Tratamento de valores ausentes  
Valores nulos são tratados com média, moda ou preenchimento específico, dependendo da coluna.

### ✔️ 3. Detecção e tratamento de outliers (IQR)  
O método **Interquartile Range (IQR)** foi utilizado para identificar e remover valores discrepantes da coluna `price`.

### ✔️ 4. Transformação de variáveis categóricas  
- `room_type` → categorizado e convertido em códigos numéricos  
- `neighbourhood_cleansed` → transformado utilizando *target encoding* (média dos preços por bairro)

---

## 📊 Resultados

Após o pré-processamento, o dataset final está:

- livre de valores ausentes críticos  
- sem outliers extremos de preço  
- com variáveis categóricas tratadas  
- pronto para análises, dashboards ou modelos preditivos  

---

## 🛠️ Tecnologias Utilizadas

- Python  
- Pandas  
- Matplotlib  
- Google Colab  
- Jupyter Notebook  

---

## 🚀
