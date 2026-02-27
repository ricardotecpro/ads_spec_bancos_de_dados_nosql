# Exercícios: Aula 13 - Modelagem de Documentos (NoSQL) 🏗️

Aprenda a arte de decidir entre unir ou separar seus dados no MongoDB.

---

## 🟢 Nível: Básico

### 1. Conceitos de Modelagem
Explique com suas palavras a diferença entre as estratégias de **Embedding** e **Referencing**.

### 2. Escolha de Estratégia
Em um sistema de biblioteca, você armazenaria os capítulos de um livro de forma **Aninhada** ou **Referenciada** no documento do Livro? Justifique.

---

## 🟡 Nível: Intermediário

### 3. Modelagem de Usuário
Desenhe um JSON de um usuário que contenha:
*   Nome e E-mail.
*   Três endereços aninhados (Casa, Trabalho, Praia).
*   Uma lista de IDs de `fotos_perfil` (Referenciadas).

### 4. Vantagens e Desvantagens
Cite uma vantagem de performance e uma desvantagem de manutenção ao usar o **Embedding**.

---

## 🔴 Nível: Desafio

### 5. O Cenário Híbrido
Imagine um sistema de rede social como o Twitter.
1.  O perfil do usuário deve ter os nomes dos seus 5 amigos mais próximos aninhados.
2.  As postagens do usuário (que podem ser milhares) devem ser referenciadas.
3.  Escreva o JSON que represente esse perfil de usuário seguindo essa lógica.
4.  Por que guardamos os nomes dos amigos aninhados se já temos os IDs deles? (Dica: Pesquise por *Extended Reference Pattern*).