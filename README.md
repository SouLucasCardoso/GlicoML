# GlicoML: Previsão de Risco de Diabetes com Machine Learning Clássico

O **GlicoML** é um projeto acadêmico desenvolvido como requisito final para a disciplina de Machine Learning no curso de Engenharia de Computação da **SATC**. O objetivo é auxiliar no diagnóstico precoce de diabetes utilizando algoritmos de classificação supervisionada em dados clínicos.

## 📋 Sobre o Projeto

O diabetes é uma condição crônica que afeta milhões de pessoas, e sua detecção precoce é fundamental para evitar complicações graves. Este projeto visa resolver o problema de diagnóstico tardio, que muitas vezes depende de análises clínicas demoradas, propondo um modelo preditivo baseado em dados fisiológicos.

O sistema classifica pacientes em duas categorias:
* **0:** Não diabético 
* **1:** Diabético

## 🚀 Tecnologias Utilizadas

O projeto foi desenvolvido em **Python**, utilizando o ambiente **Google Colab**. As principais bibliotecas empregadas foram:

* **Manipulação de Dados:** `pandas`, `numpy` 
* **Visualização:** `matplotlib`, `seaborn` 
* **Machine Learning:** `scikit-learn` 

## 📊 Dataset

Utilizou-se o **Pima Indians Diabetes Dataset**, uma base de dados pública e renomada na área da saúde.
* **Dimensões:** 768 registros e 9 colunas.
* **Variáveis:** Gravidez, Glicose, Pressão Sanguínea, Espessura da Pele, Insulina, IMC, DiabetesPedigreeFunction, Idade e Outcome (variável alvo).

## ⚙️ Metodologia (Pipeline)

O desenvolvimento seguiu um pipeline estruturado de Machine Learning:

1.  **Análise Exploratória (EDA):** Verificação de distribuição das classes, correlações (destaque para Glicose vs Outcome) e ausência de valores nulos.
2.  **Pré-processamento:**
    * Divisão dos dados em treino (70%) e teste (30%) com estratificação.
    * Padronização dos dados utilizando `StandardScaler` para otimizar modelos sensíveis à escala.
3.  **Modelagem:** Treinamento de cinco algoritmos clássicos:
    * Regressão Logística (LR)
    * Support Vector Machine (SVM)
    * K-Nearest Neighbors (KNN)
    * Naive Bayes (GaussianNB)
    * Árvores de Decisão (Decision Tree)
4.  **Avaliação:** Análise comparativa utilizando métricas como Acurácia, Precisão, Recall, F1-Score e Matriz de Confusão.

## 📈 Resultados e Conclusão

Os experimentos demonstraram que técnicas de Machine Learning podem prever diabetes com boa eficiência. Os modelos que utilizam dados padronizados, especificamente o **SVM** e a **Regressão Logística**, apresentaram os melhores desempenhos gerais.

A métrica **F1-Score** foi priorizada na seleção do melhor modelo, dado o leve desbalanceamento das classes e a importância de equilibrar precisão e recall em diagnósticos médicos.

## 👨‍💻 Autores

* **Kaique Demetrio** - [GitHub](https://github.com/kaiquedm12)
* **Paulo de Souza Fontanela** - [GitHub](https://github.com/paulos-f)
* **Lucas Cardoso Rodrigues** - [GitHub](https://github.com/SouLucasCardoso)

---
*Desenvolvido na SATC - Educação e Tecnologia (2025)* 
