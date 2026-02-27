# Projeto 13: Arquitetando o Banco de um App de Música 🏗️

**Objetivo**: Aplicar padrões de modelagem NoSQL para um cenário real de streaming de música.

---

## 📝 O Desafio
Você foi contratado para desenhar o banco de dados de um novo "Spotify". Você precisa decidir como armazenar as informações para que o app seja veloz.

## 🚀 Tarefas
1.  **Modelagem de Playlist**: Desenhe o JSON de uma `Playlist`. Ela deve conter o nome, o autor e uma lista das 10 primeiras músicas (nome e duração). Você vai usar **Aninhamento** ou **Referência** para as músicas totais da playlist?
2.  **Modelagem de Artista**: Como guardar a biografia e a lista de álbuns?
3.  **Justificativa**: Escreva um pequeno parágrafo explicando por que você escolheu aninhamento para as músicas da playlist (ou por que não escolheu).
4.  **Criação no MongoDB**: Execute os comandos `insertOne` no mongosh para criar um exemplo real das coleções `artistas` e `playlists`.

## ✅ Critérios de Entrega
*   O desenho dos 2 esquemas JSON.
*   O script `.js` com as inserções.
*   Explicação técnica da escolha da estratégia.