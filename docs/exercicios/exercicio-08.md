# Exercícios: Aula 08 - JOINs: Junções entre Tabelas 🔗

Pratique a união de dados vindos de múltiplas tabelas.

---

## 🟢 Nível: Básico

### 1. Meu Primeiro JOIN
Dada a tabela `pedidos` (id, data, cliente_id) e `clientes` (id, nome), escreva o SQL para listar o **ID do pedido** e o **Nome do cliente** usando um `INNER JOIN`.

### 2. Entendendo o LEFT JOIN
Qual o resultado da consulta abaixo?
`SELECT p.nome, c.cor FROM produtos p LEFT JOIN cores c ON p.id_cor = c.id;`
O que acontecerá se um produto não tiver uma cor cadastrada no banco?

---

## 🟡 Intermediário

### 3. JOIN com Filtro
Liste o nome dos alunos e o nome dos cursos em que eles estão matriculados, mas apenas para o curso de **"Informática"**.

### 4. Relatório de Inatividade
Você precisa descobrir quais **fornecedores** nunca nos venderam nada. Escreva uma consulta usando `LEFT JOIN` entre `fornecedores` e `compras` e filtre os resultados onde a compra é `NULL`.

---

## 🔴 Nível: Desafio

### 5. O Grande Relatório (Multi-JOIN)
Escreva um script SQL para unir 4 tabelas e exibir os seguintes campos:
*   Nome do Cliente (`clientes`)
*   Data do Pedido (`pedidos`)
*   Nome do Produto (`produtos`)
*   Nome da Categoria do Produto (`categorias`)

**Regra**: Use apelidos para as tabelas (ex: `FROM clientes c`) para deixar o código mais limpo.