# Exercícios: Aula 07 - Consultas Avançadas e Agregações 🧪

Pratique a geração de estatísticas e relatórios complexos.

---

## 🟢 Nível: Básico

### 1. Estatística Simples
Escreva uma consulta para encontrar a **média de preços** de todos os produtos na tabela `produtos`. Use um apelido (AS) para que a coluna se chame `media_precos`.

### 2. Contagem de Registros
Quantos clientes estão cadastrados que moram na cidade de `Rio de Janeiro`? Use o comando SQL correspondente.

---

## 🟡 Nível: Intermediário

### 3. Agrupamento por Categoria
Escreva o comando SQL que mostre o nome da **categoria** e o **valor total em estoque** (preço * quantidade) para cada categoria, ordenado do maior para o menor valor.

### 4. Filtro em Grupos
Liste todas as cidades que possuem **mais de 100 clientes** cadastrados. Use o `GROUP BY` e o `HAVING`.

---

## 🔴 Nível: Desafio

### 5. Relatório Gerencial
Você precisa descobrir quais vendedores bateram a meta de R$ 10.000,00 em vendas no mês de Outubro.
1.  Utilize a tabela `vendas` (vendedor_id, data, valor).
2.  Filtre pela data (Outubro/2024).
3.  Agrupe pelo `vendedor_id`.
4.  Mostre apenas quem vendeu acima de 10.000.
5.  Ordene o ranking do melhor vendedor para o pior.