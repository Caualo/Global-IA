# Predição de Eventos Climáticos Extremos

## Visão Geral

Este projeto desenvolve um modelo de Machine Learning para **predizer o número de eventos climáticos extremos** com base em variáveis ambientais e climáticas globais. Utilizando dados de 15 países coletados entre 2000-2023, o projeto aplica técnicas avançadas de ciência de dados para entender e prever padrões de eventos extremos relacionados às mudanças climáticas.

## Objetivo

Desenvolver um modelo preditivo capaz de estimar o número de eventos climáticos extremos (tempestades, enchentes, secas, etc.) que um país pode experimentar com base em:
- Temperatura média
- Emissões de CO2
- Nível do mar
- Precipitação
- População
- Energia renovável
- Área florestal

## Dataset

### Características dos Dados
- **Registros**: 1.000 amostras
- **Período**: 2000-2023 (24 anos)
- **Países**: 15 países diversos
- **Variáveis**: 10 features originais

### Variáveis do Dataset
| Variável | Tipo | Descrição |
|----------|------|-----------|
| Year | Inteiro | Ano de registro (2000-2023) |
| Country | Categórica | País ou região |
| Avg Temperature (°C) | Float | Temperatura média anual |
| CO2 Emissions (Tons/Capita) | Float | Emissões de CO2 per capita |
| Sea Level Rise (mm) | Float | Elevação anual do nível do mar |
| Rainfall (mm) | Inteiro | Precipitação total anual |
| Population | Inteiro | População do país |
| Renewable Energy (%) | Float | Porcentagem de energia renovável |
| Extreme Weather Events | Inteiro | **TARGET**: Número de eventos extremos |
| Forest Area (%) | Float | Porcentagem de área florestal |

## Tecnologias Utilizadas

### Linguagem e Bibliotecas
```python
# Core
Python 3.8+
pandas 1.5+
numpy 1.21+

# Machine Learning
scikit-learn 1.1+
xgboost 1.6+

# Visualização
matplotlib 3.5+
seaborn 0.11+

# Estatística
scipy 1.9+
```

### Ferramentas
- **Jupyter Notebook** - Desenvolvimento e análise
- **Git** - Controle de versão
- **GitHub** - Repositório



## Metodologia

### 1. Análise Exploratória
- **Estatísticas descritivas** de todas as variáveis
- **Análise de correlações** entre features e target
- **Visualizações temporais** e geográficas
- **Identificação de outliers** e padrões

### 2. Preparação dos Dados
- **Feature Engineering**: 20+ novas variáveis criadas
  - Interações entre variáveis
  - Índices compostos (pressão climática, saúde ambiental)
  - Variáveis temporais e categóricas
- **Normalização** com StandardScaler
- **Encoding** de variáveis categóricas
- **Seleção** das 20 features mais importantes

### 3. Modelagem
Algoritmos testados:
- **Linear Regression** (baseline)
- **Ridge/Lasso Regression** (regularização)
- **Random Forest** (ensemble)
- **Gradient Boosting** (boosting)
- **XGBoost** (state-of-the-art)
- **Support Vector Regression** (kernel-based)
- **Neural Networks** (deep learning)


### Insights Principais
1. **Correlações fracas** entre variáveis individuais e eventos extremos
2. **Necessidade de feature engineering** para capturar padrões complexos
3. **Modelos ensemble** (Random Forest, XGBoost) apresentam melhor performance
4. **Variáveis de interação** são mais preditivas que variáveis isoladas

## Features Mais Importantes

As features com maior poder preditivo identificadas pelo modelo:

1. Índice de Pressão Climática
2. Interação Temperatura-CO2
3. Razão Precipitação-Temperatura
4. Índice de Saúde Ambiental
5. Variáveis geográficas (países específicos)

## Aplicações Práticas

### Uso Potencial
- **Planejamento governamental** para preparação de emergências
- **Seguros climáticos** para precificação de riscos
- **ONGs ambientais** para alocação de recursos
- **Pesquisa científica** em mudanças climáticas


### Datasets
- [Climate Change Dataset](fonte-do-dataset)

### Artigos Científicos
- IPCC Climate Change Reports
- Machine Learning for Climate Science
- Extreme Weather Event Prediction Studies

### Bibliotecas e Ferramentas
- [Scikit-learn Documentation](https://scikit-learn.org/)
- [XGBoost Documentation](https://xgboost.readthedocs.io/)
- [Pandas Documentation](https://pandas.pydata.org/)
