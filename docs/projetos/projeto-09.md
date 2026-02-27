# Projeto 09: Simulação de Transações Bancárias 🔑

**Objetivo**: Implementar o controle de transações para garantir a consistência de dados em operações financeiras.

---

## 📝 O Desafio
Você deve simular o sistema de transferências de um banco digital. Existem duas tabelas: `contas` (id, cliente, saldo) e `historico_transferencias` (id, origem_id, destino_id, valor, data).

## 🚀 Tarefas
Escreve o script SQL para realizar uma transferência de R$ 300,00 de "Ana" para "Bia":
1.  Inicie a transação (`BEGIN`).
2.  Verifique se Ana tem saldo (apenas via comentário ou lógica simples).
3.  Subtraia o valor da conta da Ana.
4.  Adicione o valor na conta da Bia.
5.  Insira o registro no histórico.
6.  **Simulação de Falha**: Imagine que o sistema de histórico caiu. Execute um `ROLLBACK` e verifique os saldos.
7.  **Finalização**: Repita o processo, mas finalize com `COMMIT`.

## ✅ Critérios de Entrega
*   O script `.sql` contendo os dois blocos (o que falha e o que funciona).
*   Print do saldo das contas antes e depois de cada operação.