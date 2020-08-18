# TesteMutant
---------------------------
--- INSTRUÇÕES PARA USO ---
---------------------------

1 - Criar DB
	1.1 - Abra o SQL Server;
	1.2 - Nos arquivos do projeto, aba a pasta "SQL" e, execute o arquivo "CriaçãoDB.sql", ele irá criar o DB, as tabelas e alimentá-las;
	1.3 - Ainda na pasta "SQL", execute todos os outros arquivos. São os scripts utilizados para funcionamento do projeto.

2 - Cópia dos arquivos
	2.1 - As páginas estão em ASP, portanto, será necessário instalar o IIS no computador e, criar um diretório para o site;
	2.2 - Na pasta configurada, coloque todos os arquivos contidos na pasta do projeto (exceto pela pasta "SQL");
	2.3 - No arquivo "Funcoes.asp", será necessário editar a função "SqlServerOpen", colocando a instância do DB, login e senha.

3 - Utilização do projeto
	3.1 - No navegador, abra o arquivo "Index.asp". Ele será a página inicial do projeto;
	3.2 - O campo "ID Pedido" é preenchido automaticamente (conforme último pedido cadastrado no banco de dados);
	3.3 - Preencha o campo "Nome do Cliente";
	3.4 - Selecione o "Lanche";
	3.5 - Preencha os ingredientes adicionais (caso necessário);
		3.5.1 - Caso o ingrediente seja selecionado, porém não seja inserido um número maior que zero, o mesmo não será enviado para a próxima página;
		3.5.2 - Caso seja inserido um número no ingrediente, mas o mesmo não foi selecionado, o mesmo não será enviado para a próxima página;
		3.5.3 - Caso o lanche selecionado seja a opção "personalizado", é obrigatória a seleção de ao menos um ingrediente;
	3.6 - Clique no botão enviar;
	3.7 - Serão exibidas as informações do pedido e um link para voltar a tela de pedido.

------------------------------
--- OBSERVAÇÕES DO PROJETO ---
------------------------------

1 - Devido viagem que fiz e prioridade em relação a trabalhos do MBA, além de problemas com o javascript (por não conhecer muito bem a linguagem), não consegui implementar algumas funcionalidades. São elas:
	- Aplicação das regras de desconto;
	- Tratamento de SQL Injection / tratamento das informações;
	- Design melhorado.
