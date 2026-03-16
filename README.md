\# Análise de Performance Comercial com Excel



\## Sobre o projeto



Este projeto tem como objetivo identificar quais variáveis possuem maior relação com a performance comercial, utilizando técnicas de análise exploratória e estatística no Excel.



\## Dataset



O conjunto de dados utilizado neste projeto contém informações sobre transações de vendas realizadas em diferentes cidades.

Cada registro representa uma venda e inclui variáveis como:



\- Data da venda

\- Cidade

\- Linha de produto

\- Quantidade de itens vendidos

\- Receita total da venda

\- Forma de pagamento



O dataset contém 1000 registros de vendas realizados entre janeiro e dezembro de 2023.

Esses dados foram utilizados para analisar padrões de receita, ticket médio e volume de vendas, permitindo identificar fatores relacionados à performance comercial.



\## Ferramentas utilizadas



A análise foi conduzida utilizando:



\-Microsoft Excel

\-Tabelas Dinâmicas

\-Agrupamento

\-Fórmulas Avançadas

\-Cálculo manual de Weight of Evidence (WOE)

\-Cálculo manual de Information Value (IV)

\-Dashboard

\-Estruturação Analítica de Dados



\##Análise dos Resultados



1. Quantidade — IV = 0,75



A variável Quantidade apresentou Information Value muito alto, indicando forte capacidade preditiva em relação ao evento analisado.

Interpretação analítica

A quantidade de produtos adquiridos é o fator que mais explica o comportamento observado na base, sugerindo que clientes com padrões diferentes de volume de compra apresentam perfis distintos em relação ao evento analisado.

Observação técnica importante:

Valores de IV muito altos (>0,5) às vezes podem indicar erros de dados e ruídos de ajustes



2\. Linha de Produto — IV = 0,01



A variável Linha de Produto apresentou Information Value muito baixo.

Isso indica que:

a categoria do produto não possui poder significativo para explicar o evento analisado.

Interpretação analítica

As diferentes categorias de produtos apresentam comportamento semelhante em relação ao evento analisado, indicando que a escolha do tipo de produto não influencia significativamente o resultado do modelo.



3\. Forma de Pagamento — IV = 0,00



A variável Forma de Pagamento apresentou Information Value praticamente nulo.

Isso indica que:

não há relação estatística relevante entre a forma de pagamento e o evento analisado.

Interpretação

Clientes que pagam com: dinheiro, cartão e carteira digital, apresentam comportamento semelhante em relação ao evento estudado.



4\. Cidades - IV = 0,00



Poder preditivo muito fraco

Interpretação analítica

Esse resultado indica que a variável cidade provavelmente possui poder preditivo muito baixo ou inexistente, 



5\. Avaliação (rating) — IV = 0,00



A variável Avaliação (rating) também apresentou ausência de poder preditivo.

Isso indica que:

A avaliação do cliente não está associada ao evento modelado dentro dessa base.

Interpretação

O nível de satisfação do cliente, medido pela avaliação, não apresenta relação estatística significativa com o comportamento analisado.



Conclusão Geral



A análise de Information Value mostrou que:

Quantidade é a única variável com alto poder preditivo, apresentando forte capacidade de discriminação entre os grupos analisados.

As variáveis Linha de Produto, Forma de Pagamento, Cidade e Avaliação apresentam baixo ou nenhum poder explicativo, indicando a necessidade de incluir novas variáveis para aprofundar a análise.

De forma geral, os resultados indicam que o volume de compra é o principal fator associado ao evento analisado, enquanto as demais variáveis possuem pouca relevância preditiva dentro da base.



\## Dashboard

## Dashboard

![Dashboard](images/Dashboard_vendas.png)


\## Principais Insights


Insight 1 — Distribuição geográfica equilibrada

As três cidades analisadas apresentam níveis semelhantes de faturamento, com leve destaque para Naypyitaw.

Isso indica distribuição equilibrada da demanda.



Insight 2 — Mix de produtos balanceado



As categorias apresentam receitas próximas, sugerindo um portfólio bem distribuído, sem dependência de um único produto.



Insight 3 — Diferença entre volume e ticket médio

Algumas categorias apresentam maior volume de vendas, enquanto outras possuem ticket médio mais elevado.

Isso indica dois perfis de produto:

produtos de alto giro

produtos de maior valor agregado



Insight 4 — Baixo poder preditivo das variáveis sobre satisfação

A análise de Information Value mostrou que as variáveis disponíveis possuem baixo poder explicativo sobre o rating dos clientes, sugerindo que fatores adicionais podem influenciar a satisfação.





\## Estrutura do projeto

sales-performance-analysis

│

├── data

├── images

├── dashboard

└── README.md

