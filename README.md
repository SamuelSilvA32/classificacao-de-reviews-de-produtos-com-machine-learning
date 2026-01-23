# 🤖 Classificação de Reviews de Produtos com Machine Learning

Projeto demonstrativo de **Machine Learning aplicado a Processamento de Linguagem Natural (NLP)**, com o objetivo de classificar automaticamente reviews de produtos como **positivos** ou **negativos**.

---

## 📌 Contexto

Empresas que atuam no comércio eletrônico recebem grandes volumes de avaliações textuais de clientes. A classificação automática desses reviews permite monitorar a satisfação dos consumidores e identificar problemas recorrentes nos produtos.

Este projeto simula esse cenário utilizando **dados fictícios**, com foco educacional e de portfólio.

---

## 🎯 Objetivo do Projeto

Desenvolver um modelo de Machine Learning capaz de classificar reviews de produtos como **positivo** ou **negativo**, passando por todas as etapas do pipeline:

- Análise exploratória
- Pré-processamento de texto
- Vetorização
- Treinamento do modelo
- Avaliação e interpretação dos resultados

---

## 📚 Bibliotecas Utilizadas
- **pandas** — manipulação e análise de dados tabulares  
- **numpy** — operações numéricas e suporte computacional  
- **scikit-learn** — pré-processamento, vetorização TF-IDF, modelagem e métricas  
- **matplotlib** — visualização de dados e gráficos  
- **re** — limpeza e normalização de textos (expressões regulares)  
- **collections** — contagem e análise de frequência de palavras

---

## 📊 Conjunto de Dados

- Dataset **fictício**, criado para fins educacionais
- Reviews curtos de produtos eletrônicos
- Classes:
  - `positivo`
  - `negativo`
- Foram inseridos propositalmente:
  - Textos ambíguos
  - Reviews muito curtos
  - Inconsistências entre nota e sentimento

Esses problemas simulam desafios comuns encontrados em dados reais.

---

## 🧹 Pré-processamento de Texto

As seguintes etapas foram aplicadas:

- Normalização (lowercase)
- Remoção de pontuação e números
- Remoção de stopwords
- Preservação do texto original para comparação

---

## 🔢 Vetorização

- Técnica utilizada: **TF-IDF**
- Consideração de unigramas e bigramas
- Limite de features para adequação ao tamanho do dataset

---

## 🤖 Modelo Utilizado

- **Regressão Logística**
- Motivos da escolha:
  - Simplicidade
  - Interpretabilidade
  - Boa performance em tarefas clássicas de NLP

Os dados foram divididos em conjuntos de treino e teste com **estratificação das classes**.

---

## 📈 Avaliação do Modelo

- Accuracy obtido: **0.40**
- Conjunto de teste reduzido (5 observações)
- O modelo apresentou viés em favor da classe positiva

O desempenho limitado era esperado devido a:
- Pouco volume de dados
- Textos curtos
- Alta ambiguidade linguística

As métricas foram analisadas com cautela, priorizando interpretação qualitativa.

---

## 🧠 Principais Insights

- Reviews negativos tendem a conter palavras mais específicas relacionadas a problemas
- Reviews curtos dificultam a classificação correta
- O modelo é sensível à distribuição das classes e ao volume de dados

---

## ⚠️ Limitações

- Dataset pequeno e fictício
- Ausência de validação cruzada
- Avaliação baseada em uma única divisão treino/teste
- Não utilização de técnicas avançadas como embeddings ou deep learning

Este projeto **não tem finalidade produtiva**, sendo voltado exclusivamente ao aprendizado.

---

## 🚀 Possíveis Melhorias

- Aumento do volume e diversidade dos dados
- Balanceamento das classes
- Teste de modelos alternativos (ex.: Naive Bayes)
- Inclusão de uma classe neutra
- Uso de técnicas mais avançadas de NLP

### 🗂 Estrutura do Projeto

📁 classificacao-reviews-produtos
├── assets/
│ └── imagens e gráficos utilizados no relatório
├── data/
│ └── reviews_produtos.csv
├── notebook/
│ └── modelo_classificacao_reviews.ipynb
├── relatorio/
│ └── relatorio_classificacao_reviews.pdf
└── README.md

---

