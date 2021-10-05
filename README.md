# Via_Italia

--INCLUSÃO DE DADOS NAS TABELAS

SELECT * FROM TB_CLIENTE

INSERT INTO TB_CLIENTE VALUES ('Josué Junior', '30', 'xforest@gmail.com'),
							  ('Jorge Nelson','65','lopesjn@gmail.com'),
							  ('Cristina Oliveira', '25', 'oli.cristina@gmail.com'),
							  ('Jessica Carneiro','36', 'jess_carneiro@gmail.com'),
							  ('Priscila Souza', '32', 'pritty_souza@hotmail.com'),
							  ('Pedro Prado', '19','pp_prado@outlook.com'),
							  ('Samuel Lima', '44', 'samulima@gmail.com'),
							  ('Maciel Garcia', '78', 'macielgarcia_55@gmail.com'),
							  ('Flora Matos', '25', 'matos_flor@outlook.com'),
							  ('Fagundes Ramos', '36', 'fgundes_ramos@hotmail.com'),
							  ('Gustavo Lima', '18', 'lima_guto@terra.com'),
							  ('Sueli Costa', '45', 'susu_costa@gmail.com');

--resultado:

COD_CLIENTE	NOME	IDADE	EMAIL
1	Jorge Alencar	40	jorge.alencar@email.com.br
2	Amanda Tostão	35	amanda.tostao@email.com.br
3	Marcelo Silva	32	marcelo.silva@email.com.br
4	Rebeca Lopes	34	bekkaslopes@gmail.com
5	Josué Junior	30	xforest@gmail.com
6	Jorge Nelson	65	lopesjn@gmail.com
7	Cristina Oliveira	25	oli.cristina@gmail.com
8	Jessica Carneiro	36	jess_carneiro@gmail.com
9	Priscila Souza	32	pritty_souza@hotmail.com
10	Pedro Prado	19	pp_prado@outlook.com
11	Samuel Lima	44	samulima@gmail.com
12	Maciel Garcia	78	macielgarcia_55@gmail.com
13	Flora Matos	25	matos_flor@outlook.com
14	Fagundes Ramos	36	fgundes_ramos@hotmail.com
15	Gustavo Lima	18	lima_guto@terra.com
16	Sueli Costa	45	susu_costa@gmail.com

--atualizando o email de um registro

UPDATE TB_CLIENTE SET EMAIL = 'lima_gutto@terra.com.br' WHERE COD_CLIENTE = 15
SELECT * FROM TB_CLIENTE

1	Jorge Alencar	40	jorge.alencar@email.com.br
2	Amanda Tostão	35	amanda.tostao@email.com.br
3	Marcelo Silva	32	marcelo.silva@email.com.br
4	Rebeca Lopes	34	bekkaslopes@gmail.com
5	Josué Junior	30	xforest@gmail.com
6	Jorge Nelson	65	lopesjn@gmail.com
7	Cristina Oliveira	25	oli.cristina@gmail.com
8	Jessica Carneiro	36	jess_carneiro@gmail.com
9	Priscila Souza	32	pritty_souza@hotmail.com
10	Pedro Prado	19	pp_prado@outlook.com
11	Samuel Lima	44	samulima@gmail.com
12	Maciel Garcia	78	macielgarcia_55@gmail.com
13	Flora Matos	25	matos_flor@outlook.com
14	Fagundes Ramos	36	fgundes_ramos@hotmail.com
15	Gustavo Lima	18	lima_gutto@terra.com.br
16	Sueli Costa	45	susu_costa@gmail.com

--UPDATE E INSERT NA TABELA TB_PRODUTO

COD_PRODUTO	DESCRICAO	VALOR	SITUACAO
1	Fettuccine	20.00	A
2	Lasanha	18.00	A
3	Ravioli	21.00	A
4	Risoto	20.00	A
5	Nhoque 	16.00	A

--ALTER NA COLUNA DESCRICAO

ALTER TABLE tb_produto 
ALTER COLUMN DESCRICAO VARCHAR (50) 

UPDATE TB_PRODUTO 
SET DESCRICAO = 'Fettuccine com Skitake e Rúcula' 
where COD_PRODUTO = 1
UPDATE TB_PRODUTO 
SET DESCRICAO = 'Lasanha Quatro Queijos' 
where COD_PRODUTO = 2
UPDATE TB_PRODUTO 
SET DESCRICAO = 'Ravioli à Fiorentina' 
where COD_PRODUTO = 3
UPDATE TB_PRODUTO 
SET DESCRICAO = 'Risoto del Mare'
where COD_PRODUTO = 4
UPDATE TB_PRODUTO 
SET DESCRICAO = 'Nhoque ao Sugo di Pomodoro'
where COD_PRODUTO = 5
select * from TB_PRODUTO

COD_PRODUTO	DESCRICAO	VALOR	SITUACAO
1	Fettuccine com Skitake e Rúcula	20.00	A
2	Lasanha Quatro Queijos	18.00	A
3	Ravioli à Fiorentina	21.00	A
4	Risoto del Mare	20.00	A
5	Nhoque ao Sugo di Pomodoro	16.00	A

INSERT INTO TB_PRODUTO VALUES('Spaghetti com Frutos do Mar','67', 'A'),
							 ('Fusili Calabresi', '58','A'),
							 ('Penne Alla Diavola', '56','A'),
							 ('Ravioli di Formaggio di Cabra', '58','A'),
							 ('Lasanha Calabeccia','59','A'),
							 ('Spaghetti Quatro Queijos','49','A'),
							 ('Fusili com Brasiola','59','A'),
							 ('Filé à Fiorentina','69', 'A'),
							 ('Filé à Parmegiana','68','A');
               
select * from TB_PRODUTO

COD_PRODUTO	DESCRICAO	VALOR	SITUACAO
1	Fettuccine com Skitake e Rúcula	20.00	A
2	Lasanha Quatro Queijos	18.00	A
3	Ravioli à Fiorentina	21.00	A
4	Risoto del Mare	20.00	A
5	Nhoque ao Sugo di Pomodoro	16.00	A
6	Spaghetti com Frutos do Mar	67.00	A
7	Fusili Calabresi	58.00	A
8	Penne Alla Diavola	56.00	A
9	Ravioli di Formaggio di Cabra	58.00	A
10	Lasanha Calabeccia	59.00	A
11	Spaghetti Quatro Queijos	49.00	A
12	Fusili com Brasiola	59.00	A
13	Filé à Fiorentina	69.00	A
14	Filé à Parmegiana	68.00	A
