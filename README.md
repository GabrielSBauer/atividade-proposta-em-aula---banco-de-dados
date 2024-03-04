# atividade-proposta-em-aula---banco-de-dados
crair um database e realizar algumas atividades


oque foi feito no banco.

CREATE DATABASE lista_de_contato; //cria o database 

use lista_de_contatos; //acessa o database


//cria a tabela contatos dentro do database

CREATE TABLE contatos (
id INT AUTO_INCREMENT PRIMARY KEY,
nome VARCHAR(255) NOT NULL,
telefone VARCHAR(20),
email VARCHAR(255),
grupo VARCHAR(50)
);


// adiciona a coluna favorito que esqueci de adicionar!

ALTER TABLE contatos
ADD COLUMN favorito BOOLEAN DEFAULT FALSE;



//adiciona contatos ficticios gerados por ia

INSERT INTO contatos (nome, telefone, email, grupo) VALUES 
('Rafaela Oliveira', '10101010101', 'rafaela@example.com', 'Trabalho'),
('João Pereira', '11111111111', 'joao2@example.com', 'Amigos'),
('Mariana Rodrigues', '12121212121', 'mariana5@example.com', 'Família'),
('Lucas Costa', '13131313131', 'lucas6@example.com', 'Trabalho'),
('Laura Martins', '14141414141', 'laura6@example.com', 'Amigos'),
('Gabriel Pereira', '15151515151', 'gabriel7@example.com', 'Família'),
('Ana Silva', '16161616161', 'ana3@example.com', 'Trabalho'),
('Carlos Santos', '17171717171', 'carlos3@example.com', 'Amigos'),
('Fernanda Oliveira', '18181818181', 'fernanda5@example.com', 'Família'),
('Marcos Carvalho', '19191919191', 'marcos5@example.com', 'Trabalho'),
('Camila Pereira', '20202020202', 'camila5@example.com', 'Amigos'),
('Gabriel Rodrigues', '21212121212', 'gabriel8@example.com', 'Família'),
('Isabela Silva', '22222222222', 'isabela5@example.com', 'Trabalho'),
('Leonardo Santos', '23232323232', 'leonardo5@example.com', 'Amigos'),
('Amanda Oliveira', '24242424242', 'amanda5@example.com', 'Família'),
('Lucas Martins', '25252525252', 'lucas7@example.com', 'Trabalho'),
('Laura Costa', '26262626262', 'laura7@example.com', 'Amigos'),
('Gabriel Pereira', '27272727272', 'gabriel9@example.com', 'Família'),
('Mariana Almeida', '28282828282', 'mariana6@example.com', 'Trabalho'),
('Pedro Rodrigues', '29292929292', 'pedro5@example.com', 'Amigos'),
('Tatiane Santos', '30303030303', 'tatiane5@example.com', 'Família'),
('Diego Oliveira', '31313131313', 'diego5@example.com', 'Trabalho'),
('Sara Pereira', '32323232323', 'sara5@example.com', 'Amigos'),
('André Costa', '33333333333', 'andre5@example.com', 'Família'),
('Vanessa Sousa', '34343434343', 'vanessa5@example.com', 'Trabalho'),
('Rafael Martins', '35353535353', 'rafael5@example.com', 'Amigos'),
('Fernanda Almeida', '36363636363', 'fernanda6@example.com', 'Família'),
('Marcos Carvalho', '37373737373', 'marcos6@example.com', 'Trabalho'),
('Camila Pereira', '38383838383', 'camila6@example.com', 'Amigos'),
('Gabriel Rodrigues', '39393939393', 'gabriel10@example.com', 'Família'),
('Isabela Silva', '40404040404', 'isabela6@example.com', 'Trabalho'),
('Leonardo Santos', '41414141414', 'leonardo6@example.com', 'Amigos'),
('Amanda Oliveira', '42424242424', 'amanda6@example.com', 'Família'),
('Lucas Martins', '43434343434', 'lucas8@example.com', 'Trabalho'),
('Laura Costa', '44444444444', 'laura8@example.com', 'Amigos'),
('Gabriel Pereira', '45454545454', 'gabriel11@example.com', 'Família'),
('Mariana Almeida', '46464646464', 'mariana7@example.com', 'Trabalho'),
('Pedro Rodrigues', '47474747474', 'pedro6@example.com', 'Amigos'),
('Tatiane Santos', '48484848484', 'tatiane6@example.com', 'Família'),
('Diego Oliveira', '49494949494', 'diego6@example.com', 'Trabalho'),
('Sara Pereira', '50505050505', 'sara6@example.com', 'Amigos'),
('André Costa', '51515151515', 'andre6@example.com', 'Família'),
('Vanessa Sousa', '52525252525', 'vanessa6@example.com', 'Trabalho'),
('Rafael Martins', '53535353535', 'rafael6@example.com', 'Amigos'),
('Fernanda Almeida', '54545454545', 'fernanda7@example.com', 'Família'),
('Marcos Carvalho', '55555555555', 'marcos7@example.com', 'Trabalho'),
('Camila Pereira', '56565656565', 'camila7@example.com', 'Amigos');

// altera os dados do 

UPDATE contatos
SET nome = 'Bauer',
    email = 'bauer@Bauer.com',
    grupo = 'familia',
    favorito = TRUE
WHERE id = 1;

UPDATE contatos
SET nome = 'caique',
    email = 'bocamino@unip.com',
    grupo = 'faculdade',
    favorito = TRUE
WHERE id = 2;

UPDATE contatos
SET nome = 'igor',
    email = 'igor@unip.com',
    grupo = 'faculdade',
    favorito = TRUE
WHERE id = 3;

UPDATE contatos
SET nome = 'bruno',
    email = 'brunao@unip.com',
    grupo = 'faculdade',
    favorito = TRUE
WHERE id = 4;

UPDATE contatos
SET nome = 'felipe',
    email = 'felipe@unip.com',
    grupo = 'faculdade',
    favorito = TRUE
WHERE id = 5;

UPDATE contatos
SET nome = 'luiz',
    email = 'luiz.aluno@unip.com',
    grupo = 'faculdade',
    favorito = TRUE
WHERE id = 6;

UPDATE contatos
SET nome = 'luan',
    email = 'luan@unip.com',
    grupo = 'faculdade',
    favorito = TRUE
WHERE id = 7;

UPDATE contatos
SET nome = 'joaozinho',
    email = 'joaodapedra@gmail.com',
    grupo = 'tabalho',
    favorito = TRUE
WHERE id = 8;

UPDATE contatos
SET nome = 'marcelao',
    email = 'marcela.gomes@unip.com',
    grupo = 'professor',
    favorito = TRUE
WHERE id = 9;

UPDATE contatos
SET nome = 'daniela',
    email = 'daniela@unip.com',
    grupo = 'professor',
    favorito = TRUE
WHERE id = 10;

//fazer buscas 

select * from contatos
where favorito = true;
//contatos favoritos
+----+-----------+-----------+------------------------+-----------+----------+
| id | nome      | telefone  | email                  | grupo     | favorito |
+----+-----------+-----------+------------------------+-----------+----------+
|  1 | Bauer     | 123456789 | bauer@Bauer.com        | familia   |        1 |
|  2 | caique    | 987654321 | bocamino@unip.com      | faculdade |        1 |
|  3 | igor      | 555555555 | igor@unip.com          | faculdade |        1 |
|  4 | bruno     | 111111111 | brunao@unip.com        | faculdade |        1 |
|  5 | felipe    | 222222222 | felipe@unip.com        | faculdade |        1 |
|  6 | luiz      | 333333333 | luiz.aluno@unip.com    | faculdade |        1 |
|  7 | luan      | 444444444 | luan@unip.com          | faculdade |        1 |
|  8 | joaozinho | 555555555 | joaodapedra@gmail.com  | tabalho   |        1 |
|  9 | marcelao  | 666666666 | marcela.gomes@unip.com | professor |        1 |
| 10 | daniela   | 777777777 | daniela@unip.com       | professor |        1 |
+----+-----------+-----------+------------------------+-----------+----------+

select * from contatos
where grupo = 'trabalho'; // filtra todos salvos no grupo trabalho
+-----+--------------------+-------------+-----------------------+----------+----------+
| id  | nome               | telefone    | email                 | grupo    | favorito |
+-----+--------------------+-------------+-----------------------+----------+----------+
|  12 | Sofia Rodrigues    | 999999999   | sofia@example.com     | Trabalho |        0 |
|  15 | Fernando Oliveira  | 1212121212  | fernando@example.com  | Trabalho |        0 |
|  18 | Camila Sousa       | 1515151515  | camila@example.com    | Trabalho |        0 |
|  21 | Marcelo Almeida    | 1818181818  | marcelo@example.com   | Trabalho |        0 |
|  24 | Cristina Rodrigues | 2121212121  | cristina@example.com  | Trabalho |        0 |
|  27 | Felipe Oliveira    | 2424242424  | felipe@example.com    | Trabalho |        0 |
|  30 | Débora Sousa       | 2727272727  | debora@example.com    | Trabalho |        0 |
|  33 | Bruno Almeida      | 3030303030  | bruno@example.com     | Trabalho |        0 |
|  36 | Nathalia Rodrigues | 3333333333  | nathalia@example.com  | Trabalho |        0 |
|  39 | Marcos Oliveira    | 3636363636  | marcos@example.com    | Trabalho |        0 |
|  42 | Amanda Sousa       | 3939393939  | amanda@example.com    | Trabalho |        0 |
|  45 | Lucas Almeida      | 4242424242  | lucas2@example.com    | Trabalho |        0 |
|  48 | Ana Rodrigues      | 4545454545  | ana2@example.com      | Trabalho |        0 |
|  51 | Paulo Oliveira     | 4848484848  | paulo2@example.com    | Trabalho |        0 |
|  54 | Sara Sousa         | 5151515151  | sara2@example.com     | Trabalho |        0 |
|  57 | Rafael Almeida     | 5454545454  | rafael2@example.com   | Trabalho |        0 |
|  60 | Camila Rodrigues   | 5757575757  | camila2@example.com   | Trabalho |        0 |
|  63 | Leonardo Oliveira  | 6060606060  | leonardo2@example.com | Trabalho |        0 |
|  65 | Lucas Costa        | 6262626262  | lucas3@example.com    | Trabalho |        0 |
|  68 | Mariana Almeida    | 6565656565  | mariana3@example.com  | Trabalho |        0 |
|  71 | Diego Oliveira     | 6868686868  | diego3@example.com    | Trabalho |        0 |
|  74 | Vanessa Sousa      | 7171717171  | vanessa3@example.com  | Trabalho |        0 |
|  77 | Marcos Carvalho    | 7474747474  | marcos3@example.com   | Trabalho |        0 |
|  80 | Isabela Silva      | 7777777777  | isabela3@example.com  | Trabalho |        0 |
|  83 | Lucas Martins      | 8080808080  | lucas4@example.com    | Trabalho |        0 |
|  86 | Mariana Almeida    | 8383838383  | mariana4@example.com  | Trabalho |        0 |
|  89 | Diego Oliveira     | 8686868686  | diego4@example.com    | Trabalho |        0 |
|  92 | Vanessa Sousa      | 8989898989  | vanessa4@example.com  | Trabalho |        0 |
|  95 | Marcos Carvalho    | 9292929292  | marcos4@example.com   | Trabalho |        0 |
|  98 | Isabela Silva      | 9595959595  | isabela4@example.com  | Trabalho |        0 |
| 101 | Lucas Martins      | 9898989898  | lucas5@example.com    | Trabalho |        0 |
| 103 | Rafaela Oliveira   | 10101010101 | rafaela@example.com   | Trabalho |        0 |
| 106 | Lucas Costa        | 13131313131 | lucas6@example.com    | Trabalho |        0 |
| 109 | Ana Silva          | 16161616161 | ana3@example.com      | Trabalho |        0 |
| 112 | Marcos Carvalho    | 19191919191 | marcos5@example.com   | Trabalho |        0 |
| 115 | Isabela Silva      | 22222222222 | isabela5@example.com  | Trabalho |        0 |
| 118 | Lucas Martins      | 25252525252 | lucas7@example.com    | Trabalho |        0 |
| 121 | Mariana Almeida    | 28282828282 | mariana6@example.com  | Trabalho |        0 |
| 124 | Diego Oliveira     | 31313131313 | diego5@example.com    | Trabalho |        0 |
| 127 | Vanessa Sousa      | 34343434343 | vanessa5@example.com  | Trabalho |        0 |
| 130 | Marcos Carvalho    | 37373737373 | marcos6@example.com   | Trabalho |        0 |
| 133 | Isabela Silva      | 40404040404 | isabela6@example.com  | Trabalho |        0 |
| 136 | Lucas Martins      | 43434343434 | lucas8@example.com    | Trabalho |        0 |
| 139 | Mariana Almeida    | 46464646464 | mariana7@example.com  | Trabalho |        0 |
| 142 | Diego Oliveira     | 49494949494 | diego6@example.com    | Trabalho |        0 |
| 145 | Vanessa Sousa      | 52525252525 | vanessa6@example.com  | Trabalho |        0 |
| 148 | Marcos Carvalho    | 55555555555 | marcos7@example.com   | Trabalho |        0 |
| 150 | Rafaela Oliveira   | 10101010101 | rafaela@example.com   | Trabalho |        0 |
+-----+--------------------+-------------+-----------------------+----------+----------+
 
select * from contatos
    -> where nome = 'marcelao'; // filtra apenas o nome da pesquisa
+----+----------+-----------+------------------------+-----------+----------+
| id | nome     | telefone  | email                  | grupo     | favorito |
+----+----------+-----------+------------------------+-----------+----------+
|  9 | marcelao | 666666666 | marcela.gomes@unip.com | professor |        1 |
+----+----------+-----------+------------------------+-----------+----------+

mysql> delete from contatos where nome = 'marcelao'; // deleta o contato marcelao
