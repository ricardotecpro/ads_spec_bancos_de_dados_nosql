# Aula 04: DDL - Criação da Estrutura 🏗️
## Mão na Massa com SQL
### Ricardo Pires
#### Bancos de Dados SQL e NoSQL

---

## 🎯 O que vamos aprender hoje?
- A linguagem DDL
- Criando Bancos de Dados
- Criando Tabelas e Tipos
- Constraints (Restrições)
- Índices e Performance
- Alterando e Removendo Estruturas

---

## 📜 O que é DDL?
- **D**ata **D**efinition **L**anguage
- Foco na **ESTRUTURA** (o container)
- Não mexe nos dados (linhas) ainda! 📂 <!-- .element: class="fragment" -->

---

## 🛠️ Comandos Principais
- `CREATE`: Criar
- `ALTER`: Mudar
- `DROP`: Destruir 🔥
- `TRUNCATE`: Esvaziar <!-- .element: class="fragment" -->

---

## 🏗️ Criando o Banco de Dados
```sql
CREATE DATABASE meu_projeto;
```
- Dica: No pgAdmin, você pode usar a interface visual, mas o SQL é mais poderoso!

---

## 📑 Criando uma Tabela
```sql
CREATE TABLE usuarios (
    id SERIAL PRIMARY KEY,
    nome VARCHAR(100) NOT NULL,
    email VARCHAR(150) UNIQUE
);
```
- `SERIAL`: Auto-incremento ➕
- `NOT NULL`: Obrigatório ❗
- `UNIQUE`: Sem repetições 🆔 <!-- .element: class="fragment" -->

---

## 🔑 Restrições (Constraints)
Servem para garantir a qualidade:
- **PK**: Chave Primária
- **FK**: Chave Estrangeira
- **CHECK**: Validação personalizada
- **DEFAULT**: Valor padrão <!-- .element: class="fragment" -->

---

## ⛓️ Criando Chave Estrangeira (FK)
```sql
CREATE TABLE pedidos (
    id SERIAL PRIMARY KEY,
    id_cliente INT REFERENCES usuarios(id),
    total DECIMAL(10,2)
);
```
- O comando `REFERENCES` cria o elo de integridade! 🛡️

---

## ✅ A cláusula CHECK
```sql
ALTER TABLE usuarios 
ADD CHECK (idade >= 18);
```
- Impede a entrada de dados inválidos na raiz! <!-- .element: class="fragment" -->

---

## ⚡ Índices: O Atalho
- Sem Índice: Busca sequencial (lento) 🐢
- Com Índice: Busca binária/B-Tree (rápido) 🐇
```sql
CREATE INDEX idx_email ON usuarios(email);
```

---

## ⚖️ Prós e Contras dos Índices
- **Pró**: Leituras instantâneas
- **Contra**: Deixa o `INSERT` um pouco mais pesado
- **Regra**: Indexe colunas muito usadas no `WHERE`. <!-- .element: class="fragment" -->

---

## 🔨 Alterando a Tabela (ALTER)
- Mudar nome da coluna
- Mudar tipo de dado
- Adicionar ou remover restrições
```sql
ALTER TABLE usuarios 
RENAME COLUMN nome TO nome_completo;
```

---

## 🔥 Destruindo com Segurança (DROP)
```sql
DROP TABLE usuarios;
```
- Cuidado: Isso apaga a tabela E os dados dela! 🛑
- Use `DROP TABLE IF EXISTS` para scripts mais seguros. <!-- .element: class="fragment" -->

---

## 🧹 Limpeza Rápida (TRUNCATE)
- Quer limpar a tabela sem apagar a estrutura?
```sql
TRUNCATE TABLE logs;
```
- Muito mais rápido que `DELETE FROM logs`. <!-- .element: class="fragment" -->

---

## 💻 Visualizando no pgAdmin
- Query Tool: Onde a mágica acontece
- Dashboards: Monitorando o servidor
- ERD Tool: Gerador de diagrama a partir do código

---

## 🧬 Ciclo de Vida do Banco
1. Planejar (DER)
2. Criar (DDL)
3. Popular (DML - Próxima aula!)
4. Consultar (DQL)

---

## 🧠 Desafio Prático
- Tente criar um script SQL para:
- Tabela `Escolas`
- Tabela `Salas` (com FK para Escolas)
- Coluna `capacidade` com `CHECK > 0`. <!-- .element: class="fragment" -->

---

## 🚀 Dica de Mestre
Sempre use scripts `.sql` para criar seus bancos.
- Facilita o deploy
- Serve como documentação
- Permite controle de versão (Git) <!-- .element: class="fragment" -->

---

## 🏁 Resumo
- DDL define a "casa" dos dados
- `CREATE`, `ALTER`, `DROP` são os pilares
- PKs e FKs garantem a ordem
- Índices garantem a velocidade

---

## 👋 Até a próxima aula!
### Tema: Módulo II - SQL Prática (DML) ⚙️
["Ir para Prática"](../exercicios/exercicio-04.md)