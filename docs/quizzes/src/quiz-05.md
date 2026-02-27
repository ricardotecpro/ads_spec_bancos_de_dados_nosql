# Quiz Aula 05 - DML (Manipulação de Dados) 🧠

Teste seus conhecimentos sobre como inserir, alterar e remover dados em tabelas SQL.

---

1. **O que significa a sigla DML?**
    - [ ] Data Management Layout.
    - [ ] Dynamic Memory Loading.
    - [x] Data Manipulation Language.
    - [ ] Database Mode Locator.
    - [ ] Database Mother Language.

    > **Explicação**: DML é a parte do SQL que lida com o conteúdo das tabelas (os dados), não com a estrutura.

2. **Qual comando é usado para adicionar novos registros a uma tabela?**
    - [ ] `ADD`
    - [ ] `NEW`
    - [x] `INSERT`
    - [ ] `CREATE`
    - [ ] `PUT`

    > **Explicação**: `INSERT INTO` é o comando padrão para inserir novas linhas de dados.

3. **Se uma coluna foi definida com o tipo `SERIAL`, o que acontece no INSERT?**
    - [ ] O usuário deve obrigatoriamente digitar o número.
    - [x] O banco de dados gera o próximo número da sequência automaticamente.
    - [ ] O banco de dados gera um texto aleatório.
    - [ ] O comando INSERT falha se não houver um ID manual.
    - [ ] A coluna é preenchida com a data atual.

    > **Explicação**: `SERIAL` automatiza o preenchimento de IDs, evitando erros de duplicidade manual.

4. **Para atualizar informações em um banco relacional, usamos:**
    - [ ] `CHANGE`
    - [ ] `UPGRADE`
    - [ ] `MODIFY`
    - [x] `UPDATE`
    - [ ] `REPLACE`

    > **Explicação**: `UPDATE` permite modificar valores de colunas em registros já existentes.

5. **Qual a função da cláusula `SET` no comando UPDATE?**
    - [ ] Filtrar quais linhas serão alteradas.
    - [ ] Criar uma nova tabela.
    - [x] Definir quais colunas receberão os novos valores.
    - [ ] Ordenar os resultados.
    - [ ] Deletar os dados antigos.

    > **Explicação**: No comando `UPDATE`, o `SET` especifica "o que" será mudado (ex: `SET preco = 10`).

6. **O que acontece se um comando DELETE for executado sem a cláusula WHERE?**
    - [ ] O comando retorna um erro de sintaxe.
    - [ ] Apenas o primeiro registro é apagado.
    - [ ] O banco de dados pede uma confirmação por e-mail.
    - [x] Todos os registros da tabela são excluídos permanentemente.
    - [ ] Nada acontece, o WHERE é obrigatório no PostgreSQL.

    > **Explicação**: O DELETE sem filtro atua sobre todo o conjunto de dados da tabela.

7. **Qual é o comando mais adequado para apagar todos os dados de uma tabela muito grande de forma extremamente rápida?**
    - [ ] `DELETE ALL`
    - [ ] `DROP TABLE`
    - [x] `TRUNCATE TABLE`
    - [ ] `REMOVE DATA`
    - [ ] `WIPE TABLE`

    > **Explicação**: `TRUNCATE` esvazia a tabela ignorando triggers e logs de exclusão linha a linha, sendo muito mais performático.

8. **Como se insere múltiplos registros em um único comando SQL?**
    - [ ] Executando vários `INSERT INTO` separados por ponto e vírgula.
    - [x] Usando `VALUES` seguido de várias listas de parênteses separadas por vírgula.
    - [ ] Criando uma tabela temporária de importação.
    - [ ] Usando o comando `MULTI INSERT`.
    - [ ] Não é possível, deve-se inserir um por um.

    > **Explicação**: Ex: `INSERT INTO t (val) VALUES (1), (2), (3);`.

9. **No comando UPDATE, qual operador usamos para aumentar um valor numérico em 10%?**
    - [ ] `SET preco = preco + 10`
    - [ ] `SET preco = 1.10`
    - [x] `SET preco = preco * 1.10`
    - [ ] `SET preco = preco / 10`
    - [ ] `SET preco = +10%`

    > **Explicação**: Multiplicar por 1.10 adiciona 10% ao valor original da coluna.

10. **Qual comando DML deve ser usado com mais cautela pelo administrador?**
    - [ ] `INSERT`
    - [ ] `SELECT`
    - [x] `DELETE`
    - [ ] `COMMIT`
    - [ ] `ROLLBACK`

    > **Explicação**: O `DELETE` (especialmente sem WHERE) pode causar perda irreversível de dados se não houver backups.