Developed by: Thiago Augusto

Prop�sito: fazer com que o aluno possa avaliar os agendamentos com uma nota de 1 a 5

A pasta functions lista todas as classes 
	connection.php = Respons�vel pela conex�o e m�todos com o banco de dados utilizando PDO
	agendamento.php = Respons�vel pelos atributos e m�todos de agendamento
	usuario.php = Respons�vel pelos atributos e m�todos do usu�rio


How to connect:
Acesse o arquivo connection.php que est� dentro da pasta functions e mude os atributos, respons�veis pela conex�o
Utilize o sistema FrenteEad para acessar a parte de avalia��o, pois o sistema utiliza sess�es para acessar o sistema de avalia��o
Dados pegos pelo sistema
Nome do usu�rio = $_SESSION['nome_usuario']
Tipo do usu�rio = $_SESSION['tipo_usuario']
Id do usu�rio = $_SESSION['id_usuario']

OBS: o usu�rio do tipo aluno somente avaliar� os agendamentos que forem agendados pelo mesmo
     o usu�rio do tipo funcion�rio somente poder� ver a m�dia de todos os agendamentos e outros dados gerais, ou escolher um usu�rio do tipo aluno atrav�s do e-mail e acessar os dados dos agendamentos gerais (m�dia, etc) do mesmo, e pode saber se o mesmo � chato ou n�o.