
# Crie uma tebela contendo os seguintes itens :
LIVRO, AUTOR, SEXO,	PAGINAS, EDITORA, VALOR,UF, ANO

# 1 – Trazer todos os dados
comando utilizado: select * from livros;

# 2 – Trazer o nome do livro e o nome da editora
comando utilizado: SELECT LIVRO, EDITORA
FROM LIVROS;

# 3 - Trazer o nome do livro e a UF dos livros publicados por autores do sexo masculino
comando utilizado: SELECT AUTOR, SEXO,LIVRO, UF
FROM LIVROS
WHERE SEXO = 'M';

# 4 - Trazer o nome do livro e o número de páginas dos livros publicados por autores do sexo feminino
SELECT AUTOR,  LIVRO, PAGINAS
FROM LIVROS
WHERE SEXO = 'F';

# 5 - Trazer os valores dos livros das editoras de São Paulo
SELECT UF, LIVRO, VALOR
FROM LIVROS
WHERE UF = 'SP';
