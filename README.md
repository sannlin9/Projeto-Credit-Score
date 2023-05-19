# Credit Score

## Resumo.
### O projeto tem como objetivo criar um modelo de machine learning para o score de crédito, abrangendo todo o pipeline de processamento dos dados. O processo envolve as seguintes etapas:

1. Dados do projeto: Trata-se de um problema de credit scoring para cartão de crédito, utilizando uma amostra de 15 safras coletadas entre janeiro de 2015 e março de 2016. O objetivo é prever se um cliente entrará em inadimplência ou não pagará suas dívidas. Os clientes inadimplentes são marcados como "maus" no conjunto de dados.

![image](https://github.com/sannlin9/Projeto-Credit-Score/assets/125318548/cb224e60-6b4d-46f2-96d6-50b957ece596)


2. Exploração de dados: Os dados coletados são explorados para entender sua estrutura, distribuição, correlações e possíveis padrões. Isso envolve a análise estatística dos dados, a visualização de gráficos e a identificação de insights relevantes.

![image](https://github.com/sannlin9/Projeto-Credit-Score/assets/125318548/21bf3901-bd38-4c93-977b-feebe2a1a90c)


3. Limpeza e pré-processamento dos dados: Nesta fase, os dados são submetidos a um processo de tratamento que envolve lidar com valores faltantes, codificar variáveis categóricas, normalizar ou padronizar variáveis numéricas, identificar e tratar outliers, e outras transformações necessárias.

![image](https://github.com/sannlin9/Projeto-Credit-Score/assets/125318548/4f270f0e-8562-4d1d-a639-4f6580c2270b)
![image](https://github.com/sannlin9/Projeto-Credit-Score/assets/125318548/0aded210-edac-4425-b1bf-d607738a88ed)


4. O modelo: Após o tratamento adequado dos dados, utilizou-se a ferramenta pycaret para o treinamento do modelo e ajuste de hiperparâmetros. O algoritmo de machine learning escolhido foi o Light Gradient Boosting Machine devido ao seu bom desempenho e baixo custo computacional.

![image](https://github.com/sannlin9/Projeto-Credit-Score/assets/125318548/2627d998-76c0-4b73-bddc-6a047d0e1032)

O modelo apos treinamento:

![image](https://github.com/sannlin9/Projeto-Credit-Score/assets/125318548/111fd776-accd-4637-8d7c-c73fc4767490)

Caso queira ler em detalhes todo o projeto está documentado em detalhes [aqui](https://github.com/sannlin9/Projeto-Credit-Score/blob/main/Desenvolvimento..ipynb).

5. Deploy do modelo: Após o treinamento, ajuste e validação do modelo, procedeu-se à implementação no Streamlit. Foi desenvolvida uma aplicação que recebe novos dados e realiza as previsões do modelo, retornando ao usuário um arquivo Excel.

[streamlit-app_pycaret-2023-05-19-14-05-31.webm](https://github.com/sannlin9/Projeto-Credit-Score/assets/125318548/9ca5b992-8d65-43da-a6cf-75aa6e7628c3)


6. Ao longo de todo o processo, é crucial monitorar as métricas de desempenho do modelo. O objetivo final é desenvolver um modelo de score de crédito confiável e preciso, capaz de tomar decisões embasadas nos dados disponíveis.

##### Quanto aos resultados:

Na base de teste (out-of-time), obtivemos uma precisão de 92%.

![image](https://github.com/sannlin9/Projeto-Credit-Score/assets/125318548/31230734-e90e-4b5d-a9a4-9ff5244b0800)

Algumas outras metricas de desempenho.

###### Curva ROC.
![image](https://github.com/sannlin9/Projeto-Credit-Score/assets/125318548/fd77ccb2-c0f8-4022-a179-f0e54c5fd389)
###### Precision- Recal

![image](https://github.com/sannlin9/Projeto-Credit-Score/assets/125318548/46e931cd-a577-4e27-bfcc-6c0d4076a124)

###### Matrix de confusão.

![image](https://github.com/sannlin9/Projeto-Credit-Score/assets/125318548/1f669b6d-f922-4237-8108-468ce5d33f11)


