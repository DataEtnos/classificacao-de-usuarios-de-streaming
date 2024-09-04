Análise de Churn em Serviços de Streaming
Objetivo:
O objetivo deste projeto foi analisar os dados de um serviço de streaming para entender os padrões que influenciam o churn dos clientes, ou seja, a decisão de cancelar a assinatura.

Ferramentas Utilizadas:

Python (Pandas, NumPy, Matplotlib, Seaborn)
Scikit-learn para modelagem preditiva e avaliação
XGBoost para experimentação com modelos baseados em gradiente boosting
Metodologia:

Carregamento e Pré-processamento dos Dados:

O conjunto de dados continha informações como idade, gênero, tipo de assinatura, número de dispositivos conectados, número de serviços de streaming utilizados, entre outros. Valores ausentes foram tratados e colunas irrelevantes foram removidas para focar nas variáveis que mais impactam o churn.
Exploração dos Dados e Visualização:

Para entender melhor os dados, foram gerados gráficos de barras e boxplots, analisando a relação entre variáveis como gênero, tipo de assinatura, número de perfis ativos, e número de serviços de streaming com o churn.

Gráfico 1: Número de Churn por Gênero
![mumero de churned por genero](https://github.com/user-attachments/assets/cb7293ef-c750-42fa-8f00-20d2f01b4119)




Este gráfico mostra a distribuição do churn entre homens e mulheres, revelando que a taxa de churn é semelhante entre os gêneros.

Gráfico 2: Número de Perfis Ativos por Churn
![numero de perfil ativo por churned](https://github.com/user-attachments/assets/3a4d6f06-e614-4616-8e0c-2191e38f0c5c)



Aqui, observamos a relação entre o número de perfis ativos e a taxa de churn. Curiosamente, clientes com 3 perfis ativos apresentam uma menor probabilidade de churn.

Gráfico 3: Número de Serviços de Streaming por Gênero
![numero de serviço por genero](https://github.com/user-attachments/assets/0d33645b-ac94-4ea3-a512-a4fef58dd3f9)

Este gráfico mostra que, em média, as mulheres utilizam ligeiramente mais serviços de streaming que os homens.

Gráfico 4: Número de Serviços de Streaming por Tipo de Assinatura
![numero de serviços de streaming por inscrisção](https://github.com/user-attachments/assets/06978709-9dbb-401f-953c-c1a58e026038)


Ao analisar o número de serviços de streaming utilizados com base no tipo de assinatura, notamos que clientes com assinaturas Premium tendem a utilizar mais serviços de streaming.

Tratamento de Outliers:
![tratamento de outliers](https://github.com/user-attachments/assets/261cfd73-4623-4bbf-9f34-09cd6069a42a)


Utilizando um boxplot, foram identificados e tratados outliers nas variáveis numéricas, garantindo que as análises subsequentes fossem mais robustas.

Gráfico 5: Tratamento de Outliers

O gráfico boxplot destaca a distribuição das variáveis e os outliers que foram removidos ou ajustados no processo.

Modelagem Preditiva:

Após o pré-processamento dos dados, diferentes modelos de machine learning, incluindo Random Forest, Regressão Logística, KNN e XGBoost, foram aplicados para prever o churn dos clientes.
A Regressão Logística apresentou o melhor desempenho com um F1 Score de 70,10%, mostrando-se o modelo mais equilibrado em termos de precisão e recall.
Conclusão: O projeto revelou que variáveis como o tempo na plataforma, o tipo de assinatura, e o número de perfis ativos são fatores chave na propensão ao churn. Com esses insights, estratégias mais direcionadas de retenção de clientes podem ser desenvolvidas.
