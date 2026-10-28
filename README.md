# Classificador de Avaliações de Clientes (Customer Review Classifier)

[Português](#português) | [English](#english)

> **Projeto em andamento / Work in progress** (previsão / expected: nov/2026)


## Português

### O problema de negócio
Em e-commerce e delivery, milhares de avaliações chegam todos os dias. Ler uma por uma não escala, e reclamações importantes se perdem. Trabalhei como Team Leader de satisfação do cliente e vi isso de perto: quanto antes o time entende **por que** o cliente está insatisfeito, mais rápido ele age.

**Objetivo:** classificar automaticamente o sentimento (positivo ou negativo) de avaliações escritas em português e resumir os principais motivos de reclamação para o time de atendimento.

### Dados
[Brazilian E-Commerce Public Dataset by Olist](https://www.kaggle.com/datasets/olistbr/brazilian-ecommerce): avaliações reais de clientes com nota de 1 a 5 e comentário em português.
- Rótulo: notas 1 e 2 = **negativo**; notas 4 e 5 = **positivo** (nota 3 removida por ser neutra).

### Abordagem
1. **Análise exploratória:** distribuição das notas, tamanho dos comentários, palavras mais frequentes por sentimento.
2. **Modelo base (baseline):** TF-IDF + Regressão Logística (scikit-learn).
3. **Comparação:** modelo pré-treinado de sentimento do Hugging Face.
4. **Avaliação:** acurácia, F1 e matriz de confusão no conjunto de teste.
5. **Demonstração:** app em Gradio publicado no Hugging Face Spaces.

### Resultados
Em andamento. Aqui vão entrar a comparação entre os modelos (acurácia e F1), os erros mais comuns e os próximos passos.

### Links
- Notebook no Kaggle: em breve
- Demo no Hugging Face: em breve

### Tecnologias
Python, pandas, scikit-learn, Hugging Face Transformers, Gradio

### Como rodar
```bash
pip install -r requirements.txt
jupyter notebook notebooks/classificador.ipynb
```

## English

### Business problem
E-commerce and delivery companies receive thousands of reviews every day. Reading each one doesn't scale, and important complaints get lost. As a Customer Satisfaction Team Leader, I saw this firsthand: the sooner a team understands **why** a customer is unhappy, the faster it can act.

**Goal:** automatically classify the sentiment (positive or negative) of Portuguese-language reviews and summarize the main complaint reasons for the support team.

### Data
[Brazilian E-Commerce Public Dataset by Olist](https://www.kaggle.com/datasets/olistbr/brazilian-ecommerce): real customer reviews with 1–5 scores and Portuguese comments.
- Label: scores 1–2 = **negative**; scores 4–5 = **positive** (score 3 removed as neutral).

### Approach
1. **Exploratory analysis:** score distribution, comment length, most frequent words by sentiment.
2. **Baseline:** TF-IDF + Logistic Regression (scikit-learn).
3. **Comparison:** pretrained sentiment model from Hugging Face.
4. **Evaluation:** accuracy, F1 and confusion matrix on the test set.
5. **Demo:** Gradio app on Hugging Face Spaces.

### Results
In progress. This section will compare the models (accuracy and F1), the most common errors and next steps.

### Links
- Kaggle notebook: coming soon
- Hugging Face demo: coming soon

### Tech stack
Python, pandas, scikit-learn, Hugging Face Transformers, Gradio

Autora / Author: Beatriz De Araújo
