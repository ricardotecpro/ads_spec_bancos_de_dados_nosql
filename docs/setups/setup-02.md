# Setup 02: MongoDB 🍃

O MongoDB é o banco de dados NoSQL líder de mercado, baseado em documentos JSON (BSON).

## 1. Instalação no Windows
1.  Acesse [mongodb.com/try/download/community](https://www.mongodb.com/try/download/community).
2.  Baixe o instalador `.msi` (versão Current).
3.  Execute o instalador e escolha o tipo **Complete**.
4.  Marque a opção **"Install MongoDB as a Service"**.
5.  Marque a opção **"Install MongoDB Compass"** (ferramenta visual).

## 2. MongoDB Shell (mongosh)
O shell não vem mais no instalador principal.
1.  Baixe o **MongoDB Shell** separadamente em [mongodb.com/try/download/shell](https://www.mongodb.com/try/download/shell).
2.  Extraia o arquivo e adicione a pasta `bin` ao seu PATH.

## 3. Verificação
1.  Abra o **MongoDB Compass**.
2.  Clique em **Connect** (a URL padrão é `mongodb://localhost:27017`).
3.  No terminal, teste:
    ```bash
    mongosh
    ```

## 4. Dica de Uso 💡
Diferente do SQL, você não precisa criar um banco de dados explicitamente antes de usá-lo; o MongoDB o cria automaticamente ao inserir o primeiro documento.