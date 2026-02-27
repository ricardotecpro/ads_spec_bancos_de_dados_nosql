# Quiz Aula 07 - Consultas Avançadas e Agregações 🧠

Teste sua capacidade de gerar relatórios e sumarizar dados em SQL.

---

1. **Qual função é usada para contar o número de linhas em um resultado?**
    - [ ] `TOTAL()`
    - [ ] `SUM()`
    - [x] `COUNT()`
    - [ ] `ADD()`
    - [ ] `NUMBER()`

    > **Explicação**: `COUNT(*)` ou `COUNT(coluna)` devolve o número de registros encontrados.

2. **Para calcular a média aritmética de uma coluna numérica, usamos:**
    - [ ] `MEDIUM()`
    - [ ] `SUM()`
    - [x] `AVG()`
    - [ ] `MIN()`
    - [ ] `MAX()`

    > **Explicação**: `AVG` vem de *Average* (média).

3. **Qual função retorna o maior valor encontrado em uma coluna?**
    - [ ] `BIGGEST()`
    - [ ] `LARGER()`
    - [x] `MAX()`
    - [ ] `TOP()`
    - [ ] `CEIL()`

    > **Explicação**: `MAX()` identifica o valor máximo do conjunto.

4. **Para que serve a cláusula `AS` em uma consulta SQL?**
    - [ ] Para salvar o resultado em um arquivo.
    - [ ] Para definir o banco de dados.
    - [x] Para dar um apelido (Alias) a uma coluna ou tabela.
    - [ ] Para ordenar os dados por data.
    - [ ] Para deletar dados antigos.

    > **Explicação**: O apelido ajuda na leitura de colunas calculadas (ex: `SUM(x) AS total`).

5. **Quando usamos o `GROUP BY`?**
    - [ ] Sempre que usamos o WHERE.
    - [ ] Para apagar grupos de usuários.
    - [x] Sempre que queremos aplicar funções de agregação em grupos específicos de dados.
    - [ ] Para conectar duas tabelas diferentes.
    - [ ] Para formatar o texto em negrito.

    > **Explicação**: O GROUP BY agrupa registros que têm o mesmo valor em colunas específicas.

6. **Qual a principal diferença entre WHERE e HAVING?**
    - [ ] Não há diferença, são sinônimos.
    - [x] WHERE filtra registros individuais; HAVING filtra grupos (depois da agregação).
    - [ ] HAVING é apenas para o MySQL.
    - [ ] WHERE é mais rápido que o HAVING.
    - [ ] HAVING é usado apenas com strings.

    > **Explicação**: O WHERE atua antes do agrupamento, o HAVING atua sobre o resultado do agrupamento.

7. **Como você somaria todo o faturamento da tabela `vendas`?**
    - [ ] `SELECT COUNT(valor) FROM vendas`
    - [x] `SELECT SUM(valor) FROM vendas`
    - [ ] `SELECT ADD(valor) FROM vendas`
    - [ ] `SELECT TOTAL(valor) FROM vendas`
    - [ ] `SELECT * FROM vendas`

    > **Explicação**: `SUM` adiciona todos os valores numéricos de uma coluna.

8. **Para encontrar quantos estados diferentes existem na tabela de clientes, usamos:**
    - [ ] `COUNT(estado)`
    - [ ] `SUM(estado)`
    - [x] `COUNT(DISTINCT estado)`
    - [ ] `AVG(estado)`
    - [ ] `SELECT estado FROM clientes`

    > **Explicação**: O `DISTINCT` garante que cada estado seja contato apenas uma vez.

9. **O que acontece se você usar `MAX(nome)` em uma coluna de texto?**
    - [ ] O comando dá erro pois não é número.
    - [ ] Ele retorna o nome com mais letras.
    - [x] Ele retorna o último valor em ordem alfabética.
    - [ ] Ele retorna o nome do usuário mais velho.
    - [ ] Ele retorna null.

    > **Explicação**: Funções de agregação também funcionam com texto seguindo a ordem alfabética.

10. **A cláusula HAVING deve vir obrigatoriamente APÓS qual comando?**
    - [ ] `SELECT`
    - [ ] `WHERE`
    - [x] `GROUP BY`
    - [ ] `ORDER BY`
    - [ ] `LIMIT`

    > **Explicação**: Não faz sentido filtrar um grupo que ainda não foi criado pelo GROUP BY.