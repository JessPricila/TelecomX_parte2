📊 Análise de Evasão de Clientes (Churn) e Modelagem Preditiva
📌 Introdução

Este projeto tem como objetivo analisar os fatores que influenciam a evasão de clientes (customer churn) e avaliar diferentes modelos preditivos para identificar clientes com maior risco de cancelamento.

🔎 Etapas Realizadas

Carga e Pré-processamento dos Dados

Expansão de colunas aninhadas

Tratamento de valores ausentes em Charges.Total (mediana)

Limpeza de nomes de colunas e conversão de tipos

Remoção da coluna irrelevante customerID

Análise Exploratória (EDA)

Identificação de desbalanceamento entre classes (churn vs. não churn)

Visualizações: gráficos de barras, matriz de correlação

Análise de distribuição por tipo de contrato e tempo de permanência

Preparação dos Dados

Codificação de variáveis categóricas com One-Hot Encoding

Separação em variáveis preditoras (X) e variável alvo (y)

Divisão em treino (80%) e teste (20%) com estratificação

Modelagem Preditiva

Regressão Logística (com variáveis numéricas escaladas)

Random Forest (com dados originais, não escalados)

Avaliação dos Modelos

Métricas: Acurácia, Precisão, Recall, F1-score e Matriz de Confusão

🧩 Principais Fatores de Evasão

Tipo de Contrato: clientes com contratos mês a mês têm maior propensão ao churn.

Tempo de Permanência (Tenure): clientes novos ou com pouco tempo tendem a evadir mais.

Total Gasto (Charges.Total): clientes com baixo gasto acumulado têm maior risco de churn.

Serviços Contratados:

Telefone → associado a menor evasão

Internet Fibra Óptica e ausência de serviços extras → maior risco de churn

📈 Resultados dos Modelos

Regressão Logística

Acurácia: 77,9%

Precisão (Yes): 0.64

Recall (Yes): 0.55

F1-score (Yes): 0.59

Random Forest

Acurácia: 73,8%

Precisão (Yes): 0.59

Recall (Yes): 0.47

F1-score (Yes): 0.52

👉 A Regressão Logística foi mais eficaz em identificar clientes que realmente evadiram (maior recall e F1-score para a classe minoritária).

💡 Estratégias de Retenção

Criar programas de engajamento para clientes com contratos de curto prazo

Implementar onboarding robusto para novos clientes

Monitorar gasto total e padrões de uso para detectar clientes em risco

Incentivar a adesão a serviços adicionais

Utilizar o modelo preditivo para identificar clientes em risco e agir proativamente

🚀 Próximos Passos

Tratar a classe vazia na variável alvo

Aplicar técnicas de balanceamento de classes (SMOTE, pesos ajustados)

Investir em engenharia de features para melhorar predição

⚡ Projeto focado em reduzir churn e aumentar retenção de clientes através de análise de dados e machine learning.
