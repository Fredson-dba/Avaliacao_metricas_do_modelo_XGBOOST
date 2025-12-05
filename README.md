# Avaliação e métricas do modelo XGBOOST
 
OBJETIVO

O objetivo é avaliar o desempenho de um modelo XGBoost em Google Colab, utilizando a base de atrasos em voos, e calcular métricas que permitam interpretar sua performance. 

Objetivos específicos: 

Carregar os dados e preparar para predição. 

Treinar um modelo XGBoost no Colab. 

Realizar inferências (probabilidades e classes). 

Calcular métricas de classificação. 

Visualizar resultados em gráficos.

PRÁTICA 2 – AVALIAÇÃO E MÉTRICAS DO MODELO XGBOOST

Um grande site de reservas de viagens vem recebendo diversas reclamações de clientes por causa de atrasos inesperados em voos.

Para melhorar a experiência, a empresa quer criar um recurso que informe, no momento da reserva, a probabilidade de atraso do voo. A proposta é usar dados históricos para analisar fatores como condições climáticas, horário de partida, aeroporto de origem, destino e companhia aérea.

Você faz parte da equipe de ciência de dados e recebeu a tarefa de reconstruir o sistema em Google Colab, preparando os dados, treinando um algoritmo de Machine Learning (XGBoost), avaliando métricas e propondo melhorias para aumentar a precisão do modelo.


🎯 OBJETIVO DA ATIVIDADE

O objetivo é avaliar o desempenho de um modelo XGBoost em Google Colab, utilizando a base de atrasos em voos, e calcular métricas que permitam interpretar sua performance.

Objetivos específicos:

•	Carregar os dados e preparar para predição.
•	Treinar um modelo XGBoost no Colab.
•	Realizar inferências (probabilidades e classes).
•	Calcular métricas de classificação.
•	Visualizar resultados em gráficos.

🧩 DESAFIO PRÁTICO

O seu notebook deve conter, no mínimo:

1.	Importar e preparar os dados

•	Baixar a base de dados flights_delays_120.csv (ver instruções abaixo).
•	Tratar variáveis categóricas e numéricas.
•	Dividir em treino e teste.

2.	Treinar o modelo XGBoost

•	Definir um classificador XGBoost com parâmetros simples.
•	Treinar com os dados de treino.

3.	Predição do modelo

•	Obter probabilidades com predict_proba.
•	Converter para classe binária (threshold 0.5).

4.	Matriz de Confusão

•	Calcular a matriz de confusão.
•	Visualizar em gráfico.

5.	Métricas de desempenho

•	Extrair TP, TN, FP, FN.
•	Calcular Sensibilidade (Recall), Especificidade, FPR, FNR, Acurácia.

6.	Curva ROC e AUC

•	Gerar a curva ROC.
•	Calcular e exibir o AUC.

🛠️ ORIENTAÇÕES TÉCNICAS
Na construção do seu notebook, é obrigatório fazer, se aplicável:


| Etapa | Ações mínimas requeridas | Funções/Ferramentas-chave |
| ----- | ---- | --- |
| Carregar dados | Ler CSV, separar X e y | pd.read_csv, DataFrame |
| Dividir treino/teste | Garantir estratificação | train_test_split(stratify=y) |
| Treinar XGBoost | Ajustar classificador | XGBClassifier().fit() |
| Predição | Probabilidade → binário | predict_proba, comparação com threshold |
| Matriz de confusão | Calcular e visualizar | confusion_matrix, matplotlib |
| Matriz de confusão | Calcular e visualizar | confusion_matrix, matplotlib |
| Métricas | TP/TN/FP/FN, sens., espec., FPR, FNR, acurácia | A partir da confusion_matrix |
| ROC/AUC | Curva ROC e AUC | roc_curve, auc/roc_auc_score |

💡 DICAS

Para facilitar sua pesquisa e aprendizado durante o laboratório, fique de olho em algumas dicas:

- Formato dos dados de teste: revise como preparar corretamente os dados para envio ao endpoint, garantindo o formato esperado (CSV, JSON, etc.) e a correspondência entre variáveis preditoras e rótulos.
- Avaliação de métricas: conheça as funções do sklearn.metrics para calcular as métricas.
- Visualização dos resultados: utilize bibliotecas como matplotlib e seaborn para gerar gráficos e matrizes de confusão que ajudem na interpretação dos resultados.
