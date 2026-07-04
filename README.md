# MVP PUC-Rio: Daniel Lima: Machine Learning & Analytics

# Como acessar o projeto

[![Open in Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/DanielStringLima/MVP_Machile_Learning_202607/blob/main/mvp_machine_learning_e_analytics_Analise_de_Credito_Daniel_Lima.ipynb)

# Objetivo do Projeto
Este projeto apresenta a análise de dados, o pré-processamento e o desenvolvimento de um modelo de Machine Learning utilizando o dataset Loan Approval Prediction Dataset. O objetivo é analisar quais são as variáveis que interferem na aprovação ou reprovação do crédito solicitado e criar um modelo de ML que auxilie na tomada de decisão entre aprovar ou não o crédito para o cliente.

## Etapas Realizadas

* **1 - Descrição do Problema**
* **2 - Hipóteses do Problema**
* **3 - Tipo de Problema**
* **4 - Seleção de Dados**
* **5 - Atributos do Dataset**
* **6 - Importação das Bibliotecas Necessárias e Carga de Dados**
* **7 - Importação dos dados**
* **8 - Conhecendo o dataframe**
    * 8.1 - Diagnóstico visual de dados faltantes
* **9 - Resultados iniciais obtidos**
* **10 - Limpeza e padronização de dados**
* **11 - Conferindo os dados depois da padronização**
* **12 - Análise de Dados**
    * 12.1 - Heatmap (Mapa de calor)
        * 12.1.1 - Heatmap: Resultados
    * 12.2 - Boxplot de renda
        * 12.2.1 - Boxplot renda do solicitante do crédito X aprovação do crédito
    * 12.3 - Histórico de crédito X número de aprovações de crédito
        * 12.3.1 - Gráfico crédito X número de aprovações de crédito
    * 12.4 - Endividamento X aprovação de crédito
        * 12.4.1 - Análise do endividamento familiar
* **13 - Respondendo as hipóteses**
* **14 - Preparação para Modelagem (Z-Score)**
    * 14.1 - Pós padronização
        * 14.1.2 - Gráfico Z-Score
        * 14.1.3 - Visualização gráfica do Z-Score

## Machine Learning & Analytics

* **1 - Preparação dos dados e divisão treino/teste**
    * 1.1 - Baseline e modelos candidatos
        * 1.1.2 - Avaliação de Performance e Comparação dos modelos
            * 1.1.2.1 - Avaliação do desempenho
* **2 - Otimização do Modelo**
    * 2.1 - Resultados alcançados
* **3 - Matriz de confusão: Análise de erros e acertos**
* **4 - Comparação final dos modelos**
* **5 - Limitações e melhorias**

## Conclusão
O objetivo desse MVP foi desenvolver e avaliar um modelo de Machine Learning capaz de auxiliar no processo de análise da concessão de crédito, identificando padrões que permitissem desenvolver um filtro para demonstrar clientes aptos ou não para receber o crédito. A fase inicial do projeto se deu através de uma análise exploratória dos dados, onde as hipóteses levantadas revelaram que o histórico de crédito e o percentual de endividamento dos clientes agem como os indicadores mais críticos para a tomada de decisão do banco. Foi necessário desenvolver métricas personalizadas como a parcela mensal e percentual de endividamento familiar para uma visão mais realista da capacidade de pagamento do cliente.

A etapa de padronização dos dados se mostrou fundamental ao tornar os dados mais adequados para a análise, permitindo responder às hipóteses elencadas. A aplicação do Z-Score tornou as variáveis numéricas comparáveis entre si e contribuiu para a redução do impacto das diferentes escalas, preparando os dados para um treinamento mais consistente.

Na etapa de Machine Learning, foram desenvolvidos um modelo baseline utilizando Regressão Logística e um modelo candidato baseado em Random Forest, otimizado via GridSearchCV. O Random Forest otimizado apresentou melhor desempenho: 79% de acurácia, F1-score de 0,86 para a classe positiva e recall de 99%. Isso demonstra uma elevada capacidade de identificar clientes aptos à concessão, embora o modelo apresente um comportamento mais agressivo, aceitando mais falsos positivos para reduzir ao máximo a rejeição de bons clientes.

A análise da matriz de confusão revelou o equilíbrio estratégico do modelo, que prefere aprovar bons pagadores mesmo correndo o risco de aprovar quem não deveria, evitando negar crédito a quem tem potencial. Este MVP demonstrou que a eficiência de um modelo preditivo depende da qualidade dos dados, do pré-processamento e da correta interpretação das métricas. O modelo funciona como um ótimo filtro inicial e, com melhorias futuras — como variáveis comportamentais e técnicas de balanceamento — terá ainda maior capacidade de apoiar decisões estratégicas na concessão de crédito.
