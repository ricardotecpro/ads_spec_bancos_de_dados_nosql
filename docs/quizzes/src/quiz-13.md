# Quiz Aula 13 - Modelagem de Documentos 🧠

Teste sua visão estratégica de como organizar dados no MongoDB.

---

1. **A frase "Dados que são lidos juntos, devem ser salvos juntos" define qual estratégia?**
    - [ ] Referência.
    - [ ] Normalização.
    - [x] Aninhamento (Embedding).
    - [ ] Deleção.
    - [ ] Indexação.

    > **Explicação**: Esta é a filosofia base do NoSQL para otimizar a performance de leitura.

2. **Qual a principal vantagem do Aninhamento (Embedding)?**
    - [ ] Economiza espaço em disco.
    - [x] Extremamente rápido para leitura, pois evita JOINs em memória.
    - [ ] Permite que o documento cresça infinitamente.
    - [ ] Torna os dados mais confidenciais.
    - [ ] É o padrão de todos os bancos SQL.

    > **Explicação**: Trazer todos os dados relacionados em uma única consulta ao disco é o segredo da velocidade do MongoDB.

3. **O limite máximo de tamanho para um documento no MongoDB é:**
    - [ ] 1MB.
    - [ ] 4MB.
    - [x] 16MB.
    - [ ] 1GB.
    - [ ] Ilimitado.

    > **Explicação**: O MongoDB impõe um limite de 16MB por documento para evitar uso excessivo de memória RAM e lentidão.

4. **Quando um relacionamento é 1:Muitos (ex: Milhares de posts de um usuário), qual a melhor escolha?**
    - [ ] Anilhamento (Embedding).
    - [x] Referência (Linking).
    - [ ] Apagar os dados.
    - [ ] Criar uma nova coleção para cada post.
    - [ ] Usar Excel.

    > **Explicação**: O aninhamento de milhares de itens faria o documento estourar o limite de 16MB.

5. **A Referência (Linking) no MongoDB se assemelha a qual conceito do SQL?**
    - [ ] SELECT.
    - [ ] INDEX.
    - [x] Chave Estrangeira (Foreign Key).
    - [ ] INNER JOIN nativo.
    - [ ] TRIGGER.

    > **Explicação**: Na referência, guardamos o ID de outro documento para simbolizar a relação entre eles.

6. **Desvantagem do Aninhamento (Embedding):**
    - [ ] Os dados ficam desorganizados.
    - [ ] É impossível buscar os dados aninhados.
    - [ ] O banco de dados para de funcionar.
    - [x] Pode causar redundância de dados e dificultar a atualização em massa.
    - [ ] Exige que o usuário saiba SQL.

    > **Explicação**: Se o dado aninhado muda em um lugar, você teria que atualizar em todos os documentos onde ele foi replicado.

7. **O que é um "Relacionamento Híbrido"?**
    - [ ] Quando o banco é metade SQL e metade NoSQL.
    - [ ] Quando o banco roda em dois servidores diferentes.
    - [x] Quando usamos Referência, mas aninhamos os campos mais usados para evitar buscas extras.
    - [ ] Quando o código é feito em Java e Kotlin ao mesmo tempo.
    - [ ] Quando usamos MongoDB local e remoto.

    > **Explicação**: É a técnica de guardar o ID (Referência) + Informação básica (Nome) para agilizar a exibição da lista.

8. **Para representar um "Carrinho de Compras" com 1 a 10 itens, o que você usaria?**
    - [ ] Referência.
    - [x] Aninhamento.
    - [ ] Cross Join.
    - [ ] Tabela Associativa.
    - [ ] CSV externo.

    > **Explicação**: Como o número de itens é pequeno e fixo por carrinho, o aninhamento é ideal.

9. **Por que no NoSQL dizemos que a modelagem é "orientada à aplicação"?**
    - [ ] Porque o programador escolhe o banco.
    - [ ] Porque os aplicativos são lentos.
    - [x] Porque desenhamos os dados baseados em como a tela do app vai exibi-los.
    - [ ] Porque o banco não aceita comandos via console.
    - [ ] Porque o app cria o banco de dados.

    > **Explicação**: No NoSQL, priorizamos a performance e a usabilidade do app final em vez da perfeição matemática da normalização.

10. **A redundância de dados no NoSQL é vista como:**
    - [ ] Um erro grave do programador.
    - [ ] Um problema de segurança.
    - [x] Um preço aceitável para ganhar performance de leitura.
    - [ ] Algo que o MongoDB corrige sozinho.
    - [ ] O motivo de o banco ser gratuito.

    > **Explicação**: Replicar dados (Denormalização) é uma técnica comum para evitar consultas complexas e lentas.