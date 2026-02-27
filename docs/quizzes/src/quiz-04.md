# Quiz Aula 04 - DDL (Criação da Estrutura) 🧠

Teste seus conhecimentos sobre comandos de criação e alteração de tabelas.

---

1. **Qual comando é usado para criar uma nova base de dados no PostgreSQL?**
    - [ ] `NEW DATABASE`
    - [ ] `MAKE DATABASE`
    - [x] `CREATE DATABASE`
    - [ ] `ADD DATABASE`
    - [ ] `BUILD DATABASE`

    > **Explicação**: `CREATE DATABASE` é o comando padrão DDL para iniciar um novo container de tabelas.

2. **O que significa a sigla DDL?**
    - [ ] Data Delivery Language.
    - [ ] Dynamic Data Link.
    - [x] Data Definition Language.
    - [ ] Database Design Layout.
    - [ ] Direct Data Loading.

    > **Explicação**: DDL é a parte do SQL que define as estruturas (Esquema) do banco.

3. **Qual a função da restrição `NOT NULL` em uma coluna?**
    - [ ] Permite que a coluna seja excluída a qualquer momento.
    - [ ] Garante que o valor seja sempre maior que zero.
    - [x] Impede que a coluna seja deixada em branco (sem valor).
    - [ ] Criptografa os dados daquela coluna.
    - [ ] Faz com que a coluna aceite apenas números.

    > **Explicação**: `NOT NULL` torna o preenchimento daquele campo obrigatório.

4. **Para que serve o tipo de dado `SERIAL` no PostgreSQL?**
    - [ ] Para guardar números de série de produtos.
    - [ ] Para indicar que os dados são transmitidos via conexão serial.
    - [x] Para criar automaticamente uma sequência numérica autoincrementada.
    - [ ] Para salvar arquivos de vídeo (séries).
    - [ ] Para limitar a tabela a apenas 100 linhas.

    > **Explicação**: `SERIAL` é um atalho que cria uma sequência e a associa à coluna (geralmente a PK).

5. **Qual comando exclui uma tabela e todos os seus dados permanentemente?**
    - [ ] `DELETE TABLE`
    - [ ] `REMOVE TABLE`
    - [x] `DROP TABLE`
    - [ ] `CLEAR TABLE`
    - [ ] `ERASE TABLE`

    > **Explicação**: `DROP TABLE` remove o objeto da estrutura do banco. Cuidado: não tem "Lixeira"!

6. **Diferente de `DROP`, o comando `TRUNCATE` faz o seguinte:**
    - [ ] Apaga apenas a estrutura e mantém os dados.
    - [x] Apaga todos os dados (linhas), mas mantém a estrutura da tabela vazia.
    - [ ] Muda o nome da tabela.
    - [ ] Cria uma cópia da tabela.
    - [ ] Compacta a tabela para economizar espaço.

    > **Explicação**: `TRUNCATE` é muito mais rápido que o `DELETE` comum para esvaziar tabelas grandes.

7. **Qual comando permite adicionar uma nova coluna a uma tabela já existente?**
    - [ ] `UPDATE TABLE`
    - [ ] `EXTEND TABLE`
    - [x] `ALTER TABLE`
    - [ ] `EXPAND TABLE`
    - [ ] `REVISE TABLE`

    > **Explicação**: `ALTER TABLE` é o comando para mudar definições de colunas, nomes ou restrições.

8. **A restrição `UNIQUE` em uma coluna garante que:**
    - [ ] O valor seja sempre igual a 1.
    - [ ] A coluna seja a chave primária.
    - [x] Não existam dois registros com o mesmo valor naquela coluna.
    - [ ] Apenas o administrador possa ver os dados.
    - [ ] O dado seja escrito em letras maiúsculas.

    > **Explicação**: Diferente da PK, uma tabela pode ter várias colunas `UNIQUE` (ex: CPF e Email).

9. **O que é um Índice (INDEX) no banco de dados?**
    - [ ] Uma lista de erros do sistema.
    - [ ] O número da página no manual do PostgreSQL.
    - [x] Uma estrutura que acelera a busca de registros em uma tabela.
    - [ ] Um backup em tempo real.
    - [ ] O ID do usuário que criou a tabela.

    > **Explicação**: Índices funcionam como sumários, permitindo localizar dados sem ler a tabela toda.

10. **A cláusula `CHECK` serve para:**
    - [ ] Verificar se o servidor está online.
    - [ ] Marcar uma tarefa como concluída.
    - [x] Validar se um valor atende a uma condição (ex: `idade >= 18`).
    - [ ] Conferir a senha do banco de dados.
    - [ ] Contar quantas linhas a tabela possui.

    > **Explicação**: `CHECK` garante a "regra de negócio" diretamente no nível do banco de dados.