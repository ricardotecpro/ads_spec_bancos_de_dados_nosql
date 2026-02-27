# Quiz Aula 15 - Ecossistema Moderno e Cloud 🧠

Reforce sua visão profissional sobre arquitetura de dados e deploy NoSQL.

---

1. **O que é o MongoDB Atlas?**
    - [ ] Um mapa Mundi secreto do MongoDB.
    - [x] Um serviço gerenciado (DBaaS) de MongoDB na nuvem.
    - [ ] Uma ferramenta para desenhar tabelas SQL.
    - [ ] Um framework de front-end.
    - [ ] Um tipo de documento JSON.

    > **Explicação**: O Atlas gerencia a infraestrutura, permitindo que o desenvolvedor foque apenas nos dados.

2. **Qual a maior vantagem de uma "Arquitetura Poliglota"?**
    - [ ] Aprender várias línguas humanas.
    - [ ] Usar apenas um banco de dados para tudo.
    - [x] Usar o melhor banco de dados para cada necessidade específica do app.
    - [ ] Deixar o banco de dados mais colorido.
    - [ ] Economizar memória RAM do servidor.

    > **Explicação**: Em sistemas modernos, é comum usar SQL para finanças e NoSQL para catálogos ou logs.

3. **A segurança por "IP Whitelist" no Atlas serve para:**
    - [ ] Bloquear o banco de dados para todos.
    - [ ] Deixar o banco de dados mais rápido.
    - [x] Permitir acesso apenas de IPs conhecidos e autorizados.
    - [ ] Mudar o nome das coleções.
    - [ ] Criar um backup automático.

    > **Explicação**: Esta é uma camada de proteção essencial contra acessos não autorizados de hackers.

4. **Quando é recomendável NÃO usar NoSQL?**
    - [ ] Quando o banco é gratuito.
    - [ ] Quando os dados mudam muito.
    - [x] Quando os dados são ultra-relacionais e dependem de transações ACID complexas em várias tabelas.
    - [ ] Quando o aplicativo é para celular.
    - [ ] Quando o volume de dados é muito baixo.

    > **Explicação**: Para sistemas com regras de negócio muito rígidas e relacionais, o SQL ainda é o rei.

5. **A "Escalabilidade Horizontal" do NoSQL significa:**
    - [ ] Comprar um servidor maior e mais caro.
    - [x] Dividir os dados em vários servidores (clusters) menores e mais baratos.
    - [ ] Organizar os dados em ordem alfabética.
    - [ ] Mudar o banco de dados para o disco rígido.
    - [ ] Usar mais de um sistema operacional.

    > **Explicação**: É a capacidade de crescer "para os lados", adicionando mais máquinas conforme a demanda.

6. **O MongoDB Vector Search é focado em:**
    - [ ] Buscar nomes de cidades no mapa.
    - [ ] Calcular a velocidade de download.
    - [x] Aplicações de Inteligência Artificial e buscas por semelhança.
    - [ ] Somar valores das vendas do mês.
    - [ ] Ordenar resultados por data.

    > **Explicação**: Buscas vetoriais permitem encontrar dados parecidos através de representações matemáticas, ideal para IAs.

7. **Para conectar seu App ou Compass ao Atlas, você precisa de uma:**
    - [ ] Chave de fenda.
    - [ ] Nova instalação do Windows.
    - [x] Connection String (URL de conexão).
    - [ ] Senha do Gmail.
    - [ ] Licença da Microsoft.

    > **Explicação**: A connection string contém o protocolo, usuário, senha e o endereço do cluster na nuvem.

8. **Qual o custo de um cluster em nível "M0" (Sandbox) no MongoDB Atlas?**
    - [ ] $10 por mês.
    - [ ] $100 por ano.
    - [x] Gratuito (Forever Free).
    - [ ] $1 por dia.
    - [ ] Depende da velocidade da internet.

    > **Explicação**: O nível M0 é o plano gratuito ideal para estudantes e pequenos projetos.

9. **Em uma arquitetura moderna, onde o Redis costuma ser utilizado?**
    - [ ] Para salvar o banco de dados principal.
    - [x] Como camada de Cache para dados acessados com muita frequência e alta velocidade.
    - [ ] Para guardar fotos de perfil.
    - [ ] Para rodar relatórios mensais.
    - [ ] Como servidor de e-mail.

    > **Explicação**: Redis é um banco em memória ultra-veloz focado em cache e sessões.

10. **Qual a melhor prática de segurança ao usar o MongoDB Atlas em produção?**
    - [ ] Compartilhar a senha do admin no GitHub.
    - [ ] Não usar senhas nos clusters.
    - [x] Usar o Princípio do Menor Privilégio (usuário com acesso apenas a um banco específico).
    - [ ] Deixar a porta 27017 aberta para qualquer IP.
    - [ ] Reiniciar o banco toda semana.

    > **Explicação**: Garantir que cada aplicação tenha apenas as permissões necessárias para o seu funcionamento.