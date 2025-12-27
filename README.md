# 🍷 Wine Outlier Analysis

[![Notebook](https://img.shields.io/badge/Jupyter-Notebook-orange?logo=jupyter)](wine_outlier_analysis_full.ipynb)
[![Python](https://img.shields.io/badge/python-3.7%2B-blue)](https://www.python.org/)
[![PyOD](https://img.shields.io/badge/PyOD-Outlier%20Detection-red)](https://pyod.readthedocs.io)
[![License](https://img.shields.io/badge/license-MIT-green)](LICENSE)

## 📌 Visão Geral

Este projeto contém um **Jupyter Notebook** que realiza uma análise comparativa de detecção de outliers no **Wine Dataset** (UCI Machine Learning Repository) utilizando diversos algoritmos da biblioteca **PyOD**. O objetivo é demonstrar como diferentes métodos se comportam ao identificar instâncias atípicas em um conjunto de dados multivariado.

---

## 📁 Conteúdo do Repositório

- 📄 `wine_outlier_analysis_full.ipynb`  
  Notebook completo com:
  - Carregamento e preparação dos dados
  - Aplicação de vários detectores de outliers
  - Visualizações com PCA
  - Gráficos de scores ordenados
  - Curvas ROC / AUC para comparação dos modelos

---

## 🧠 Detalhes da Análise

### 🧾 Dados

Usamos o **Wine Dataset** com:

- 178 amostras de vinhos italianos
- 13 atributos físico-químicos
- 1 rótulo de classe (tipo de vinho): utilizado apenas para referência visual

Os dados são carregados diretamente da URL oficial do **UCI Machine Learning Repository**.

---

## 🔍 Detectores de Outliers

Usamos os seguintes algoritmos do PyOD:

| Método             | Abordagem                                        |
|--------------------|--------------------------------------------------|
| **KNN**            | Distância de vizinhança                          |
| **LOF**            | Local Outlier Factor                              |
| **IsolationForest**| Florestas de isolamento                          |
| **OneClassSVM**    | SVM de classe única                              |
| **ECOD**           | Distribuição empírica                             |
| **HBOS**           | Histogram-based Outlier Score                     |
| **ABOD**           | Ângulo-based Detection                            |
| **FastABOD**       | Versão acelerada de ABOD                          |
| **COPOD**          | Copula-based Outlier Detection                    |
| **MAD**            | Median Absolute Deviation                         |
| **SOS**            | Stochastic Outlier Selection                      |

---

## 📊 Visualizações Incluídas

O notebook gera:

- 📌 **PCA 2D**: projeção dos dados destacando outliers
- 📈 **Scores ordenados**: comparação dos valores de anomalia entre métodos
- 📉 **Curvas ROC / AUC**: avaliação comparativa de cada detector

Essas visualizações ajudam a interpretar o desempenho qualitativo e quantitativo dos métodos.

---

## 🛠️ Como Rodar

### 🔧 Requisitos

Instale as dependências:

```bash
pip install pyod scikit-learn pandas matplotlib seaborn
# wine_outlier_analysis_full
