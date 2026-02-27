# Projeto 08: Consultas Multi-tabelas (JOINs) 🚢

**Objetivo**: Relacionar dados de diferentes partes do banco para gerar relatórios consolidados.

---

## 📝 O Desafio
Você precisa criar o relatório de fechamento de um sistema de E-commerce. O banco possui as tabelas: `clientes`, `pedidos` e `vendedores`.

## 🚀 Tarefas
Escreva o script SQL que resolva:
1.  **Relatório de Pedidos**: Listar o ID do pedido, a data e o **Nome do Cliente** que fez a compra.
2.  **Lista de Vendedores Ativos**: Listar o nome de todos os vendedores e o ID dos pedidos que eles realizaram (mesmo que um vendedor ainda não tenha feito nenhuma venda).
3.  **Relatório Completo**: Unir Clientes e Pedidos para mostrar apenas quem já comprou pelo menos uma vez.
4.  **Clientes Sem Pedidos**: Descobrir o nome dos clientes que ainda não realizaram nenhuma compra (Dica: Use `LEFT JOIN` e `WHERE ... IS NULL`).

## ✅ Critérios de Entrega
*   Uso de aliases (`AS`) para as tabelas.
*   Script `.sql` limpo e comentado.
*   Screenshot dos resultados no pgAdmin.