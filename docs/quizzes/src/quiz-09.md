# Quiz Aula 09 - Transações e Integridade ACID 🧠

Teste seus conhecimentos sobre como o banco de dados garante que os dados nunca se percam ou fiquem errados.

---

1. **O que é uma "Transação" no contexto de bancos de dados?**
    - [ ] Uma venda realizada em dinheiro.
    - [ ] Um backup que é movido para outro servidor.
    - [x] Uma unidade de trabalho que deve ser executada totalmente ou não ser executada.
    - [ ] O ato de trocar o nome das tabelas.
    - [ ] Uma conexão de rede entre o cliente e o servidor.

    > **Explicação**: Transações garantem a integridade do conjunto de operações.

2. **Qual comando finaliza uma transação, salvando todas as alterações permanentemente?**
    - [ ] `SAVE`
    - [ ] `FINISH`
    - [x] `COMMIT`
    - [ ] `DONE`
    - [ ] `EXIT`

    > **Explicação**: Somente após o `COMMIT` os outros usuários podem ver as alterações e elas se tornam duráveis.

3. **Para desfazer todas as alterações de uma transação que ainda não foi confirmada, usamos:**
    - [ ] `UNDO`
    - [ ] `DELETE`
    - [ ] `CANCEL`
    - [x] `ROLLBACK`
    - [ ] `REVERT`

    > **Explicação**: O `ROLLBACK` volta o banco ao estado exato em que estava antes do `BEGIN`.

4. **Na sigla ACID, o que significa a "Atomicidade"?**
    - [ ] Que o banco de dados usa energia nuclear.
    - [x] Que a transação é tratada como uma unidade indivisível (tudo ou nada).
    - [ ] Que os dados são muito pequenos.
    - [ ] Que o banco só funciona em servidores de alta performance.
    - [ ] Que cada linha tem um ID atômico.

    > **Explicação**: Ou todos os comandos da transação funcionam, ou nenhum deles é aplicado.

5. **A propriedade "Consistência" (C do ACID) garante que:**
    - [ ] O banco nunca fique offline.
    - [ ] Os dados sejam salvos em ordem alfabética.
    - [x] O banco de dados passe de um estado válido para outro, respeitando todas as regras.
    - [ ] Todas as senhas sejam iguais.
    - [ ] O tamanho do banco seja constante.

    > **Explicação**: Impede que transações deixem dados que violem restrições (como chaves estrangeiras ou CHECKs).

6. **O que a propriedade "Isolamento" (I do ACID) evita?**
    - [ ] Que o servidor pegue vírus.
    - [ ] Que o banco de dados seja acessado pela internet.
    - [x] Que transações simultâneas interfiram umas nas outras antes de terminar.
    - [ ] Que o banco ocupe muito espaço em disco.
    - [ ] Que o usuário acesse a tabela de outro usuário.

    > **Explicação**: Garante que o resultado final de transações paralelas seja o mesmo de se tivessem ocorrido uma após a outra.

7. **A "Durabilidade" (D do ACID) significa que:**
    - [ ] O banco de dados vai durar muitos anos.
    - [ ] O hardware do servidor é resistente.
    - [x] Uma vez que o COMMIT aconteceu, os dados não se perdem mesmo em queda de energia.
    - [ ] O usuário não pode apagar os dados.
    - [ ] O sistema é difícil de quebrar.

    > **Explicação**: Garante a persistência dos dados em armazenamento não volátil.

8. **Qual o comando usado para iniciar manualmente uma transação no PostgreSQL?**
    - [ ] `START`
    - [x] `BEGIN`
    - [ ] `GO`
    - [ ] `TRANSACTION ON`
    - [ ] `INIT`

    > **Explicação**: `BEGIN` marca o ponto de partida de uma unidade lógica de trabalho.

9. **Para que serve o comando `SAVEPOINT`?**
    - [ ] Para salvar o banco de dados em um HD externo.
    - [ ] Para marcar o final da transação.
    - [x] Para criar um ponto de restauração intermediário dentro de uma transação longa.
    - [ ] Para definir qual usuário pode ver o dado.
    - [ ] Para pausar o banco de dados por alguns segundos.

    > **Explicação**: Você pode dar um `ROLLBACK TO savepoint_name` sem cancelar a transação inteira.

10. **Em qual cenário a transação é MAIS CRÍTICA?**
    - [ ] Mudança na cor de fundo do site.
    - [ ] Consulta da previsão do tempo.
    - [x] Transferência bancária entre contas de clientes diferentes.
    - [ ] Download de uma imagem de perfil.
    - [ ] Listagem de nomes em ordem alfabética.

    > **Explicação**: Onde a falha parcial (ex: tirar dinheiro de um e não colocar no outro) gera prejuízo ou erro grave.