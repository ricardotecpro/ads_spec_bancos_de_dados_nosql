# Aula 04 - DDL (Criação da Estrutura) 🏗️

!!! tip "Objetivo"
    **Objetivo**: Aprender a linguagem DDL (Data Definition Language) para criar, alterar e excluir a estrutura física do banco de dados no PostgreSQL.

---

## 1. O que é DDL? 📜

**DDL** (Data Definition Language) é o subconjunto do SQL usado para definir a estrutura do banco de dados (o "esqueleto").

Comandos principais:
*   `CREATE`: Cria objetos (bancos, tabelas, índices).
*   `ALTER`: Altera a estrutura de objetos existentes.
*   `DROP`: Exclui objetos permanentemente.
*   `TRUNCATE`: Esvazia uma tabela (deleta os dados, mas mantém a estrutura).

---

## 2. Criando o Banco e Tabelas 🛠️

Antes de guardar dados, precisamos do "container".

### Criando o Banco de Dados
```sql
CREATE DATABASE curso_db;
```

### Criando uma Tabela Completa
```sql
CREATE TABLE professores (
    id SERIAL PRIMARY KEY,       -- Serial cria um autoincremento
    nome VARCHAR(100) NOT NULL,  -- Não permite valores vazios
    email VARCHAR(150) UNIQUE,  -- Não permite emails repetidos
    data_contratacao DATE DEFAULT CURRENT_DATE
);
```

---

## 3. Chaves e Restrições (Constraints) 🔑

As restrições garantem a qualidade dos dados.

*   `PRIMARY KEY`: Identificador único.
*   `FOREIGN KEY`: Relacionamento com outra tabela.
*   `NOT NULL`: Campo obrigatório.
*   `UNIQUE`: Valor não pode se repetir.
*   `CHECK`: Valida uma condição (ex: `CHECK (preco > 0)`).

---

## 4. Índices: Acelerando as Buscas ⚡

Índices funcionam como o sumário de um livro. Eles ajudam o SGBD a encontrar dados sem precisar ler a tabela inteira.

```sql
CREATE INDEX idx_nome_professor ON professores(nome);
```

> [!WARNING]
> Índices aceleram a leitura (`SELECT`), mas tornam a escrita (`INSERT`, `UPDATE`) um pouco mais lenta. Use com sabedoria!

---

## 5. Alterando e Excluindo 🔨

Errou o nome da coluna? Precisa adicionar um campo novo?

### Adicionando Coluna
```sql
ALTER TABLE professores ADD COLUMN especialidade VARCHAR(50);
```

### Removendo Tabela (CUIDADO!)
```sql
DROP TABLE professores; -- Isso apaga os dados e a estrutura!
```

---

## 6. Prática no Terminal (pgAdmin) 💻

Abra o Query Tool no seu pgAdmin e execute estes comandos:

```termynal
$ CREATE DATABASE escola;
$ \c escola (conectar no banco via psql)
$ 
$ CREATE TABLE alunos (
$     id SERIAL PRIMARY KEY,
$     nome VARCHAR(100) NOT NULL
$ );
```

---

## 7. Mini-Projeto: O Banco da Escola 🚀

Crie o script DDL para o seguinte cenário:
1.  Uma tabela `cursos` com `id`, `nome` e `carga_horaria`.
2.  Uma tabela `matriculas` que liga `alunos` (já criada) aos `cursos`.

> Dica: Use `REFERENCES` para criar a Chave Estrangeira.

---

## 8. Exercícios de Fixação 🧠

1.  Qual a diferença entre os comandos `DROP` e `TRUNCATE`?
2.  Por que a coluna `id` geralmente usa o tipo `SERIAL` no PostgreSQL?
3.  Escreva o comando SQL para adicionar uma restrição `UNIQUE` na coluna `CPF` da tabela `alunos`.

---

**Próxima Aula**: Vamos aprender a colocar dados nessas tabelas com o [DML - Manipulação de Dados](../aulas/aula-05.md)! ⚙️