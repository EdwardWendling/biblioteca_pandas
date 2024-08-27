# biblioteca_pandas

# Algumas métricas e KPIs foram solicitados pela loja de varejo para serem calculados ​​a partir da união das bases de vendas e clientes:
Departamentos Mais Vendidos
Podemos agrupar as vendas por departamento (categoria) e somar a receita de vendas de cada um para descobrir quais são os departamentos que geram mais receita para a loja.
Esse KPI serve para avaliar o desempenho de cada departamento e definir estratégias por categoria de produto.
1. Média de Preço e Frete por Departamento
Similar ao KPI anterior, podemos calcular a média de preço e frete para cada departamento, para entender a precificação e custo de entrega por categoria de produto.
Isso ajuda a moldar estratégias de preços e frete por tipo de produto.
2. Vendas por Mês
Um KPI simples mas essencial é a evolução das vendas por mês, para entender sazonalidades e comparar desempenho mensal ao longo do tempo.
Isso permite projetar vendas, metas e orçamentos mensais.
3. Média de Renda por Canal de Venda
Podemos unir os canais de venda (e-commerce, lojas físicas, televendas) com a renda média dos clientes para analisar o perfil de cada canal.
Isso ajuda a caracterizar a persona de cada canal para direcionar estratégias de marketing.
4. Média de Idade por Bandeira
As bandeiras de cartão (Visa, Mastercard, Elo etc.) podem segmentar tipos de cliente. Podemos calcular a idade média por bandeira para confirmar se esse padrão se repete.
Caso sim, isso permite personalizar comunicação e ofertas por bandeira de cartão.
Além dos KPIs solicitados, algumas premissas e regras do negócio foram passadas para tratamento na análise de dados:
Erro no Sistema para Estado Civil
Foi identificado um erro no sistema onde, para vendas sem informação de estado (UF), o estado está sendo preenchido automaticamente como Mato Grosso do Sul.
Essa premissa deve ser considerada na análise, tratando vendas sem UF como MT para não distorcer resultados regionais.
Validador de Preço x Frete
Outra premissa é que o preço não pode ser maior do que o preço + frete, pois isso geraria prejuízo nas vendas.
Devemos criar uma rotina de validação nos dados para identificar e tratar essas ocorrências onde preço > preço + frete.


