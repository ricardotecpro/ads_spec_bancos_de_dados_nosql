# Exercícios: Aula 03 - Normalização e Estrutura Relacional 📡

Pratique a organização de tabelas seguindo as regras de normalização.

---

## 🟢 Nível: Básico

### 1. Tipos de Dados Corretos
Escolha o melhor tipo de dado (PostgreSQL) para armazenar as seguintes informações:
a) Preço de um produto (ex: R$ 49,90).
b) Texto longo de uma postagem de blog.
c) Quantidade de itens em estoque (número inteiro).
d) Data e hora exata de um acesso ao sistema.
e) Status de entrega (V ou F).

### 2. O Conceito de NULL
Explique a frase: "NULL não é zero, nem um espaço vazio". Por que o uso indiscriminado de colunas que aceitam NULL pode ser ruim para o banco?

---

## 🟡 Nível: Intermediário

### 3. Aplicando a 1ª Forma Normal (1FN)
A tabela abaixo está violando a 1FN. Como você a reestruturaria?
**Tabela: Projetos**
| ID_Proj | Nome_Projeto | Equipe_Membros (Lista de nomes) |
|---|---|---|
| 1 | App Mobile | João, Maria, Pedro |
| 2 | Site Web | Ana, José |

### 4. Entendendo a 3ª Forma Normal (3FN)
Observe a tabela: `Carros (ID_Carro, Placa, Modelo, Marca_Nome, Marca_Pais)`.
Por que ela viola a 3FN? Quais tabelas novas você criaria para normalizá-la?

---

## 🔴 Nível: Desafio

### 5. Caso Real: Sistema de Pedidos Mal Estruturado
Você recebeu uma planilha de Excel para importar para o banco, mas ela está "achatada" (flat):
`Planilha: Pedido_ID, Data, Cliente_ID, Cliente_Nome, Cliente_Email, Item_Nome, Item_Qtd, Item_Preco_Unitario`.

**Sua tarefa:**
1.  Identifique as repetições de dados.
2.  Projete o esquema normalizado (mínimo 3 tabelas).
3.  Indique as Chaves Primárias (PK) e Estrangeiras (FK).
