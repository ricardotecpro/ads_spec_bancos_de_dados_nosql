# Quiz Aula 02 - Modelagem de Dados e Modelo E-R 🧠

Verifique sua compreensão sobre como projetar estruturas de bancos de dados.

---

1. **O que é uma "Entidade" no Modelo E-R?**
    - [ ] Uma linha de código em Python.
    - [ ] Um comando para apagar o banco de dados.
    - [x] Um objeto ou conceito do mundo real sobre o qual queremos armazenar dados.
    - [ ] A cor de fundo da interface do usuário.
    - [ ] Uma conexão de rede sem fio.

    > **Explicação**: Entidades representam "coisas" como Aluno, Carro ou Venda.

2. **Qual a função da Chave Primária (PK)?**
    - [ ] Ligar duas tabelas diferentes.
    - [ ] Armazenar o nome completo do usuário.
    - [x] Identificar de forma única e exclusiva cada registro em uma tabela.
    - [ ] Permitir que o banco de dados seja acessado pela internet.
    - [ ] Criptografar as senhas das tabelas.

    > **Explicação**: A PK garante que não existam linhas duplicadas e permite localizar um registro específico rapidamente.

3. **Para que serve a Chave Estrangeira (FK)?**
    - [ ] Para identificar o país de origem do banco de dados.
    - [x] Para estabelecer um relacionamento entre duas tabelas, apontando para a PK de outra.
    - [ ] Para criar cópias de segurança automáticas.
    - [ ] Para aumentar a velocidade de processamento de cálculos matemáticos.
    - [ ] Para definir o tipo de dado de uma coluna (inteiro ou texto).

    > **Explicação**: A FK é o elo de ligação entre entidades relacionadas.

4. **Um relacionamento onde um Cliente pode fazer vários Pedidos, mas cada Pedido pertence a apenas um Cliente, é do tipo:**
    - [ ] 1:1 (Um para Um)
    - [x] 1:N (Um para Muitos)
    - [ ] N:N (Muitos para Muitos)
    - [ ] N:1 (Vários para Um - do ponto de vista do Cliente)
    - [ ] Sem relacionamento.

    > **Explicação**: 1 Cliente -> N Pedidos. É o tipo de relacionamento mais comum.

5. **Em um relacionamento N:N (Muitos para Muitos), como o modelo relacional resolve a ligação?**
    - [ ] Colocando duas PKs na mesma tabela.
    - [ ] Criando uma coluna com uma lista de IDs.
    - [x] Criando uma terceira tabela (tabela associativa ou de ligação).
    - [ ] Não é possível fazer relacionamentos N:N em bancos SQL.
    - [ ] Apagando os dados duplicados automaticamente.

    > **Explicação**: Tabelas de ligação (ex: `Matriculas` ligando `Alunos` e `Disciplinas`) são essenciais para N:N.

6. **O que é "Integridade Referencial"?**
    - [ ] A velocidade com que os dados são lidos.
    - [ ] O tamanho total do arquivo do banco de dados.
    - [x] A regra que garante que as chaves estrangeiras sempre apontem para chaves primárias válidas.
    - [ ] A capacidade do banco de dados de rodar em qualquer sistema operacional.
    - [ ] O ato de fazer backup todos os dias.

    > **Explicação**: Impede o surgimento de "registros órfãos" (ex: um pedido sem cliente).

7. **Qual destes é um exemplo de Atributo?**
    - [ ] A tabela "Funcionários".
    - [x] O "Salário" de um funcionário.
    - [ ] O banco de dados "Empresa".
    - [ ] O SGBD PostgreSQL.
    - [ ] O diagrama de blocos.

    > **Explicação**: Atributos são as características (propriedades) das entidades.

8. **O que é um Diagrama Entidade-Relacionamento (DER)?**
    - [ ] Um código SQL pronto para rodar.
    - [ ] Uma planilha de Excel com dados.
    - [x] Uma representação gráfica da estrutura do banco de dados.
    - [ ] Um tutorial de como instalar o pgAdmin.
    - [ ] Uma lista de erros do sistema.

    > **Explicação**: O DER é a representação visual da modelagem lógica.

9. **Qual a cardinalidade entre "Carro" e "Placa" (considerando o padrão brasileiro)?**
    - [x] 1:1
    - [ ] 1:N
    - [ ] N:N
    - [ ] N:1
    - [ ] Não há relação.

    > **Explicação**: Um carro tem uma placa, e uma placa pertence a um único carro.

10. **A ferramenta dbdiagram.io é classificada como:**
    - [ ] Um SGBDR.
    - [ ] Um Sistema Operacional.
    - [x] Uma ferramenta CASE (Computer-Aided Software Engineering).
    - [ ] Um navegador de internet.
    - [ ] Um editor de vídeo.

    > **Explicação**: Ferramentas CASE auxiliam no design e engenharia de software/dados.
