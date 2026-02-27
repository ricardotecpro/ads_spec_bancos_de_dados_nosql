# Quiz Aula 14 - Consultas e Agregações no MongoDB 🧠

Teste seus conhecimentos sobre o poderoso Aggregation Framework do MongoDB.

---

1. **A estrutura de agregação do MongoDB é baseada no conceito de:**
    - [ ] Tabelas Verdade.
    - [ ] Árvores Binárias.
    - [x] Pipelines (Linhas de Montagem).
    - [ ] Recursividade Infinita.
    - [ ] JOINs Automáticos.

    > **Explicação**: O framework processa documentos através de uma série de estágios sequenciais.

2. **Qual estágio do pipeline é usado para FILTRAR documentos?**
    - [ ] `$filter`
    - [ ] `$where`
    - [x] `$match`
    - [ ] `$select`
    - [ ] `$limit`

    > **Explicação**: O `$match` funciona como a cláusula WHERE do SQL.

3. **Para realizar agrupamentos (como somar ou tirar a média), usamos o estágio:**
    - [ ] `$total`
    - [ ] `$collect`
    - [x] `$group`
    - [ ] `$combine`
    - [ ] `$aggregate`

    > **Explicação**: O `$group` permite agrupar por uma chave específica e aplicar funções matemáticas.

4. **Qual operador de grupo usamos para contar quantos itens existem em um grupo?**
    - [ ] `{ $count: 1 }`
    - [x] `{ $sum: 1 }`
    - [ ] `{ $add: 1 }`
    - [ ] `{ $total: 1 }`
    - [ ] `{ $list: 1 }`

    > **Explicação**: Somar 1 para cada documento encontrado no grupo é a forma padrão de contar.

5. **O estágio `$lookup` serve para:**
    - [ ] Buscar um texto dentro do documento.
    - [ ] Criar um índice.
    - [x] Unir dados de duas coleções diferentes (simula um JOIN).
    - [ ] Formatar a saída do JSON.
    - [ ] Deletar documentos duplicados.

    > **Explicação**: Ele permite buscar documentos em outra coleção que correspondam a um campo específico.

6. **Para escolher apenas alguns campos e esconder outros no resultado final, usamos:**
    - [ ] `$hide`
    - [ ] `$view`
    - [x] `$project`
    - [ ] `$only`
    - [ ] `$display`

    > **Explicação**: `$project` controla a "projeção" do documento final.

7. **Como ordenar os resultados de uma agregação de forma DESCENDENTE (do maior para o menor)?**
    - [ ] `{ $sort: 1 }`
    - [x] `{ $sort: -1 }`
    - [ ] `{ $order: "DESC" }`
    - [ ] `{ $rank: -1 }`
    - [ ] `{ $sort: "top" }`

    > **Explicação**: No MongoDB, `1` é ascendente e `-1` é descendente.

8. **O estágio `$limit` deve ser usado geralmente:**
    - [ ] No início de todos os pipelines.
    - [ ] Apenas se o banco der erro.
    - [x] No final do pipeline para restringir o volume de dados exibidos.
    - [ ] Para aumentar a memória do servidor.
    - [ ] Para mudar o nome da coleção.

    > **Explicação**: Ele limita a quantidade de documentos que saem da "linha de montagem".

9. **O que acontece se você colocar o `$match` após o `$group` em uma coleção de 1 milhão de itens?**
    - [ ] O banco explode.
    - [ ] A consulta fica mais rápida.
    - [x] A consulta fica lenta, pois o banco teve que agrupar 1 milhão de itens antes de filtrar.
    - [ ] O resultado é deletado.
    - [ ] O banco ignora o filtro.

    > **Explicação**: Filtrar o quanto antes economiza processamento e memória.

10. **A agregação no MongoDB é executada em:**
    - [ ] No navegador do usuário.
    - [x] No servidor de banco de dados.
    - [ ] No celular do cliente.
    - [ ] Em um arquivo Excel.
    - [ ] No satélite do GPS.

    > **Explicação**: O banco processa tudo internamente e devolve apenas o resultado final para a aplicação.