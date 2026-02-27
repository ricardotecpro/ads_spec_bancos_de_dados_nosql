# Exercícios: Aula 05 - DML (Manipulação de Dados) ⚙️

Pratique os comandos de inserção, atualização e exclusão de dados.

---

## 🟢 Nível: Básico

### 1. Inserção Simples
Escreva o comando SQL para inserir um novo registro na tabela `clientes` com os seguintes dados:
*   Nome: `Carlos Eduardo`
*   CPF: `123.456.789-00`
*   Cidade: `São Paulo`

### 2. Inserção Múltipla
Você recebeu uma lista de 3 novos produtos para cadastrar. Escreva um **único comando INSERT** para adicionar:
*   `Mouse Sem Fio` - R$ 89,00 - Estoque: 50
*   `Teclado Mecânico` - R$ 250,00 - Estoque: 20
*   `Monitor 24"` - R$ 900,00 - Estoque: 10

---

## 🟡 Nível: Intermediário

### 3. Atualização Segura
Escreva o comando para atualizar o preço de todos os produtos da categoria `Eletrônicos` (ID 5) em **5% de aumento**.
*Dica: Use `preco = preco * 1.05`.*

### 4. O Perigo do DELETE
Explique o que aconteceria com os dados se você executasse o comando `DELETE FROM usuarios;` por engano. Qual a importância do `Backup` e da cláusula `WHERE` nesse contexto?

---

## 🔴 Nível: Desafio

### 5. Manutenção de Dados Complexa
Imagine que um cliente mudou de cidade e todos os seus pedidos pendentes devem ser atualizados com uma nova "Taxa de Entrega".
1.  Escreva o comando para mudar a cidade do cliente `João Silva` para `Curitiba`.
2.  Escreva o comando para aumentar em R$ 15,00 o `valor_total` de todos os pedidos do cliente `João Silva` que ainda não foram entregues (`status = 'Pendente'`).