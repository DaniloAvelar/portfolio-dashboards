📊 Dashboard de Vendas, Custo, Margem de Lucro e KPI — Power BI
Projeto desenvolvido como parte de um módulo de capacitação em Business Intelligence com Power BI, com foco em modelagem de dados, criação de métricas com DAX e construção de dashboards interativos.

🎯 Objetivo
Analisar o desempenho de vendas de uma empresa global, explorando métricas de valor de venda, custo de envio, lucro e margem de lucro segmentadas por categoria de produto, mercado, modo de envio e período de tempo.

🗂️ Fonte de Dados
Os dados foram fornecidos em 4 arquivos CSV, importados e modelados diretamente no Power BI Desktop:
TabelaDescriçãoClientesInformações cadastrais: cidade, estado, país, região, mercado e segmentoPedidosDados dos pedidos: datas, modo de envio e prioridadeProdutosCatálogo de produtos: categoria, subcategoria e nomeVendasTabela fato com valor de venda, custo de envio, quantidade vendida e chaves de relacionamento

🔗 Modelagem de Dados
O modelo segue o padrão Star Schema, com a tabela Vendas como tabela fato central e as demais como tabelas dimensão:

Clientes → Vendas (1 para *)
Pedidos → Vendas (1 para *)
Produtos → Vendas (1 para *)

Os relacionamentos foram criados manualmente na visão de modelo do Power BI.

🧮 Métricas Criadas (DAX)
Duas colunas calculadas foram criadas na tabela Vendas:

Lucro — Diferença entre o valor de venda e os custos
MargemLucro — Percentual de lucro sobre o valor de venda


📈 Dashboard
O dashboard "Vendas, Custo, Margem de Lucro e KPI" é composto pelos seguintes visuais:
VisualDescrição🔽 Painel de FiltrosFiltro por Ano/Mês e por Categoria de Produto📉 Gráfico de LinhaComportamento da Margem de Lucro ao longo do tempo (2011–2014)📊 Gráfico de CascataSoma de Valor de Venda por Modo de Envio🔘 Medidor (Gauge)Média de Valor de Venda com meta definida🟦 Mapa de Árvore (Treemap)Média de Custo de Envio por Mercado🍩 Gráfico de RoscaMédia de Lucro por Categoria de Produto
Principais Insights

Tecnologia lidera em lucro médio, representando 46,55% do total entre as categorias
APAC possui o maior custo médio de envio entre os mercados globais
A margem de lucro se manteve estável entre 88,5% e 89,5% ao longo dos anos analisados
O Modo de Envio Classe Padrão concentra o maior volume de vendas


🛠️ Tecnologias Utilizadas

Power BI Desktop
DAX (Data Analysis Expressions)
Modelagem Star Schema


👤 Autor
Danilo Aliotto Avelar
