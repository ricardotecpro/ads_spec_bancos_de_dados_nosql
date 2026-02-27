# Exercícios: Aula 11 - Introdução ao NoSQL e MongoDB 🌐

Explore os conceitos fundamentais que diferenciam o NoSQL dos bancos tradicionais.

---

## 🟢 Nível: Básico

### 1. Definição NoSQL
O que significa o termo NoSQL? É correto dizer que bancos NoSQL não aceitam comandos SQL? Explique.

### 2. Identificação de Tipos
Associe o banco de dados à sua categoria NoSQL:
a) **MongoDB** -> ( ) Grafo
b) **Redis** -> ( ) Colunar
c) **Neo4j** -> ( ) Documento
d) **Cassandra** -> ( ) Chave-Valor

---

## 🟡 Nível: Intermediário

### 3. SQL vs NoSQL (Cenários)
Para os cenários abaixo, qual modelo você escolheria e por quê?
a) Um sistema bancário de transferências financeiras críticas.
b) Um sistema de logs de sensores de IoT que gera milhões de registros por segundo.
c) Um catálogo de e-commerce onde os produtos mudam de atributos constantemente (ex: um tênis tem "tamanho", mas um computador tem "processador").

### 4. Entendendo Documentos (JSON)
Escreva um pequeno documento JSON que represente um **Livro**, contendo: `titulo`, `autor` (objeto com nome e país), `ano` e uma lista de `categorias`.

---

## 🔴 Nível: Desafio

### 5. O Teorema CAP
Explique, com suas palavras, por que é impossível garantir **C**onsistência, **A**vailabilidade e **P**artição ao mesmo tempo em um sistema distribuído. Se um cabo de rede for cortado separando os servidores (Partição), o que o administrador deve priorizar?