# Quiz Aula 10 - Projeto Parcial: Sistema Relacional 🧠

Consolide seus conhecimentos sobre o Módulo II e verifique se você está pronto para o NoSQL.

---

1. **Qual a principal vantagem de usar um sistema de banco de dados relacional (SQL) para um E-commerce?**
    - [ ] Ele é mais colorido.
    - [ ] Ele não precisa de internet.
    - [x] Ele garante a integridade e consistência dos dados através de relacionamentos e transações.
    - [ ] Ele apaga os dados automaticamente.
    - [ ] Ele é gratuito em todos os servidores.

    > **Explicação**: SQL é ideal para dados que precisam de regras rígidas e precisão (como finanças e estoque).

2. **O comando que une dados de clientes e pedidos é o:**
    - [ ] `UNITE`
    - [ ] `CONCAT`
    - [x] `JOIN`
    - [ ] `MERGE`
    - [ ] `LINK`

    > **Explicação**: O JOIN é a ferramenta base para navegar entre tabelas relacionadas.

3. **Se eu quiser apagar uma categoria que ainda possui produtos associados, o que o SGBDR geralmente faz?**
    - [ ] Apaga tudo.
    - [x] Bloqueia a exclusão para manter a integridade referencial.
    - [ ] Muda o nome dos produtos.
    - [ ] Cria uma nova categoria.
    - [ ] Reinicia o servidor.

    > **Explicação**: Chaves estrangeiras servem para evitar que existam registros "órfãos".

4. **Qual o papel do `LIMIT` em um relatório de "Top 5 Produtos"?**
    - [ ] Ele define o preço máximo.
    - [ ] Ele ordena a lista.
    - [x] Ele restringe o resultado apenas às 5 primeiras linhas.
    - [ ] Ele apaga os outros produtos.
    - [ ] Ele cria um índice.

    > **Explicação**: LIMIT é fundamental para controlar o tamanho do resultado exibido.

5. **O que acontece se uma transação ACID sofrer uma queda de energia após o COMMIT?**
    - [ ] Os dados são perdidos.
    - [ ] A transação é cancelada.
    - [x] Os dados são mantidos, pois a propriedade Durabilidade garante a persistência em disco.
    - [ ] O banco de dados é corrompido.
    - [ ] O sistema pede para você digitar tudo de novo.

    > **Explicação**: Durabilidade garante que confirmou, tá salvo.

6. **A cláusula `WHERE` serve para filtrar:**
    - [ ] Grupos de dados.
    - [x] Linhas individuais antes da agregação.
    - [ ] O nome das colunas.
    - [ ] O tipo do banco de dados.
    - [ ] O usuário que está logado.

    > **Explicação**: O WHERE é o filtro primário de qualquer consulta SQL.

7. **Para saber o total faturado por cada vendedor, usamos:**
    - [ ] `ORDER BY vendedor_id`
    - [ ] `SELECT * FROM vendas`
    - [x] `SUM(valor)` com `GROUP BY vendedor_id`
    - [ ] `COUNT(valor)` com `HAVING`
    - [ ] `DISTINCT vendedor_id`

    > **Explicação**: Agrupamento + Soma é a fórmula para relatórios de faturamento.

8. **Qual o tipo de dado ideal para um campo de "Preço" que precisa de precisão centesimal?**
    - [ ] `INT`
    - [ ] `TEXT`
    - [ ] `BOOLEAN`
    - [x] `NUMERIC` ou `DECIMAL`
    - [ ] `VARCHAR`

    > **Explicação**: Tipos decimais exatos evitam erros de arredondamento em cálculos financeiros.

9. **O que é um script DDL?**
    - [ ] Um código para inserir dados.
    - [x] Um conjunto de comandos que definem a estrutura (tabelas, chaves) do banco.
    - [ ] Um backup dos dados.
    - [ ] Um comando de busca.
    - [ ] Uma senha de acesso.

    > **Explicação**: DDL = Define. DML = Manipula. DQL = Consulta.

10. **Ao final do Módulo II, qual sua principal conclusão sobre bancos relacionais?**
    - [ ] Eles são bagunçados.
    - [x] Eles são organizados, seguros e baseados em regras matemáticas (conjuntos).
    - [ ] Eles servem apenas para guardar nomes de pessoas.
    - [ ] Eles serão substituídos totalmente pelo Excel.
    - [ ] Eles não usam SQL.

    > **Explicação**: Bancos SQL são o pilar da organização de dados empresarial há décadas.