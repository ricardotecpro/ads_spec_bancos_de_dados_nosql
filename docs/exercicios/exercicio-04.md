# Exercícios: Aula 04 - DDL (Criação da Estrutura) 🏗️

Coloque em prática a criação de bancos de dados, tabelas e chaves usando SQL.

---

## 🟢 Nível: Básico

### 1. Criando sua primeira Tabela
Escreva o comando SQL para criar uma tabela chamada `produtos` com as seguintes colunas:
*   `id`: Chave Primária com autoincremento.
*   `nome`: Texto de até 100 caracteres, obrigatório.
*   `preco`: Valor decimal.
*   `quantidade`: Valor inteiro.

### 2. Comandos Fundamentais
Diferencie, em uma frase cada, a função dos comandos:
a) `CREATE DATABASE`
b) `ALTER TABLE`
c) `DROP TABLE`

---

## 🟡 Nível: Intermediário

### 3. Restrições e Chaves Estrangeiras
Escreva o script SQL para criar um relacionamento entre `categorias` e `produtos`:
1.  Crie a tabela `categorias` (id, nome).
2.  Adicione a coluna `categoria_id` na tabela `produtos` (criada no exercício 1) como uma **Chave Estrangeira** que aponta para `categorias`.

### 4. Modificando Estruturas
Você percebeu que esqueceu de guardar o "E-mail" na tabela de `clientes`. Escreva o comando `ALTER TABLE` necessário para adicionar essa coluna com no máximo 150 caracteres.

---

## 🔴 Nível: Desafio

### 5. O Banco da Biblioteca (Script Completo)
Escreva um único script SQL que realize as seguintes tarefas em ordem:
1.  Crie as tabelas `autores` (id, nome, nacionalidade).
2.  Crie a tabela `livros` (id, titulo, ano_publicacao, autor_id).
3.  Garanta que o `autor_id` seja uma FK obrigatória.
4.  Crie um **Índice** para acelerar a busca pelo título do livro.
5.  Adicione uma restrição `CHECK` na tabela livros para que o `ano_publicacao` seja maior que 1500.
