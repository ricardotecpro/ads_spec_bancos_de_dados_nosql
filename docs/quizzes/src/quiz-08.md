# Quiz Aula 08 - JOINs: Junções entre Tabelas 🧠

Teste seus conhecimentos sobre como conectar informações de diferentes tabelas.

---

1. **Qual é a principal função do comando JOIN?**
    - [ ] Criar uma cópia de segurança da tabela.
    - [x] Unir colunas de duas ou mais tabelas baseando-se em uma coluna comum.
    - [ ] Mudar o nome das tabelas.
    - [ ] Somar todos os valores numéricos de um banco.
    - [ ] Apagar registros duplicados em tabelas diferentes.

    > **Explicação**: O JOIN permite que dados normalizados e separados sejam visualizados juntos.

2. **O `INNER JOIN` retorna quais tipos de registros?**
    - [ ] Todos os registros da tabela da esquerda.
    - [ ] Todos os registros de ambas as tabelas sempre.
    - [x] Apenas os registros que possuem correspondência nas duas tabelas.
    - [ ] Apenas os registros que não têm ligação.
    - [ ] Apenas registros de texto.

    > **Explicação**: Funciona como a "interseção" entre dois conjuntos.

3. **Qual a principal característica do `LEFT JOIN`?**
    - [ ] Ele deleta os registros da esquerda.
    - [x] Ele traz todos os registros da tabela da esquerda, mesmo sem par na direita.
    - [ ] Ele traz apenas o lado direito da tabela.
    - [ ] Ele inverte a ordem das colunas.
    - [ ] Ele é mais lento que o INNER JOIN.

    > **Explicação**: Garante a visualização total da "tabela base" (esquerda).

4. **Quando um `LEFT JOIN` não encontra um par na tabela da direita, o que ele exibe?**
    - [ ] Um erro de sistema.
    - [ ] O número zero.
    - [x] O valor `NULL`.
    - [ ] Uma mensagem de texto "Vazio".
    - [ ] Reinicia a busca do início.

    > **Explicação**: O NULL indica que não há informação associada naquele lado da junção.

5. **A cláusula usada para definir quais colunas ligam as tabelas no JOIN é:**
    - [ ] `WHERE`
    - [x] `ON`
    - [ ] `BY`
    - [ ] `KEY`
    - [ ] `LINK`

    > **Explicação**: O `ON` geralmente compara a PK de uma tabela com a FK de outra.

6. **O que acontece se você fizer um JOIN sem usar a cláusula `ON`?**
    - [ ] O banco escolhe as colunas automaticamente.
    - [x] Ocorre um **CROSS JOIN** (Produto Cartesiano), gerando muitas linhas.
    - [ ] O comando é cancelado por segurança.
    - [ ] Apenas a primeira linha é exibida.
    - [ ] O banco de dados trava.

    > **Explicação**: Sem a regra de ligação, o banco combina cada linha de A com TODAS as linhas de B.

7. **Como o `RIGHT JOIN` se diferencia do `LEFT JOIN`?**
    - [ ] É mais rápido.
    - [ ] É usado apenas para números.
    - [x] A prioridade de exibição total muda para a segunda tabela mencionada.
    - [ ] Ele apaga os dados da esquerda.
    - [ ] Não há diferença, são idênticos.

    > **Explicação**: O `RIGHT JOIN` prioriza a tabela da direita (a segunda tabela mencionada no código).

8. **Qual comando combina tudo de ambos os lados, preenchendo com NULL onde não há par?**
    - [ ] `INNER JOIN`
    - [ ] `LEFT JOIN`
    - [x] `FULL OUTER JOIN`
    - [ ] `CROSS JOIN`
    - [ ] `UNION`

    > **Explicação**: É a união total de dois conjuntos de dados.

9. **O ato de dar um nome curto para a tabela (ex: `FROM clientes c`) ajuda em quê?**
    - [ ] Deixa a consulta mais lenta.
    - [ ] Protege os nomes reais dos hackers.
    - [x] Facilita a escrita e leitura, evitando repetir nomes longos de tabelas.
    - [ ] Cria uma tabela temporária.
    - [ ] Muda o nome da tabela no disco.

    > **Explicação**: Aliases são essenciais em consultas com muitos JOINs para evitar confusão.

10. **Em um sistema de biblioteca, para ver todos os livros e os nomes de seus respectivos autores, qual JOIN é o mais indicado?**
    - [ ] `LEFT JOIN` na tabela de autores.
    - [x] `INNER JOIN` entre Livros e Autores.
    - [ ] `CROSS JOIN`.
    - [ ] `DROP JOIN`.
    - [ ] `DELETE JOIN`.

    > **Explicação**: O `INNER JOIN` mostrará os livros que possuem autores cadastrados corretamente.