Este notebook Python, projetado para Google Colab, simula um SGBD com SQLite em um cenário de loja, gerenciando clientes, produtos e vendas.

Configuração do Banco de Dados
- Importa sqlite3 e os para manipulação.
- Cria loja.db, removendo versão anterior.

Criação de Tabelas
- Clientes**: id, nome, email.  
- Produtos**: id, nome_produto, preco.  
- Vendas**: id_venda, id_cliente, id_produto, quantidade, data_venda, com chaves estrangeiras.  
- Salva mudanças com conn.commit().

Inserção de Dados
- Registra clientes, produtos e vendas simuladas com data/hora atual.

 Consultas SQL
- Clientes: Retorna todos.  
- Produtos: Filtra por preco > R$200.  
- Vendas detalhadas: Usa JOIN para exibir cliente, produto e valor total.  
- Compras de um cliente: Lista produtos comprados por "Ana Silva".  
- Gasto total por cliente: Usa SUM e GROUP BY para ordenar por valor gasto.

Exibição dos Resultados
- Imprime diretamente no Google Colab.

Fechamento da Conexão
- Fecha conn.close() para liberar recursos e garantir persistência.
