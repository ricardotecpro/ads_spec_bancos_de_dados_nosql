# Quiz Aula 12 - CRUD Básico no MongoDB 🧠

Teste seus conhecimentos sobre as operações fundamentais no banco de dados NoSQL.

---

1. **Qual comando é usado para inserir múltiplos documentos de uma vez em uma coleção?**
    - [ ] `insert()`
    - [ ] `addMany()`
    - [x] `insertMany()`
    - [ ] `push()`
    - [ ] `create()`

    > **Explicação**: `insertMany()` aceita um array de objetos para inserção em lote.

2. **O comando `db.usuarios.find({ idade: 25 })` equivale a qual cláusula SQL?**
    - [ ] `SELECT * FROM usuarios`
    - [ ] `ORDER BY idade`
    - [x] `SELECT * FROM usuarios WHERE idade = 25`
    - [ ] `GROUP BY idade`
    - [ ] `DELETE FROM usuarios`

    > **Explicação**: Passar um objeto para o `find()` define os critérios de filtragem (Busca).

3. **No MongoDB, o que acontece se você tentar inserir dados em uma coleção que ainda não existe?**
    - [ ] O banco retorna um erro de "Tabela não encontrada".
    - [ ] O banco pede para você criar a tabela primeiro.
    - [x] O banco cria a coleção e insere o documento automaticamente.
    - [ ] O banco trava.
    - [ ] O banco deleta os dados.

    > **Explicação**: NoSQL é Schema-less; a estrutura é criada "on the fly" na primeira inserção.

4. **Para atualizar apenas ALGUNS campos de um documento sem apagar o restante, usamos o operador:**
    - [ ] `$update`
    - [ ] `$change`
    - [x] `$set`
    - [ ] `$replace`
    - [ ] `$fix`

    > **Explicação**: O `$set` atualiza apenas as chaves informadas, mantendo o restante do documento intacto.

5. **Qual a função do operador `$gt` nas consultas do MongoDB?**
    - [ ] Abrir o banco (Get).
    - [x] Filtrar valores "Maiores Que" (Greater Than).
    - [ ] Filtrar valores "Menores Que" (Gue Less Than).
    - [ ] Gerar um ID aleatório.
    - [ ] Agrupar por data (Group Time).

    > **Explicação**: Operadores lógicos como `$gt`, `$lt`, `$gte` são fundamentais para filtros numéricos.

6. **Como deletar TODOS os documentos de uma coleção, mas manter a coleção ativa?**
    - [ ] `db.colecao.drop()`
    - [ ] `db.colecao.remove()`
    - [x] `db.colecao.deleteMany({})`
    - [ ] `db.colecao.clear()`
    - [ ] `db.colecao.empty()`

    > **Explicação**: Passar um objeto vazio `{}` para o `deleteMany` remove todos os registros que casarem com o filtro (ou seja, todos).

7. **O campo `_id` que surge automaticamente em cada documento serve para:**
    - [ ] Guardar o nome do usuário.
    - [x] Servir como Chave Primária única e obrigatória do documento.
    - [ ] Contar quantas vezes o documento foi lido.
    - [ ] Definir a cor do ícone no Compass.
    - [ ] Não serve para nada, pode ser removido.

    > **Explicação**: O `_id` (geralmente um ObjectId) garante que cada documento seja único no banco.

8. **Qual ferramenta visual oficial é usada para gerenciar o MongoDB?**
    - [ ] pgAdmin.
    - [ ] MySQL Workbench.
    - [x] MongoDB Compass.
    - [ ] VS Code.
    - [ ] Notepad++.

    > **Explicação**: Compass é a interface gráfica (GUI) oficial e gratuita para explorar dados do MongoDB.

9. **O que o comando `db.produtos.updateOne({ nome: "Mouse" }, { $set: { preco: 60 } })` faz?**
    - [ ] Cria um novo mouse com preço 60.
    - [x] Altera o preço do primeiro mouse encontrado na lista para 60.
    - [ ] Deleta todos os mouses por segurança.
    - [ ] Altera o preço de todos os mouses da loja.
    - [ ] Dá erro por falta de vírgula.

    > **Explicação**: `updateOne` atinge apenas o primeiro documento que satisfaz o critério de busca.

10. **A sigla CRUD significa:**
    - [ ] Copy, Read, Update, Delete.
    - [x] Create, Read, Update, Delete.
    - [ ] Create, Run, Use, Deploy.
    - [ ] Clear, Reset, Undo, Done.
    - [ ] Console, Remote, User, Data.

    > **Explicação**: São as quatro operações fundamentais de qualquer sistema de persistência de dados.