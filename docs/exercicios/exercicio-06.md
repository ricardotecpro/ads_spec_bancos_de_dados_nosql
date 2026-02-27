# Exercícios: Aula 06 - DQL Básico 💾

Pratique a arte de perguntar ao banco de dados e obter as respostas corretas.

---

## 🟢 Nível: Básico

### 1. Seleção de Colunas
Escreva o comando SELECT para visualizar apenas o **nome** e o **telefone** de todos os clientes cadastrados na tabela `clientes`.

### 2. Filtro de Igualdade
Busque todos os dados do produto que possui o **Código de Barras (EAN)** igual a `7891234567890`.

---

## 🟡 Nível: Intermediário

### 3. Uso de Operadores Relacionais
Escreva uma consulta para listar o nome e o estoque de todos os produtos que possuem **menos de 10 unidades** em estoque, ordenados pela quantidade (do menor para o maior).

### 4. Busca por Padrões (LIKE)
O gerente pediu uma lista de todos os alunos cujo e-mail termina com `@gmail.com`. Como seria esse comando SQL?

---

## 🔴 Nível: Desafio

### 5. Filtragem Composta e Ordenação
Você precisa gerar um relatório de segurança. Escreva um comando para:
1.  Listar `id`, `usuario` e `data_acesso` da tabela `logs`.
2.  Filtrar apenas acessos que ocorreram fora do horário comercial (antes das 08:00 ou depois das 18:00).
3.  Ordenar o resultado da data mais recente para a mais antiga.

*Dica: Use `WHERE hora < '08:00' OR hora > '18:00'`.*