# Exercícios: Aula 10 - Projeto Parcial 🔐

Finalize o Módulo II testando sua capacidade de integração.

---

## 🟢 Nível: Básico

### 1. Revisão de Conceitos
Explique em um parágrafo como o DDL e o DML trabalham juntos em um projeto de software.

### 2. Identificação de Erros
Observe o script abaixo e aponte pelo menos 2 erros de integridade ou lógica:
```sql
CREATE TABLE vendas (
    id INT,
    produto VARCHAR(50),
    preco DECIMAL,
    data DATE
);
INSERT INTO vendas VALUES (1, 'Celular', -100, '2024-01-01');
```

---

## 🟡 Nível: Intermediário

### 3. DQL de Auditoria
Escreva uma consulta que retorne o nome do cliente e a quantidade total de pedidos que ele já fez, mas exiba apenas os clientes que fizeram **zero** pedidos. (Dica: Use `LEFT JOIN` e `COUNT`).

### 4. Transação de Cancelamento
Escreva o bloco de comandos (`BEGIN`...`COMMIT`) para cancelar um pedido:
1.  Apagar o registro em `itens_pedido`.
2.  Apagar o registro em `pedidos`.
3.  O que acontece se você inverter a ordem e tentar apagar o pedido antes dos itens?

---

## 🔴 Nível: Desafio

### 5. O Desafio do DBA
Você foi solicitado a otimizar um banco que está lento.
1.  Cite 3 colunas que obrigatoriamente deveriam ter **Índices**.
2.  Escreva a consulta para mostrar o faturamento total por categoria, ordenado do maior para o menor.
3.  Escreva uma restrição `CHECK` para garantir que a data de entrega nunca seja anterior à data do pedido.