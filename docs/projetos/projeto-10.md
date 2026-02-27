# Projeto 10: Sistema Relacional Parcial 🔐

**Objetivo**: Construir do zero um ecossistema de banco de dados para um E-commerce, aplicando todos os comandos SQL aprendidos até aqui.

---

## 📝 O Grande Desafio: TechStore v1.0
Você recebeu a missão de criar o backend (BD) da TechStore. O sistema deve ser robusto, normalizado e rápido.

## 🚀 Etapas do Projeto

### 1. Modelagem e Criação (DDL)
*   Crie as tabelas: `categorias`, `produtos`, `clientes`, `pedidos` e `itens_pedido`.
*   Defina as chaves e os relacionamentos.
*   Crie uma restrição que impeça o estoque de ser negativo.
*   Crie um índice na coluna `nome` da tabela `produtos`.

### 2. Povoamento (DML)
*   Insira pelo menos 3 categorias (Ex: Smartphones, Laptops, Acessórios).
*   Insira 10 produtos variados.
*   Cadastre 5 clientes.

### 3. Simulando uma Venda (Transação)
*   Crie um script que:
    1. Abre uma transação.
    2. Registra um pedido para um cliente.
    3. Adiciona 2 itens a esse pedido.
    4. Atualiza o estoque desses 2 produtos.
    5. Finaliza com `COMMIT`.

### 4. Relatórios de Gestão (DQL)
*   Crie uma consulta que mostre: `Nome do Cliente`, `Data do Pedido` e `Valor Total do Pedido`. (Dica: Use JOIN e SUM).
*   Crie um ranking das categorias que mais possuem produtos cadastrados.

## ✅ Critérios de Entrega
*   Um arquivo `techstore_completo.sql` com todos os comandos comentados.
*   Diagrama E-R gerado pelo pgAdmin ou Mermaid.
*   Print do resultado do relatório de faturamento por cliente.