# Projeto 16: Projeto Final Integrador - OmniStore 🎓

**Objetivo**: Integrar os mundos SQL e NoSQL para criar uma arquitetura de dados moderna, robusta e escalável para uma startup de varejo.

---

## 📝 O Desafio: OmniStore Global
A OmniStore é uma rede que vende produtos físicos e digitais em 50 países. Você foi escalado como Líder de Dados para projetar a V1.0 do sistema.

## 🚀 Requisitos do Projeto

### Parte 1: O Núcleo Relacional (PostgreSQL)
1.  **Modelagem**: Crie as tabelas de `usuarios`, `pedidos` e `pagamentos`.
2.  **Segurança**: Implemente uma transação que, ao registrar um pagamento, mude o status do pedido para "Pago".
3.  **Relatório**: Gere um ranking dos top 5 clientes que mais gastaram na loja.

### Parte 2: O Cérebro Flexível (MongoDB)
1.  **Modelagem**: Crie a coleção `catalogo_produtos`. Como cada produto tem atributos diferentes (ex: uma TV tem Polegadas, mas um Sapato tem Tamanho), use a flexibilidade do NoSQL.
2.  **Engajamento**: Modele as `avaliacoes` (reviews) dos produtos. Elas devem ser aninhadas ou referenciadas? Explique no código.
3.  **Agregação**: Crie um pipeline que mostre a média de nota (rating) por categoria de produto.

### Parte 3: Integração e Documentação
1.  Escreva um documento (Markdown) explicando por que você não usou apenas UM tipo de banco.
2.  Descreva qual o papel do **MongoDB Atlas** nessa arquitetura.
3.  Inclua links ou screenshots para os scripts SQL e comandos do MongoDB.

---

## ✅ Critérios de Avaliação
*   **Completude**: Cumprimento de todos os requisitos técnicos.
*   **Qualidade**: Código identado, comentado e sem erros.
*   **Arquitetura**: Escolha correta de qual dado vai para qual banco.
*   **Apresentação**: README.md claro e profissional no repositório.

---

## 🎓 Parabéns!
Este é o ápice do seu aprendizado. Ao terminar este projeto, você terá em mãos um portfólio de peso para apresentar em qualquer entrevista técnica! 🚀