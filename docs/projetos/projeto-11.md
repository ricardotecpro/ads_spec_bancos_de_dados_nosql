# Projeto 11: Comparativo Relacional vs NoSQL 🌐

**Objetivo**: Analisar criticamente as diferenças entre os modelos e converter uma estrutura relacional para o formato de documento.

---

## 📝 O Desafio
Você tem o modelo de um **Blog** no PostgreSQL:
*   Tabela `Autores` (id, nome)
*   Tabela `Posts` (id, titulo, conteudo, autor_id)
*   Tabela `Comentarios` (id, texto, post_id)

## 🚀 Tarefas
1.  **Mapeamento**: Desenhe como essa estrutura ficaria em um **único documento JSON** no MongoDB (utilizando aninhamento).
2.  **Análise de Vantagens**: Liste 3 vantagens de usar o MongoDB para este cenário de Blog.
3.  **Análise de Riscos**: Liste 2 riscos de segurança ou integridade que o MongoDB traz em comparação ao PostgreSQL.

## ✅ Critérios de Entrega
*   O código JSON formatado do post com seus comentários e autor.
*   Um pequeno texto (bullet points) comparativo.