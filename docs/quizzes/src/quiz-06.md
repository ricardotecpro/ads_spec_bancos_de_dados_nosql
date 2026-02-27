# Quiz Aula 06 - DQL Básico 🧠

Teste sua habilidade em extrair informações de bancos de dados relacionais.

---

1. **Qual é o comando principal do subconjunto DQL?**
    - [ ] `GET`
    - [ ] `FETCH`
    - [x] `SELECT`
    - [ ] `SEARCH`
    - [ ] `SHOW`

    > **Explicação**: `SELECT` é a palavra-chave universal para consultas em SQL.

2. **O que o caractere asterisco (`*`) representa em um comando SELECT?**
    - [ ] A primeira coluna da tabela.
    - [ ] Apenas as colunas que possuem dados.
    - [x] Todas as colunas disponíveis na tabela.
    - [ ] O banco de dados inteiro.
    - [ ] Uma busca aproximada.

    > **Explicação**: `SELECT *` recupera todos os atributos de uma tabela.

3. **Como chamamos o ato de escolher apenas algumas colunas específicas em uma consulta?**
    - [ ] Seleção.
    - [x] Projeção.
    - [ ] Filtro.
    - [ ] Agregação.
    - [ ] Ordenação.

    > **Explicação**: Projeção é a escolha das colunas (eixo vertical), seleçã é a escolha das linhas (eixo horizontal).

4. **Para filtrar as linhas que devem aparecer no resultado, usamos a cláusula:**
    - [ ] `LIMIT`
    - [ ] `GROUP BY`
    - [ ] `FROM`
    - [x] `WHERE`
    - [ ] `ORDER BY`

    > **Explicação**: O `WHERE` permite definir condições lógicas para filtrar os registros.

5. **Qual operador é usado para verificar se um valor está dentro de um intervalo (mínimo e máximo)?**
    - [ ] `INSIDE`
    - [x] `BETWEEN`
    - [ ] `MIDDLE`
    - [ ] `RANGE`
    - [ ] `AMONG`

    > **Explicação**: `BETWEEN x AND y` é equivalente a `valor >= x AND valor <= y`.

6. **Para buscar nomes que começam com a letra "A", usamos qual padrão no PostgreSQL?**
    - [ ] `LIKE 'A?'`
    - [ ] `LIKE '*A'`
    - [x] `LIKE 'A%'`
    - [ ] `LIKE '#A'`
    - [ ] `STARTWITH 'A'`

    > **Explicação**: O símbolo `%` representa qualquer quantidade de caracteres após (ou antes) da letra informada.

7. **Como ordenar o resultado de uma consulta do preço mais alto para o mais baixo?**
    - [ ] `ORDER BY preco ASC`
    - [ ] `ORDER BY preco UP`
    - [x] `ORDER BY preco DESC`
    - [ ] `SORT BY preco HIGH`
    - [ ] `GROUP BY preco DESC`

    > **Explicação**: `DESC` vem de *Descending* (descendente).

8. **A cláusula `DISTINCT` serve para:**
    - [ ] Destacar o resultado em negrito.
    - [ ] Contar quantas linhas existem.
    - [x] Eliminar linhas duplicadas do resultado final.
    - [ ] Ordenar por ordem alfabética.
    - [ ] Buscar apenas dados diferentes de zero.

    > **Explicação**: Útil para ver, por exemplo, quais cidades diferentes existem na tabela de clientes.

9. **Qual operador busca valores que pertencem a uma lista pré-definida (ex: IDs 1, 3 e 5)?**
    - [ ] `LIST`
    - [ ] `ALL`
    - [ ] `WHERE id = (1,3,5)`
    - [x] `WHERE id IN (1, 3, 5)`
    - [ ] `WHERE id SEARCH (1,3,5)`

    > **Explicação**: O operador `IN` simplifica múltiplas condições de `OR`.

10. **Em um banco de dados com milhões de registros, por que evitar o `SELECT *`?**
    - [ ] Porque ele apaga os dados acidentalmente.
    - [x] Porque consome muita banda de rede e memória desnecessariamente.
    - [ ] Porque ele inverte a ordem das colunas.
    - [ ] Porque ele não funciona com o GROUP BY.
    - [ ] Porque ele limita o resultado a 100 linhas.

    > **Explicação**: Trazer apenas o que você precisa economiza recursos do servidor e do cliente.