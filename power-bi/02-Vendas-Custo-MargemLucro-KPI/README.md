# 📊 Dashboard de Vendas, Custo, Margem de Lucro e KPI
### Business Intelligence com Power BI

Bem-vindo(a) ao repositório deste projeto de análise de dados desenvolvido em **Power BI Desktop**.
O objetivo é demonstrar habilidades em **modelagem de dados (Star Schema)**, criação de **métricas com DAX** e construção de **dashboards interativos** com foco em análise de vendas globais.

---

## 🎯 Objetivo do Projeto

Analisar o desempenho comercial de uma empresa global, explorando métricas de **valor de venda, custo de envio, lucro e margem de lucro**, segmentadas por:

* Categoria de produto
* Mercado geográfico
* Modo de envio
* Período de tempo

---

## 🛠️ Tecnologias e Ferramentas Utilizadas

* **Ferramenta de BI:** Power BI Desktop
* **Linguagem de Métricas:** DAX (Data Analysis Expressions)
* **Modelagem:** Star Schema
* **Fonte de Dados:** Arquivos CSV

---

## 🗂️ Fonte de Dados

Os dados foram fornecidos em **4 arquivos CSV**, importados e modelados diretamente no Power BI Desktop:

| Tabela | Descrição |
| :--- | :--- |
| `Clientes` | Informações cadastrais: cidade, estado, país, região, mercado e segmento |
| `Pedidos` | Dados dos pedidos: datas, modo de envio e prioridade |
| `Produtos` | Catálogo de produtos: categoria, subcategoria e nome |
| `Vendas` | Tabela fato com valor de venda, custo de envio, quantidade vendida e chaves de relacionamento |

---

## 🔗 Modelagem de Dados — Star Schema

O modelo segue o padrão **Star Schema**, com a tabela `Vendas` como **tabela fato** central e as demais como **tabelas dimensão**.
Os relacionamentos foram criados manualmente na visão de modelo do Power BI:

```
Clientes  ──(1)──────(*) ──┐
Pedidos   ──(1)──────(*) ──┤── Vendas (Fato)
Produtos  ──(1)──────(*) ──┘
```

---

## 🧮 Métricas Criadas com DAX

Duas colunas calculadas foram desenvolvidas diretamente na tabela `Vendas`:

| Métrica | Descrição |
| :--- | :--- |
| `Lucro` | Diferença entre o valor de venda e os custos |
| `MargemLucro` | Percentual de lucro sobre o valor de venda |

---

## 📈 Visão Geral do Dashboard

> **"Vendas, Custo, Margem de Lucro e KPI"**

O dashboard é composto pelos seguintes visuais interativos:

| Visual | Descrição |
| :--- | :--- |
| 🔽 **Painel de Filtros** | Filtro por Ano/Mês e por Categoria de Produto |
| 📉 **Gráfico de Linha** | Comportamento da Margem de Lucro ao longo do tempo (2011–2014) |
| 📊 **Gráfico de Cascata** | Soma de Valor de Venda por Modo de Envio |
| 🔘 **Medidor (Gauge)** | Média de Valor de Venda com meta definida (500) |
| 🟦 **Mapa de Árvore (Treemap)** | Média de Custo de Envio segmentada por Mercado |
| 🍩 **Gráfico de Rosca** | Média de Lucro distribuída por Categoria de Produto |

---

## 🚀 Principais Insights

* 🥇 **Tecnologia** lidera em lucro médio, representando **46,55%** do total entre as categorias
* 🌏 **APAC** possui o maior custo médio de envio entre os mercados globais (**29,14**)
* 📐 A margem de lucro manteve-se estável entre **88,5% e 89,5%** ao longo de todo o período analisado
* 📦 O **Modo de Envio Classe Padrão** concentra o maior volume de vendas acumulado

---

## 👤 Autor

**Danilo Aliotto Avelar**

---

## 📧 Contato

Se tiver alguma dúvida, feedback ou oportunidade de projeto, sinta-se à vontade para me acionar:

* **LinkedIn:** [Danilo Aliotto Avelar](https://www.linkedin.com/in/danilo-a-avelar/)
