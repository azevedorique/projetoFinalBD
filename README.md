# projetoFinalBD
Projeto Final de Banco de Dados


TRIGGERS: 

Para esse projeto, implementamos dois triggers no banco de dados. O Primeiro é acionado
logo após a inserção de um novo elemento na tabela Pedido. A Cada adição nessa tabela, o
atributo Quant_para_venda do livro envolvido no pedido terá seu valor reduzido em 1. O segundo
trigger atua antes da inserção e verifica se existem livros disponíveis para compra antes de
permitir a inserção na tabela Pedido. Caso não tenha nenhum livro disponível, ele impedirá a 
adição do elemento e retornará uma mensagem de erro.

STORED PROCEDURES:

Criamos dois stored procedures. O primeiro faz o cálculo do total de livros vendidos e o
segundo faz a inserção de elementos na tabela livros.

VIEWS:

Criamos duas views: Uma mostra os livros separados por tipo e a outra confere os valores
dos livros e os corrije se for necessário.

SEGURANÇA:

Para garantir a segurança do banco de dados, criamos dois usuários com permissões específicas
com diferentes níveis de acesso. Um usuário administrador que pode acessar e modificar todos 
os dados e um usuário de leitura que pode apenas visualizar os dados. Também implementamos uma
tabela de controle de acesso que define quais usuários tem permissão para realizar determinadas
operações, além de triggers para inserir, atualizar e deletar dados da tabela livros.

NORMALIZAÇÃO: 

Para colocar o nosso esquema na terceira forma normal realizamos as seguintes mudanças:

*Adicionamos uma chave primária para a entidade Biblioteca;
*Criamos uma tabela Nacionalidade e a referenciamos na tabela Autor por meio de uma chave estrangeira;
*Trocamos a chave primária da entidade Pagamento

CRUD:

Para criar o CRUD, criamos uma API usando o framework Node.js e implementamos as seguintes operações:

Visualizar a tabela livros, ou apenas um elemento dela,
Inserir elementos na tabela Disciplina,
Alterar elementos na tabela Aluno,
Excluir elementos da tabela Professor.

GRUPO : Henrique Guerra e Mateus Falcão
