# Exercícios: Aula 09 - Transações e Integridade ACID 🔑

Aprenda a proteger seus dados contra falhas e inconsistências.

---

## 🟢 Nível: Básico

### 1. Conceito Fundamental
O que é uma transação de banco de dados? Dê um exemplo do dia a dia (fora do banco) que funcione como "Tudo ou Nada".

### 2. Comandos de Controle
Explique a diferença entre:
a) `BEGIN`
b) `COMMIT`
c) `ROLLBACK`

---

## 🟡 Nível: Intermediário

### 3. A Propriedade Atomicidade (A do ACID)
Em um sistema de reserva de assentos de cinema, por que a atomicidade é vital quando o usuário escolhe o lugar e realiza o pagamento?

### 4. Simulação de Problema
Imagine que você abriu um `BEGIN`, deletou acidentalmente 1.000 linhas da tabela de `clientes` e, antes de dar o `COMMIT`, a sua internet caiu e o pgAdmin fechou. O que acontecerá com esses dados? Por quê?

---

## 🔴 Nível: Desafio

### 5. Transferência de Saldo (Código SQL)
Escreva o script SQL completo para realizar a transferência de R$ 250,00 da conta do `Cliente A` para o `Cliente B`.
*   O script deve garantir que o Cliente A possui saldo suficiente antes de tirar (usando lógica hipotética ou apenas o comando).
*   Se houver um erro simulado no meio do processo, o que você deve fazer?
*   Inclua os comandos de início, alteração e finalização.