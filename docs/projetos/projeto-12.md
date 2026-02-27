# Projeto 12: O Grande Inventário NoSQL 🍃

**Objetivo**: Aplicar os comandos de CRUD no MongoDB para gerenciar um catálogo de produtos flexível.

---

## 📝 O Desafio
Você está criando o sistema de estoque para uma loja de variedades que vende desde eletrônicos até roupas. Como os produtos são muito diferentes, você escolheu o MongoDB.

## 🚀 Tarefas
1.  **Criação**: Crie um banco chamado `loja_nosql` e uma coleção `estoque`.
2.  **Inserção Variada**: Insira 3 documentos com campos diferentes:
    *   Um Smartphone (com campos de bateria e memória).
    *   Uma Camisa (com campos de tamanho e tecido).
    *   Um Livro (com campos de autor e páginas).
3.  **Busca Filtrada**: Escreva o comando para localizar todos os produtos que custam acima de R$ 100,00.
4.  **Atualização Geral**: Adicione um campo `loja: "Sede Principal"` em todos os produtos do estoque.
5.  **Exclusão**: Delete o produto que possui o menor estoque.

## ✅ Critérios de Entrega
*   Um arquivo `.js` com os comandos usados no mongosh.
*   Screenshot do MongoDB Compass mostrando os documentos inseridos.