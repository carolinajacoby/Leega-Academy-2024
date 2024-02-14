# Leega-Academy-2024 - DESAFIO 1

CONTEXTO

Dentro da política de expansão e geração de negócios, o Board de acionistas da Leega decidiu investir no setor de Varejo e Ecommerce. Para isto decidiu adquirir uma empresa que opera globalmente, a SupremEats, e após fechado o negócio, definiram que o novo nome será Leega Foods.
A nossa equipe de ciência de dados formada por analistas, engenheiros e cientistas de dados foi chamada para várias reuniões. Nelas tivemos oportunidade de conhecer esta operação e como estão montadas as soluções de tecnologia, mas, durante estas reuniões percebemos que empresa antiga não possuía uma solução de Analytics, e muito menos Ciência de Dados, e, para que possamos crescer ainda mais teremos que criar uma solução capaz de suportar a operação desta nova empresa e gerar importantes insights para nossos acionistas.
Toda operação está apoiada por um “ERP Caseiro” desenvolvido em Access (Microsoft) que foca em transações operacionais. Esta solução possui as seguintes bases:

1.	Categoria dos Produtos
2.	Clientes
3.	Funcionários
4.	Pedidos
5.	Detalhes dos Pedidos
6.	Produtos
7.	Transportadoras
8.	Fornecedores
9.	Países
E, a modelagem que existe nesta aplicação está disponível no ERP_SUPREMEATS.PDF
Com base nestas informações, o nosso trabalho será aplicar tudo o que aprendemos nos módulos e “operacionalizar” a solução de Analytics e Data Science da Leega Foods.


# MODULO 1

Agora que aprendemos sobre Arquitetura, como a Ciência de Dados transforma empresas, como resolvemos velhos problemas de novas formas e sobre os Frameworks existentes, nosso trabalho será montar uma visão da arquitetura que poderíamos utilizar na Leega Foods com 2 opções para apresentar ao board de diretores:
	 a 1ª utilizando o modelo on-premise
	a 2ª usando um modelo Cloud (IAAS, SAAS, PAAS). 
Isto é necessário para que eles possam selecionar qual das opções querem “implementar”, mas procure não ser tão técnico e ao mesmo tempo não ser tão superficial pois na sala tem executivos que são técnicos e outros que tem conhecimento mais de negócio!
Uma dica importante, devemos nos basear nas aulas acima e no PDF do ERP que dispomos, para que possamos criar esta arquitetura e com ela ter uma arquitetura que permita atender as necessidades de informação que eles possam necessitar e, também, gerar os insights importantes ao Board. 
E, finalmente devemos ao apresentar ao Board, explicar: 
1.	A visão de contexto;
2.	A visão funcional;
3.	A visão de implantação.
Deveremos, ainda, tocar e oferecer respostas as seguintes questões que poderiam surgir:
4.	Quais os velhos problemas que poderíamos resolver? E Por quê?
5.	Quais os pilares que foram levados em consideração na montagem desta arquitetura? E busque explicar o que cada um deles trará de benefícios e resultados a nova empresa (a Leega Foods)!
Vamos lá, este é o desafio. 


# Leega-Academy-2024 -Desafio 2- SQL 

# Contexto 

A Biblioteca Municipal do Estado foi inaugurada pelo governo, em 11 de dezembro de 1988. Inicialmente, atendia a zona central do município pela pequena quantidade de obras que tinha, mas o acervo inicial foi ampliado com a colaboração de várias entidades e cidadãos e hoje seu acervo ultrapassa mais de vinte mil obras e revistas.
A Biblioteca expandiu seu acervo e seus serviços. Foram criados os setores circulantes para o público infanto-juvenil e adultos, onde os mesmo poderiam ter um maior contato com as obras incentivando a leitura da população. O projeto de informatização foi totalmente implantado em 1999. No mesmo ano, foi instalada a sala de internet,com computadores para acesso à internet. Em razão da necessidade de um local melhor que atendesse a grande quantidade de usuários e o aumento do acervo, a biblioteca mudou de local e hoje está em um lugar mais adequado, o espaço passou por reforma e planejamento arquitetônico e foi inaugurada no dia 22 de setembro de 2012. Recentemente, nos conheceram e nos contrataram para criar a sua Base de Dados com informações cadastrais do acervo, usuário, funcionário, empréstimo e reserva. Esses dados eram armazenados em arquivos de pastas suspensas e com isso a biblioteca não tinha um controle eficiente das informações, a consulta do acervo, controle de reserva e empréstimo eram feitos manualmente. A Biblioteca trabalha com um sistema de empréstimo de livros no qual o usuário pode reservar ou retirar diversos livros para utilizar em um tempo determinado, caso a devolução seja feita depois da data estipulada a pessoa deverá pagar uma multa por atraso. Para que pudéssemos realizar o projeto a equipe da Bibliotecanos entregou um modelo lógico (imaginado por eles –veja ao lado) e um arquivo excel–”dados_biblioteca.csv” contendo algumas das informações a serem inseridas na Base de Dados para podermos testar a modelagem e testar a viabilidade das solicitações.

# informações passadas pelo cliente

![Modelo Lófico do Cliente ](https://github.com/carolinajacoby/Leega-Academy-2024/blob/main/Tabela%20Cliente%20SN.JPG?raw=true)


Durante a negociação do projeto, ficou acordado quefaremos: a melhor modelagem física baseada no modelo logico entregue (e caso encontremos erro a refaremos para garantir que a modelagem atenda todas as solicitações, carga destes dados reduzidos do arquivo Excel (em anexo), a criação da 1ª versão do dicionário de dados e os SQLspara as seguintes solicitações (que eles imaginaram):

1. A Diretora Camilla Prado solicitou uma pesquisa que informe todas as obras cadastradas no acervo ordenadas por data de publicação.
2.O Governador vai doar duzentos livros para a Biblioteca, mas só irá doar se a biblioteca tiver menos de 300 obras. O Gerente Márcio Tales solicitou que fosse feita a contagem de quantas obrasa Biblioteca possui atualmente.
3.A Gerência solicitou uma pesquisa para saber quais datas ocorreram empréstimos de livros e a quantidade emprestada. A consulta deverá retornar apenas um registro para cada data.
4.O Funcionário João Paulo Assistente de RH solicitou uma pesquisa que informasse todos os empréstimos que a Recepcionista Alice Meire fez no horário das 8hs às 9hs.Responda as seguintes query's após remodelar o banco do cliente.
5.A Gerência solicitou uma pesquisa para saber quais reservas de livros que foram feitas com data maior ou igual a 18/08/2021 que ainda possuem o status de “reservado”.
6.A área de RH solicitou uma pesquisa para saber quais devoluções de livros foram feitas antes de 29/03/2022.
7.O Funcionário João Paulo solicitou uma pesquisa para saber quantas obras do gênero ‘Ficção’ existem no acervo.
8.A Diretoria solicitou uma pesquisa para identificar qual o livro possuiu a maior quantidade em estoque, incluir respectiva editora e o respectivo autor.
9.O Financeiro precisa saber qual é o livro que possui a menor quantidade em estoque e quantas vezes ele foi emprestado para que seja feita uma análise para compra de mais alguns exemplares. A área de RH precisa identificar a quantidade total dos empréstimos feitos por cada funcionário ativos.
10.A Biblioteca recebeu a visita de um grupo de alunos, mas após a visita foi verificado desaparecimento de três livros, as obras que sumiram do acervo foram ‘Filho Nativo’, ‘Vidas Secas’ e ‘Dom Casmurro’, com isto será necessária a alteração da quantidade de livros no estoque de cada obra.
11.)A Recepcionista Claudia Cristina não conseguiu terminar o cadastro de cinco usuários que passaram pela Biblioteca, foi solicitado a inserção desses usuários.
11.1) Alfredo Tenttoni, Rua Amazonas 58, Pirai, 6549-5421, 02170-251, 294.264.875-32
11.2) Cindy Crall, Rua Ipiranga 123, Vila Cristal, 5846-6577, 02182-637, 122.147.655-49
11.3) Rubens Pardo, Avenida dos Monges 51, Campo Grande, 5184-8978, 52412-365, 654.586.472-98
11.4) Carlos Pracidelli, Travessa dos Irmãos 48, Cotia, 8945-7986, 23124-005, 341.251.651-75
11.5) Ernesto Coimbra, Avenida Ampére 414, Jardim Elvira, 5844-2654, 05728-368, 193.107.214-35
12. O Financeiro solicitou a inserção do valor individual de cada obra. Crie um campo com o nome Valor_Livro na tabela Obra. Defina o tipo de dados que poderá ser aceito e o valor de cada título.
13.A Consultoria verificou que o campo Multa_Atrasoestá com o tamanho Varchar(2), foi solicitada a alteração do campo para Varchar(3).
14.Foi verificado que o campo Multa_Atrasoestá com os registros preenchidos de forma errada, foi solicitada a alteração dos registros que forem 0 para Não e 1 para SIM.
15.A Diretoria solicitou a lista de todos os livros que já foram emprestados mas foram entregues com atraso e os respectivos os nomes dos funcionários que fizeram os empréstimos.
16.A Gerência solicitou a lista de todos os livros, cujos autores não são brasileiros, que já foram devolvidos e o valor total de cada livro. O Financeiro solicitou a lista de todas as obras que tiveram data de publicação menor que 04/03/2023, sua respectiva quantidade e o seu valor unitário.
17.A área de RH solicitou a lista de todos os funcionários separados por ativos ou não, seus respectivos cargos e salários.
18.A Diretoria solicitou a lista de todos os funcionários da Biblioteca com seus respectivos departamentos que tem idade entre 30 e 40 anos.
19.A Recepção solicitou uma lista com o código do livro, nome do livro cujo valor do livro seja maior que R$ 90,00.
20.A área de RH solicitou a atualização do salário do Auxiliar Financeiro de 12% sobre o seu salário atual. A Gerência solicitou uma lista de todas as Obras, que contenham a letra “C ordenadas por gênero data de publicação entre 2021 e 2023.
21.A Recepção solicitou uma lista como todos os funcionários da Biblioteca com código, nome, e departamento, classificado pelo nome do funcionário que não emprestaram nenhum livro. A Biblioteca solicitou uma lista que exiba a quantidade de logradouros de usuários agrupados por número do CEP.
22.A Diretoria solicitou uma lista que exiba a quantidade de endereços agrupados por usuário. Hoje é aniversario da biblioteca e para comemorar foram comprados presentes a todos os usuários que foram os primeiros a utilizar a biblioteca, o gerente Carlos mendes pediu a relação da primeira pessoa a reservar, pegar emprestado e devolver um livro e suas respectivas informações para que possa ser entrado em contato com ele.
23.Foi solicitado pela diretoria saber quantas obras cada editora tem na biblioteca.
24.Foi solicitado a informação de todos os usuários que morem em uma avenida, e ainda, que seja mostrado o nome do usuário, CPF e logradouro em ordem de CPF do maior para o menor.
25.Chegou na biblioteca uma mensagem urgente da Camila pedindo um relatório contendo a informação de todos os livros que foram emprestados mais de uma vez nos anos de 2011 a 2013 agrupados pelo nome do livro.
26.O Financeiro pediu para apresentar o valor médio dos livros e informar quais são os que estão abaixo dessa media, referente a devolução e empréstimo.
27.Carlos pediu que seja feita uma pesquisa informando de todos os usuários que tem cadastro na biblioteca e que nunca levaram livros mostrar o nome de todos em Maiúsculas.
28.A recepção pediu para verificar quais os usuários que já pegaram mais de 3 livros, e em caso positivo, mostrar nomes e quais livros, ordenando pelo CEP (crescente).
29.A diretoria pediu que fosse feito uma análise do estoque, apresentando uma lista com todos os livros que já foram reservados e emprestados e, mostrar quantos estão disponíveis classificados por Gênero.
30.A biblioteca foi comprar mais livros para aumentar seu acervo, mas a editora Saraiva aumentou em 16% o valor de seus livros, atualize os preços dos livros da editora na porcentagem designada.
31.Foi solicitado apresentarmos quais as 5 obras que tiveram menos publicações e as 5 de maior, ainda, mostrar qual o autor, editora, nome do livro e quantidade de publicações em ordem decrescente .
32.Fazem cento e noventa e três meses que o instituto bibliográfico brasileiro surgiu. Para comemorar a diretoria pediu a relação de todos os usuários que tem o cpfcom o começo 193 que receberão um presente de comemoração. Para isto, foi solicitado informar o nome e o cpfde todos os usuários que estejam nesse padrão mas mostrar cpfos 3 primeiros dígitos e os dois últimos os do meio apresentar um "*" como no exemplo: 193.***.***-35, lembrando que devemos apresentar dessa maneira, pois a diretoria quer preservar essas informações que são sigilosas.
