# Exercícios: Aula 02 - Modelagem de Dados e Modelo E-R 🏗️

Aplique os conceitos de entidades, atributos, relacionamentos e chaves.

---

## 🟢 Nível: Básico

### 1. Identificando Chaves Primárias
Para as tabelas abaixo, identifique qual atributo seria a melhor escolha para ser a **Chave Primária (PK)** e justifique:
a) **Carros**: Placa, Modelo, Ano, Cor.
b) **Alunos**: Nome, Data de Nascimento, CPF, Nota.
c) **Produtos**: Nome do Produto, Código de Barras (EAN), Preço.

### 2. Conceitos Rápidos
Defina brevemente:
a) Entidade.
b) Chave Estrangeira (FK).
c) Cardinalidade 1:N.

---

## 🟡 Nível: Intermediário

### 3. Definindo Cardinalidades
Determine a cardinalidade (1:1, 1:N ou N:N) para os seguintes relacionamentos reais:
a) **Estado** e **Cidade**.
b) **Pessoa** e **CPF**.
c) **Professor** e **Turma**.
d) **Pedido** e **Produto**.

### 4. Integridade Referencial na Prática
Imagine que você tem a tabela `Autores` (PK: `id_autor`) e a tabela `Livros` (FK: `id_autor`). O que acontece com os livros se você tentar excluir um autor que possui 10 livros cadastrados? Por que o SGBD faz isso?

---

## 🔴 Nível: Desafio

### 5. Mini Modelagem: Sistema de Petshop
Crie um esboço (pode ser em texto ou lista) para um sistema de Petshop que precisa armazenar:
*   **Donos** (clientes).
*   **Pets** (um cliente pode ter vários pets, mas cada pet pertence a um único dono).
*   **Serviços** (Banho, Tosa, Consulta - um pet pode fazer vários serviços ao longo do tempo).

**O que você deve entregar:**
1.  Lista de Entidades e seus Atributos.
2.  Indicação de PKs e FKs.
3.  A cardinalidade entre as entidades.
