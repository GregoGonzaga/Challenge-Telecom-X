📊 Challenge 2 — Telecom X: Análise de Churn de Clientes
📌 Introdução
Este projeto apresenta uma análise detalhada sobre evasão de clientes (Churn) em uma empresa de telecomunicações fictícia, a Telecom X.
O objetivo é identificar os principais fatores que levam clientes a cancelar seus serviços, propondo insights e estratégias para retenção.

🧹 Limpeza e Tratamento de Dados
Normalização

As colunas aninhadas (customer, phone, internet, account) foram transformadas em uma estrutura tabular única.

Tratamento de Inconsistências

Valores como "" e "No internet service" foram padronizados para evitar distorções.

Remoção de Nulos

Linhas com valores ausentes na coluna Churn foram excluídas, resultando em 7.043 registros finais.

Conversão de Tipos

A coluna Charges.Total foi convertida de string para numérico.

Nova Feature

Criada a variável Charges.Daily = (Charges.Monthly ÷ tempo de permanência).

Codificação de Variáveis

Variáveis categóricas transformadas via One-Hot Encoding para permitir análises e uso em modelos de machine learning.

📈 Análise Exploratória de Dados (AED)
Análise Descritiva

Cálculo de média, mediana e desvio padrão para variáveis numéricas.

Distribuição do Churn

Gráficos de contagem mostram desequilíbrio entre clientes que evadiram e os que permaneceram.

Boxplots de Variáveis Numéricas

Clientes que cancelam serviços tendem a ter menores valores de Charges.Monthly e Charges.Daily.

Análise de Variáveis Categóricas

Clientes com contratos "Month-to-month" e pagamento via "Electronic check" apresentam maior probabilidade de churn.

🛠️ Tecnologias Utilizadas
Python

Pandas (manipulação e limpeza de dados)

Matplotlib / Seaborn (visualizações)

NumPy (operações numéricas)

📂 Estrutura do Projeto
bash
Copiar
Editar
├── data/               # Base de dados bruta e tratada
├── notebooks/          # Análises e scripts em Jupyter Notebook
├── images/             # Gráficos e visualizações
└── README.md           # Documentação do projeto
📢 Conclusões
Contratos curtos e pagamentos via métodos menos automáticos estão associados a maior evasão.

Clientes com custos mensais menores também apresentam maior risco de churn.

Estratégias de fidelização e benefícios para contratos anuais podem reduzir o churn.

📬 Contato    
Autor: Gregorio Tomas da Silva Gonzaga
LinkedIn: https://www.linkedin.com/in/gregorio-tomas-gonzaga-86614077/
E-mail: gregorio.gonzaga@outlook.com
