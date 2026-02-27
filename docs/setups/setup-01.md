# Setup 01: PostgreSQL 🐘

O PostgreSQL é um dos bancos de dados relacionais mais avançados e utilizados no mundo.

## 1. Instalação no Windows
1.  Acesse o site oficial: [postgresql.org/download/windows](https://www.postgresql.org/download/windows/).
2.  Clique em **Download the installer** (EDB).
3.  Escolha a versão mais recente (ex: 16 ou 17).
4.  Durante a instalação, certifique-se de marcar:
    *   PostgreSQL Server
    *   pgAdmin 4 (Interface Gráfica)
    *   Command Line Tools
5.  **IMPORTANTE**: Defina uma senha para o usuário `postgres` e **não a esqueça**.
6.  Mantenha a porta padrão `5432`.

## 2. Verificação
1.  Abra o **pgAdmin 4**.
2.  Conecte-se ao servidor local usando a senha definida.
3.  Abra o terminal (cmd ou powershell) e digite:
    ```bash
    psql --version
    ```

## 3. Configuração do Path (Opcional)
Para usar o `psql` em qualquer lugar do terminal:
1.  Adicione o caminho da pasta `bin` do PostgreSQL (ex: `C:\Program Files\PostgreSQL\16\bin`) às **Variáveis de Ambiente** do Windows.