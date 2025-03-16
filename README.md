# SQL-
sql do cartorio da EBAC
CREATE TABLE usuarios
(
cpf integer,
nome varchar(50),
sobrenome varchar(50),
cargo varchar(50),
curso_id integer
);

CREATE TABLE curso
(
  id integer,
  nome_curso varchar(50),
  professor varchar (50),
  categoria varchar (50)
);
 
INSERT INTO usuarios (cpf, nome, sobrenome, cargo, curso_id)
VALUES ('123','pedro','brocaldi','professor','1');
INSERT INTO usuarios (cpf, nome, sobrenome, cargo, curso_id) 
VALUES ('12365','junin','tijolo','aluno','1');
INSERT INTO usuarios (cpf, nome,sobrenome,cargo,curso_id)
VALUES ('12389','junin','capital','aluno','1');
INSERT INTO usuarios (cpf, nome,sobrenome,cargo,curso_id)
VALUES ('1238','marks','louco','aluno','2');
INSERT INTO usuarios (cpf, nome, sobrenome, cargo, curso_id) 
VALUES ('1236','vitor','maluco','aluno','2');

INSERT INTO curso (id,nome_curso,professor,categoria)
VALUES ('1','ti do zero','pedro brocaldi','programaçaõ');
INSERT INTO  curso (id,nome_curso,professor,categoria)
VALUES ('2','SQL','carlos','dados');

update usuarios
set curso_id='1'
where cpf='1238';

select * from usuarios
where cpf='1238';

