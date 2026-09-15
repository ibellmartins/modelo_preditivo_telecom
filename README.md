# Previsão de Churn em Telecomunicações com Machine Learning

Projeto desenvolvido no contexto da disciplina de Inteligência Artificial da Faculdade de Computação e Informática (FCI) da Universidade Presbiteriana Mackenzie, no curso de Sistemas de Informação. 

## Integrantes

- Guilherme Soares — RA: 10428380
- Isabella Sofia Martins — RA: 10420398
- Lucas Cesar Kato — RA: 10419319

## Sobre o Projeto

O setor de telecomunicações enfrenta um problema recorrente de evasão de clientes, conhecido como **churn**. Esse fenômeno ocorre quando um assinante encerra ou deixa de utilizar os serviços contratados, provocando perda de receita e reduzindo o retorno sobre os investimentos realizados na aquisição desses clientes.

Este projeto utiliza técnicas de **Machine Learning** para identificar padrões associados ao cancelamento e desenvolver um modelo de classificação capaz de estimar a probabilidade de churn de cada cliente.

A proposta é permitir que empresas de telecomunicações adotem estratégias de retenção mais proativas, direcionando ações de atendimento e relacionamento aos clientes com maior propensão ao cancelamento.

## Objetivo

Desenvolver um modelo preditivo de Inteligência Artificial capaz de identificar antecipadamente clientes com maior probabilidade de cancelar seus serviços de telecomunicações.

Para atingir esse objetivo, o projeto contempla:

- importação, limpeza e preparação dos dados;
- análise exploratória dos dados (*Exploratory Data Analysis — EDA*);
- identificação dos principais fatores relacionados ao churn;
- transformação das variáveis categóricas por meio de **One-Hot Encoding**;
- normalização das variáveis numéricas;
- treinamento de modelos de classificação;
- avaliação do desempenho dos modelos por meio de métricas adequadas para bases desbalanceadas.

## Dataset

O projeto utiliza o dataset público **Telco Customer Churn**, disponibilizado no Kaggle e originalmente desenvolvido pela IBM para demonstração de soluções analíticas.

A base contém **7.043 registros de clientes** e **21 atributos**, incluindo informações relacionadas a:

- características demográficas;
- serviços contratados;
- tipo de contrato;
- forma de pagamento;
- mensalidade;
- tempo de permanência do cliente;
- utilização de serviços adicionais;
- ocorrência ou não de churn.

Durante a preparação dos dados, são realizadas etapas como tratamento de valores inconsistentes, remoção de identificadores sem valor preditivo, transformação de variáveis categóricas e normalização dos dados.

### Fontes do dataset

- [Kaggle — Telco Customer Churn](https://www.kaggle.com/datasets/blastchar/telco-customer-churn)
- [IBM Community — Telco Customer Churn](https://community.ibm.com/community/user/blogs/steven-macko/2019/07/11/telco-customer-churn-1113)

## Tecnologias Utilizadas

- **Linguagem:** Python
- **Manipulação de dados:** Pandas e NumPy
- **Visualização:** Matplotlib e Seaborn
- **Machine Learning:** Scikit-learn
- **Pré-processamento:** One-Hot Encoding e MinMaxScaler

## Modelos de Machine Learning

O projeto utiliza a opção **Framework**, com a biblioteca `scikit-learn`, para desenvolver e avaliar algoritmos clássicos de classificação.

Entre os modelos considerados estão:

- Regressão Logística;
- Árvores de Decisão.

Outros modelos poderão ser avaliados e comparados durante o desenvolvimento do projeto.

## Avaliação dos Modelos

Como o dataset apresenta um desbalanceamento entre clientes que permaneceram e clientes que cancelaram seus serviços, a avaliação não será baseada exclusivamente em **acurácia**.

Entre as métricas consideradas estão:

- Precisão (*Precision*);
- Curva Precision-Recall;
- Coeficiente de Correlação de Matthews (**MCC**);
- Matriz de Confusão.

Também poderão ser utilizadas estratégias como o balanceamento dos pesos das classes para reduzir o impacto do desbalanceamento durante o treinamento.

## Aspectos Éticos

Os dados utilizados neste projeto são públicos e correspondem a um cenário fictício criado para fins educacionais e de demonstração.

Apesar disso, uma eventual aplicação desse tipo de solução em dados reais exige atenção à:

- privacidade das informações dos clientes;
- proteção de dados pessoais;
- transparência das decisões algorítmicas;
- identificação e mitigação de vieses;
- utilização responsável de variáveis demográficas.

O objetivo do modelo é funcionar como uma ferramenta de apoio à tomada de decisão, e não substituir integralmente a análise humana.

## Resultado Esperado

Ao final do projeto, espera-se obter um modelo capaz de identificar clientes com maior propensão ao churn com desempenho superior a uma classificação aleatória.

A solução poderá servir como apoio às equipes de atendimento, marketing e retenção, permitindo direcionar ações aos clientes com maior risco de cancelamento e tornando as estratégias de retenção mais eficientes.
