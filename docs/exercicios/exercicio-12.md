# Exercícios: Aula 12 - Instalação e CRUD Básico (MongoDB) 🍃

Coloque a mão na massa com o banco de dados orientado a documentos.

---

## 🟢 Nível: Básico

### 1. Preparação
Você já instalou o MongoDB Compass ou Atlas? Tire um print da tela inicial conectada ao banco.

### 2. Inserção Simples
Crie uma coleção chamada `livros` e insira 3 documentos com campos `titulo`, `autor` e `ano`.

---

## 🟡 Nível: Intermediário

### 3. Filtros no Find
Escreva o comando para buscar todos os livros publicados **após o ano 2010**. (Dica: Use `$gt`).

### 4. Atualização de Dados
Houve um erro no cadastro. O autor "Joao" agora se chama "João Silva". Escreva o comando `updateOne` para corrigir apenas este documento.

---

## 🔴 Nível: Desafio

### 5. Manipulação de Arrays (O Poder do NoSQL)
No MongoDB, campos podem ser listas.
1.  Insira um documento na coleção `usuarios`:
    `{ nome: "Carlos", tags: ["Estudante", "Inovador"] }`
2.  Escreva o comando para **adicionar** a tag "SQL" ao array do usuário "Carlos". (Pesquise sobre o operador `$push`).
3.  Como você buscaria todos os usuários que possuem a tag "Inovador"?