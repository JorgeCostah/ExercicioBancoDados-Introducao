ista de Exercícios – Banco de Dados (SQLite) 
Parte 1: Criando e Manipulando Tabelas 
1
 ️ Criação de uma Tabela 
Crie uma tabela chamada "clientes" com os seguintes campos: 
• id (inteiro, chave primária e autoincrementado) 
• nome (texto, obrigatório) 
• email (texto, único) 
• idade (inteiro) 
Dica: Utilize CREATE TABLE. 
2
 ️. Inserindo Registros 
Insira 10 clientes diferentes na tabela criada no exercício anterior. 
Dica: Utilize INSERT INTO. 
3
 ️. Selecionando Todos os Dados 
Recupere e exiba todos os clientes cadastrados na tabela. 
Dica: Utilize SELECT * FROM clientes;. 
4
 ️ Filtrando por Idade 
Liste todos os clientes que tenham idade maior que 25 anos. 
Dica: Use WHERE. 
5
 ️ Ordenando Registros 
Liste os clientes ordenados em ordem alfabética pelo nome. 
Dica: Use ORDER BY nome ASC. 
6
 ️ Atualizando Dados 
Atualize o email de um cliente específico na tabela. 
Dica: Utilize UPDATE. 
7
 ️ Removendo um Cliente 
Apague um cliente da tabela utilizando o ID dele. 
Dica: Utilize DELETE FROM. 
8
 ️ Criando Outra Tabela 
Crie uma tabela chamada "pedidos" com os seguintes campos: 
• id (inteiro, chave primária e autoincrementado) 
• cliente_id (inteiro, relacionado à tabela clientes) 
• valor (real, obrigatório) 
• data_pedido (data, obrigatório) 
Dica: Use FOREIGN KEY para ligar cliente_id a id da tabela clientes. 
9
 ️ Inserindo Pedidos 
Adicione 10 pedidos diferentes à tabela "pedidos", cada um associado a um cliente existente. 
Dica: Utilize INSERT INTO. 
// No momento não responder está questão:  
10 Listando Pedidos e Clientes 
Liste os pedidos e os nomes dos clientes que os fizeram. 
Dica: Use JOIN. 
Parte 2: Consultas e Funções SQL 
1
 ️1️ Filtrando Pedidos 
Recupere todos os pedidos com valor acima de 100 reais. 
Dica: Use WHERE. 
1
 ️2️ Contando Clientes 
Conte quantos clientes estão cadastrados na tabela clientes. 
Dica: Use COUNT(*). 
1
 ️3️ Valor Médio dos Pedidos 
Calcule a média dos valores dos pedidos feitos pelos clientes. 
Dica: Use AVG(). 
1
 ️4 Pedido Mais Caro 
Recupere o pedido mais caro já feito. 
Dica: Use MAX(valor). 
1
 ️5 Pedidos Feitos por um Cliente 
Liste todos os pedidos feitos por um cliente específico. 
Dica: Use WHERE cliente_id = ?. 
1
 ️6 Clientes sem Pedidos 
Liste todos os clientes que ainda não fizeram nenhum pedido. 
Dica: Use LEFT JOIN e IS NULL. 
1
 ️8️ Quantidade de Pedidos por Cliente 
Mostre quantos pedidos cada cliente fez. 
Dica: Use GROUP BY. 
1
 ️9 Soma dos Valores de Pedidos por Cliente 
Mostre o total gasto por cada cliente. 
Dica: Use SUM(valor). 
2
 ️0 Clientes com Mais de um Pedido 
Liste os clientes que fizeram mais de um pedido. 
Dica: Use HAVING COUNT(cliente_id) > 1️. 
2
 ️0 Deletando Todos os Pedidos 
Exclua todos os pedidos da tabela pedidos. 
Dica: Use DELETE FROM pedidos. 
Parte 3: Projetos Práticos 
Projeto: Sistema de Biblioteca            
Crie um sistema de gerenciamento de livros e empréstimos no SQLite. 
Você deve criar: 
• Uma tabela livros com id, titulo e autor. 
• Uma tabela emprestimos com id, livro_id, cliente_id e data_emprestimo. 
• Insira pelo menos 5 livros e 3 empréstimos. 
• Liste quais livros estão emprestados e para quem. 
2
 ️2️ Projeto: Cadastro de Produtos e Vendas       
Crie um sistema de vendas de produtos utilizando SQLite. 
Você deve criar: 
• Uma tabela produtos com id, nome, preco e estoque. 
• Uma tabela vendas com id, produto_id, quantidade, data_venda. 
• Insira pelo menos 5 produtos e 3 vendas. 
• Liste quais produtos foram vendidos e o total arrecadado. 
