# Projeto 14: Relatórios Analíticos no MongoDB 🧪

**Objetivo**: Utilizar o Aggregation Framework para gerar inteligência de negócio a partir de dados brutos.

---

## 📝 O Desafio
Você tem uma coleção de `vendas` com os campos: `cliente`, `produto`, `quantidade`, `valor_unitario`, `categoria` e `data`.

## 🚀 Tarefas
Crie os pipelines de agregação para responder:
1.  **Faturamento por Categoria**: Qual o valor total vendido em cada categoria de produtos?
2.  **Ticket Médio**: Qual a média de valor gasto pelos clientes em suas compras?
3.  **Top 3 Vendedores**: Quais são os 3 vendedores que mais faturaram? (Supondo que haja um campo `vendedor`).
4.  **Clientes Inativos (Desafio)**: Utilize o `$lookup` para comparar a coleção de `clientes` com a de `vendas` e encontrar quem nunca comprou nada.

## ✅ Critérios de Entrega
*   O script `.js` com os pipelines comentados.
*   Uso de pelo menos 4 estágios diferentes (`$match`, `$group`, `$sort`, `$project`).
*   Screenshot dos resultados no MongoDB Compass.