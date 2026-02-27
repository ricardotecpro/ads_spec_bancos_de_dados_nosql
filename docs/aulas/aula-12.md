# Aula 12 - Instalação e CRUD Básico no MongoDB 🍃

!!! tip "Objetivo"
    **Objetivo**: Instalar o ambiente de desenvolvimento do MongoDB e dominar as quatro operações básicas (Create, Read, Update, Delete) através do terminal e de ferramentas visuais.

---

## 1. Preparando o Ambiente 🛠️

Você tem duas opções principais:
1.  **MongoDB local**: Instalado na sua máquina (vimos no Setup 02).
2.  **MongoDB Atlas**: Banco de dados na nuvem (DBaaS), gratuito para testes.

Para esta aula, usaremos o **mongosh** (MongoDB Shell) ou o **MongoDB Compass** (Interface Visual).

---

## 2. O Vocabulário MongoDB 🗣️

| SQL | MongoDB |
| :--- | :--- |
| Database | Database |
| Table | Collection |
| Row | Document |
| Column | Field |
| Join | Embedding / Reference |

---

## 3. Operações de Escrita (Create) ✍️

Diferente do SQL, não precisamos criar as colunas antes. O banco cria a coleção na primeira inserção.

```javascript
// Inserir um único documento
db.usuarios.insertOne({
  nome: "Ricardo",
  email: "ricardo@email.com",
  ativo: true
});

// Inserir vários
db.usuarios.insertMany([
  { nome: "Ana", idade: 25 },
  { nome: "Bia", idade: 30 }
]);
```

---

## 4. Operações de Busca (Read) 🔎

O `find()` é o nosso SELECT.

```javascript
// Buscar todos
db.usuarios.find();

// Buscar com filtro (nome igual a Ricardo)
db.usuarios.find({ nome: "Ricardo" });

// Buscar maiores de 20 anos ($gt = Greater Than)
db.usuarios.find({ idade: { $gt: 20 } });
```

---

## 5. Atualização (Update) 🔄

Sempre usamos operadores como o `$set`.

```javascript
// Mudar o nome do usuário com ID específico
db.usuarios.updateOne(
  { _id: ObjectId("...") }, 
  { $set: { nome: "Ricardo Pires" } }
);

// Adicionar um campo a todos os usuários
db.usuarios.updateMany({}, { $set: { verificado: false } });
```

---

## 6. Exclusão (Delete) 🗑️

Cuidado: assim como no SQL, o filtro é essencial!

```javascript
// Deletar um
db.usuarios.deleteOne({ nome: "Ana" });

// Limpar a coleção
db.usuarios.deleteMany({});
```

---

## 7. Prática: O Terminal do Futuro 💻

Abra o seu terminal e execute os comandos:

```termynal
$ mongosh
$ use meu_primeiro_banco;
$ db.produtos.insertOne({ nome: "Mouse", preco: 50 });
$ db.produtos.find();
```

---

## 8. Exercícios de Fixação 🧠

1.  No MongoDB, qual a diferença entre `insertOne` e `insertMany`?
2.  Para que serve o operador `$set` no comando de update? O que aconteceria se você não o usasse no MongoDB? (Dica: Substituição total).
3.  Como você buscaria produtos com preço entre 100 e 500 no MongoDB?

---

**Próxima Aula**: Vamos aprender as estratégias para organizar seus dados com a [Modelagem de Documentos](../aulas/aula-13.md)! 🏗️