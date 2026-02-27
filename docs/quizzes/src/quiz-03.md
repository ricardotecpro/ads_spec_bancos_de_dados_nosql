# Quiz Aula 03 - Normalização e Estrutura Relacional 🧠

Teste seus conhecimentos sobre as regras de organização de dados e Formas Normais.

---

1. **Qual é o principal objetivo da Normalização de dados?**
    - [ ] Aumentar o tamanho do banco de dados para usar mais HD.
    - [ ] Criar nomes de tabelas mais longos e difíceis.
    - [x] Eliminar redundâncias e evitar anomalias de atualização.
    - [ ] Impedir que o usuário digite números negativos.
    - [ ] Criar backups automáticos em fita.

    > **Explicação**: A normalização organiza os dados para que cada informação seja armazenada em apenas um lugar, reduzindo erros e duplicidade.

2. **O que representa o valor "NULL" em um banco de dados?**
    - [ ] O número zero.
    - [ ] Uma string de texto vazia ("").
    - [x] A ausência de valor ou um valor desconhecido.
    - [ ] O final de uma tabela.
    - [ ] Um erro crítico que trava o servidor.

    > **Explicação**: NULL indica que a informação não foi preenchida ou não existe para aquele registro específico.

3. **Para estar na 1ª Forma Normal (1FN), uma tabela deve:**
    - [ ] Ter pelo menos 10 colunas.
    - [x] Possuir apenas valores atômicos (não divisíveis) em suas células.
    - [ ] Ter todas as chaves estrangeiras criptografadas.
    - [ ] Ser exportada para Excel mensalmente.
    - [ ] Ter apenas números inteiros.

    > **Explicação**: A 1FN proíbe listas de valores (como vários telefones em uma única célula) e grupos repetidos.

4. **A 2ª Forma Normal (2FN) lida principalmente com:**
    - [ ] A cor das tabelas no diagrama.
    - [x] A dependência de colunas não-chave em relação à chave primária completa.
    - [ ] A velocidade da conexão de rede.
    - [ ] O número de usuários conectados simultaneamente.
    - [ ] A ordem alfabética das colunas.

    > **Explicação**: A 2FN garante que em tabelas com chaves compostas, os dados dependam de toda a chave, não apenas de parte dela.

5. **Qual Forma Normal (FN) é violada quando uma coluna não-chave depende de outra coluna também não-chave?**
    - [ ] 1FN
    - [ ] 2FN
    - [x] 3FN
    - [ ] 4FN
    - [ ] Nenhuma, isso é permitido.

    > **Explicação**: A 3FN elimina as dependências transitivas, garantindo que colunas dependam apenas da chave primária.

6. **O que é um "Valor Atômico"?**
    - [ ] Um número que pode explodir o banco.
    - [ ] O ID de um átomo na tabela periódica.
    - [x] Um valor indivisível que representa uma única unidade de informação.
    - [ ] A soma de todos os bits de uma linha.
    - [ ] Um valor que nunca muda.

    > **Explicação**: Atomicidade significa que o dado não pode ser decomposto em partes menores com significados diferentes para o banco.

7. **Quando a "Desnormalização" pode ser aplicada?**
    - [ ] Sempre, para simplificar o banco.
    - [x] Para melhorar a performance de leitura em sistemas com volumes massivos de dados.
    - [ ] Quando o desenvolvedor esquece as regras da 3FN.
    - [ ] Para economizar espaço em disco.
    - [ ] Apenas em bancos NoSQL.

    > **Explicação**: A desnormalização é uma decisão estratégica para ganhar velocidade em consultas complexas, sacrificando a economia de espaço.

8. **O tipo de dado `VARCHAR(100)` no PostgreSQL serve para:**
    - [ ] Guardar números decimais com 100 casas.
    - [x] Guardar texto de tamanho variável até 100 caracteres.
    - [ ] Armazenar 100 datas diferentes.
    - [ ] Criar 100 tabelas automaticamente.
    - [ ] Definir a idade do usuário.

    > **Explicação**: VARCHAR é o tipo padrão para textos curtos e médios, como nomes e endereços.

9. **O conceito de "Especialização" no banco de dados permite:**
    - [ ] Que o banco rode apenas em servidores especiais.
    - [x] Criar tabelas filhas com atributos específicos a partir de uma tabela geral.
    - [ ] Aumentar o salário do administrador.
    - [ ] Bloquear o acesso de estrangeiros.
    - [ ] Criar índices em todas as colunas.

    > **Explicação**: Permite modelar hierarquias, como Pessoa -> Pessoa Física / Pessoa Jurídica.

10. **Se uma tabela possui repetições propositais para evitar JOINs custosos, dizemos que ela está:**
    - [ ] Corrompida.
    - [ ] Super-normalizada.
    - [x] Desnormalizada.
    - [ ] Criptografada.
    - [ ] Em modo de manutenção.

    > **Explicação**: Desnormalizar é reinserir redundância controlada para otimizar a performance.