Análise de Churn em Serviços de Streaming

Descrição do Projeto: Este projeto visa prever a probabilidade de cancelamento de assinatura (churn) de clientes em um serviço de streaming. Utilizando um conjunto de dados com informações sobre idade, gênero, tipo de assinatura, dispositivos conectados, entre outras variáveis, foram aplicadas diversas técnicas de pré-processamento, como tratamento de valores nulos, normalização e codificação de variáveis categóricas.

Ferramentas e Tecnologias Utilizadas:

Python: Pandas, NumPy, Matplotlib, Seaborn
Scikit-learn: Modelos de machine learning (Random Forest, Regressão Logística, KNN), processamento de dados (OneHotEncoder, StandardScaler), e técnicas de otimização (GridSearchCV)
XGBoost para experimentação adicional com um modelo baseado em gradiente boosting
Principais Desafios: O maior desafio enfrentado foi lidar com dados faltantes e valores infinitos gerados durante os cálculos, como ao dividir o tempo na plataforma pelo número de serviços de streaming. Para isso, técnicas de imputação e substituição de valores foram aplicadas para manter a integridade dos dados.

Resultados e Insights: Os modelos foram avaliados usando métricas de F1-Score, precisão e recall. O modelo de Regressão Logística apresentou o melhor equilíbrio entre essas métricas com um F1-Score de 70,10%, superando o KNN e Random Forest. A análise mostrou que variáveis como o tempo na plataforma e o tipo de assinatura estão fortemente correlacionadas com a propensão ao churn.

Conclusão: Este projeto demonstra a aplicação prática de técnicas de machine learning em um problema de negócios real, onde a identificação de clientes propensos a cancelar a assinatura pode ajudar a empresa a desenvolver estratégias de retenção mais eficazes.
