INSERT INTO Cliente (nome, telefone, email, endereco) 
VALUES ('João Silva', '11987654321', 'joao@gmail.com', 'Rua A, 123');

INSERT INTO Veiculo (modelo, ano, placa, id_cliente) 
VALUES ('Toyota Corolla', 2020, 'ABC-1234', 1);

INSERT INTO Mecanico (nome, endereco, especialidade) 
VALUES ('Carlos Souza', 'Rua B, 456', 'Freios');

INSERT INTO Servico (descricao, preco) 
VALUES ('Troca de óleo', 150.00), ('Alinhamento', 200.00);

INSERT INTO Peca (nome, preco) 
VALUES ('Filtro de óleo', 30.00), ('Pneu 15"', 250.00);

INSERT INTO OrdemServico (numero, data_emissao, valor, status, data_conclusao, id_veiculo, id_mecanico) 
VALUES ('OS001', CURDATE(), 500.00, 'Em andamento', NULL, 1, 1);

INSERT INTO OrdemServico_Servico (id_os, id_servico) 
VALUES (1, 1), (1, 2);
