# Regressão e Séries Temporais — Entrega 5

Entrega da Semana 5 da Capacitação de Ciência de Dados. O notebook reúne três práticas independentes — Regressão Linear, Regressão Logística e Séries Temporais — cada uma seguindo a sequência: Exploração Inicial, EDA, modelagem e interpretação dos resultados.

## 📂 Estrutura

### 1) Regressão Linear — House Price
**Objetivo:** prever o preço de imóveis (`House_Price`) a partir da metragem quadrada (`Square_Footage`).

- **EDA:** verificação de dimensões, nulos, duplicados e outliers (IQR); histogramas, dispersão e matriz de correlação.
- **Modelo:** Regressão Linear simples, com `Square_Footage` como variável mais correlacionada ao preço.
- **Resultados:** R² de treino 0,982 e de teste 0,983; RMSE ≈ R$ 32.886 — o modelo explica cerca de 98,3% da variação nos preços.

### 2) Regressão Logística — Bank Customer Churn
**Objetivo:** prever a probabilidade de um cliente cancelar a conta no banco (`churn`).

- **EDA:** distribuição de churn, tenure, taxa de churn por gênero e país, boxplot de idade por churn, matriz de correlação; outliers em `age` e `credit_score` mantidos por representarem perfis reais.
- **Tratamento:** one-hot encoding de `country` e `gender`.
- **Modelo:** Regressão Logística.
- **Resultados:** acurácia de 81,5% e AUC de 0,76 — o modelo identifica bem quem permanece, mas tem mais dificuldade com quem cancela (classes desbalanceadas). Clientes da Alemanha, mais velhos e com menos produtos contratados apresentam maior probabilidade de churn.

### 3) Séries Temporais — AirPassengers
**Objetivo:** analisar a evolução do número de passageiros aéreos (1949–1960) e prever o próximo ano.

- **EDA:** série temporal ao longo do tempo, médias e totais anuais, boxplot por mês, decomposição em tendência/sazonalidade/ruído.
- **Modelo:** Holt-Winters (tendência aditiva, sazonalidade multiplicativa), validado com os últimos 12 meses como teste.
- **Resultados:** tendência de crescimento consistente e sazonalidade anual, com pico em julho/agosto; previsão gerada para os 12 meses seguintes (1961).

## 🛠️ Tecnologias utilizadas
- Python (pandas, numpy, matplotlib, seaborn)
- scikit-learn (Regressão Linear, Regressão Logística, métricas, curva ROC)
- statsmodels (Holt-Winters, decomposição sazonal)
- scipy (função sigmoide)

## 📊 Datasets
- [House Price Prediction](https://www.kaggle.com/datasets/prokshitha/home-value-insights)
- [Bank Customer Churn Prediction](https://www.kaggle.com/datasets/gauravtopre/bank-customer-churn-dataset)
- [Air Passengers](https://www.kaggle.com/datasets/rakannimer/air-passenger
   ```
## 👩‍💻 Autora

**Ana Beatriz Mendes de Sousa**  
[![LinkedIn](https://img.shields.io/badge/LinkedIn-0077B5?style=flat&logo=linkedin&logoColor=white)](https://linkedin.com/in/ana-beatriz-mendes-de-sousa)
[![GitHub](https://img.shields.io/badge/GitHub-100000?style=flat&logo=github&logoColor=white)](https://github.com/beatrizzmendees)
