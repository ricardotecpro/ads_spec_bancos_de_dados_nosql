# Projeto 15: Deploy e Segurança na Nuvem 🚀

**Objetivo**: Realizar o deploy de um banco de dados MongoDB na nuvem e configurar as camadas de segurança essenciais.

---

## 📝 O Desafio
Você deve levar o seu projeto "loja_nosql" da Aula 12 para o mundo real, utilizando o **MongoDB Atlas**.

## 🚀 Tarefas
1.  **Criação do Cluster**: Crie uma conta no MongoDB Atlas e configure um cluster gratuito (Plano M0).
2.  **Segurança**:
    *   Crie um usuário de banco com acesso de leitura e escrita.
    *   Adicione o seu IP atual na lista de permissões (Whitelist).
3.  **Migração**: Utilize o MongoDB Compass para exportar os dados do seu banco local e importar no cluster do Atlas.
4.  **Teste de Conexão**: Verifique se você consegue consultar os documentos na nuvem através do shell (`mongosh`) ou do próprio Compass.
5.  **Relatório de Arquitetura**: Escreva um pequeno texto explicando em qual provedor de nuvem (AWS, GCP ou Azure) o seu banco foi hospedado e por que a segurança por IP é necessária.

## ✅ Critérios de Entrega
*   A `connection string` do seu cluster (oculte a senha!).
*   Screenshot do painel do MongoDB Atlas mostrando o cluster ativo.
*   Screenshot dos dados visualizados no Compass via conexão Atlas.