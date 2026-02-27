# Quiz Aula 01 - Introdução a Bancos de Dados 🧠

Teste seus conhecimentos sobre os fundamentos de dados, informação e SGBDs.

---

1. **O que melhor define um "Dado" no contexto de computação?**
    - [ ] Uma mensagem contextualizada que transmite conhecimento.
    - [ ] Um elemento bruto e isolado que, por si só, não tem significado completo.
    - [ ] O resultado final de um processamento de inteligência artificial.
    - [ ] Um comando SQL pronto para ser executado.
    - [x] Um elemento bruto e isolado que, por si só, não tem significado completo.

    > **Explicação**: Dados são os componentes básicos, como números ou nomes soltos. Quando processados e contextualizados, tornam-se informação.

2. **Qual a principal diferença entre Dado e Informação?**
    - [ ] Não há diferença, são sinônimos.
    - [ ] Dado é digital, informação é analógica.
    - [x] Informação é o dado processado e contextualizado que gera sentido.
    - [ ] Dado é o que o usuário digita, informação é o que o banco apaga.
    - [ ] Informação é a soma de todos os bits de um disco rígido.

    > **Explicação**: A informação é o resultado do processamento de dados para gerar conhecimento ou suporte à decisão.

3. **Quem propôs o Modelo Relacional na década de 1970?**
    - [ ] Bill Gates
    - [ ] Steve Jobs
    - [x] Edgar F. Codd
    - [ ] Linus Torvalds
    - [ ] Ada Lovelace

    > **Explicação**: E.F. Codd, pesquisador da IBM, publicou o artigo que fundamentou as bases do modelo relacional baseado em relações (tabelas).

4. **O que significa a sigla SGBDR?**
    - [ ] Sistema de Gerenciamento de Busca de Dados Rápidos.
    - [ ] Servidor Geral de Banco de Dados Remoto.
    - [x] Sistema Gerenciador de Banco de Dados Relacional.
    - [ ] Software de Gravação de Bits e Dados Reais.
    - [ ] Site de Gestão de Banco de Dados de Rede.

    > **Explicação**: SGBDR é o software (como PostgreSQL ou MySQL) responsável por gerenciar bases de dados organizadas em tabelas.

5. **Na arquitetura Cliente/Servidor do PostgreSQL, o pgAdmin é considerado um:**
    - [ ] Servidor de aplicação.
    - [ ] Banco de dados físico.
    - [x] Cliente (interface de usuário).
    - [ ] Protocolo de rede.
    - [ ] Driver de impressora.

    > **Explicação**: O pgAdmin é uma ferramenta cliente que se conecta ao processo servidor do PostgreSQL para enviar comandos.

6. **Qual das opções abaixo é um exemplo de SGBD NoSQL?**
    - [ ] PostgreSQL
    - [ ] MySQL
    - [x] MongoDB
    - [ ] SQL Server
    - [ ] Oracle

    > **Explicação**: MongoDB é um banco de dados não relacional (NoSQL) que armazena dados em documentos, ao contrário dos outros citados.

7. **Qual é um dos principais problemas de guardar dados em "Arquivos Planos" (TXT/CSV)?**
    - [ ] São muito rápidos para buscar milhões de registros.
    - [x] Dificuldade em manter a integridade e segurança dos dados.
    - [ ] Suportam transações ACID nativas.
    - [ ] Impedem que os dados sejam lidos por seres humanos.
    - [ ] São formatos proprietários muito caros.

    > **Explicação**: Arquivos planos não oferecem mecanismos nativos de busca eficiente, concorrência ou proteção contra dados corrompidos.

8. **A porta padrão de comunicação do PostgreSQL é:**
    - [ ] 80
    - [ ] 3306
    - [ ] 27017
    - [x] 5432
    - [ ] 8080

    > **Explicação**: A porta 5432 é a porta padrão onde o servidor PostgreSQL "ouve" as requisições dos clientes.

9. **O modelo de dados que organiza as informações em tabelas com linhas e colunas é o:**
    - [ ] Modelo Hierárquico.
    - [ ] Modelo de Documentos.
    - [x] Modelo Relacional.
    - [ ] Modelo de Grafos.
    - [ ] Modelo de Chave-Valor.

    > **Explicação**: O diferencial do modelo relacional é justamente o uso de tabelas (relações) interconectadas.

10. **Qual a função do usuário `postgres` criado durante a instalação?**
    - [ ] É um usuário comum sem permissões.
    - [ ] Serve apenas para ler dados, sem poder gravar.
    - [ ] É o desenvolvedor que criou o software.
    - [x] É o superusuário (administrador) com plenos poderes no banco.
    - [ ] É um vírus que deve ser removido.

    > **Explicação**: O usuário `postgres` é o administrador padrão do sistema, possuindo controle total sobre todas as bases de dados do servidor.