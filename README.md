# Análise de Estoque 

Este projeto apresenta uma análise de dados sobre o estoque de uma rede de lojas, utilizando dados de movimentação de produtos. O objetivo principal é fornecer insights valiosos sobre o fluxo de entradas e saídas, estoque atual e a distribuição de produtos por categoria e loja.

## 1. Estrutura dos Dados

A base de dados contém **15.000 linhas** e **7 colunas**, com informações detalhadas sobre produtos, preços, movimentações e lojas. A estrutura da base está organizada da seguinte forma:

| Coluna             | Descrição                                             |
|--------------------|-------------------------------------------------------|
| COD                | Código único do produto                               |
| DESCRIÇÃO          | Descrição do produto                                  |
| CATEGORIA          | Categoria do produto (Roupas, Acessórios, Calçados)   |
| PREÇO UNITÁRIO     | Preço do produto                                      |
| ID LOJA            | Identificação da loja                                 |
| MOVIMENTAÇÃO       | Quantidade movimentada (entrada/saída)               |
| TIPO               | Tipo de movimentação (Entrada, Saída, Devolução)      |

### 2. Tratamento dos Dados

Durante a análise, a coluna **PREÇO UNITÁRIO** foi tratada para corrigir o formato de valores com vírgula, convertendo para tipo numérico.


## 3. Análises Realizadas

### 3.1. Estoque Atual

O estoque atual foi calculado somando todas as movimentações (entradas e saídas):

- **Estoque Atual Total**: **6.661 unidades**.

### 3.2. Estoque por Loja

A distribuição de estoque por loja é a seguinte:

| Loja   | Estoque Total |
|--------|---------------|
| LOJA A | 1.188         |
| LOJA B | 1.736         |
| LOJA C | 1.395         |
| LOJA D | 1.395         |
| LOJA E | 947           |


### 3.3. Estoque por Categoria

A distribuição do estoque por categoria é:

| Categoria   | Estoque Total |
|-------------|---------------|
| Acessórios  | 942           |
| Calçados    | 1.334         |
| Roupas      | 4.385         |

### 3.4. Estoque por Loja e Categoria

A análise detalhada por loja e categoria mostra a seguinte distribuição de estoque:

| Loja   | Categoria   | Estoque |
|--------|-------------|---------|
| LOJA A | Roupas      | 779     |
| LOJA B | Roupas      | 1.079   |
| LOJA C | Roupas      | 1.003   |
| LOJA D | Roupas      | 945     |
| LOJA E | Roupas      | 579     |


### 3.5. Análise do Tipo de Movimentação

A análise dos tipos de movimentação revela o seguinte:

- **Entradas**: 17.662 unidades
- **Saídas**: 14.746 unidades
- **Devoluções**: 1.809 unidades

### 4. Insights e Recomendações

- **Maior Fluxo de Entradas**: A categoria "Roupas" apresenta o maior fluxo de movimentações, tanto em entradas quanto em saídas.
- **Distribuição Desigual**: Algumas lojas, como a **LOJA B**, possuem um estoque significativamente maior, o que pode indicar uma estratégia de reposição diferenciada.
- **Devoluções**: As devoluções representam uma parte significativa das movimentações, sugerindo a necessidade de revisar a política de vendas ou a qualidade dos produtos.

## 5. Conclusão

A análise de estoque permite identificar pontos críticos e otimizar processos, como o controle de entradas e saídas, e também ajustar o estoque de acordo com a demanda das lojas e categorias. A próxima etapa seria implementar um sistema de reposição automática para melhorar a gestão de inventário.


