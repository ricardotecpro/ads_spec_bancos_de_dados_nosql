# Exercícios: Aula 14 - Consultas e Agregações no MongoDB 🧪

Aprenda a processar dados e gerar relatórios poderosos no MongoDB.

---

## 🟢 Nível: Básico

### 1. Pipeline Simples
Explique com suas palavras como funciona a ideia de "Pipeline" (Linha de montagem) no MongoDB.

### 2. Etapas de Agregação
Quais os equivalentes no SQL para as seguintes etapas do MongoDB:
a) `$match` ->
b) `$group` ->
c) `$sort` ->
d) `$limit` ->

---

## 🟡 Nível: Intermediário

### 3. Somando Valores
Dada a coleção `vendas` (vendedor, valor, data), escreva o pipeline de agregação para calcular o **valor total vendido por vendedor**.

### 4. O JOIN do NoSQL
Você tem a coleção `posts` e a coleção `autores`. Os posts possuem um campo `autor_id`. Escreva o comando `$lookup` para trazer os dados do autor dentro de cada post.

---

## 🔴 Nível: Desafio

### 5. Análise de Performance
Por que é recomendado que a etapa `$match` seja sempre a primeira do seu pipeline de agregação? O que aconteceria se você colocasse um `$match` após um `$group` que processou milhões de registros?

### 6. Desafio do $unwind
Muitos documentos no MongoDB possuem arrays (listas). Pesquise o que faz o operador `$unwind` e dê um exemplo de uso para um documento de `Pedido` que contém um array de `itens`.