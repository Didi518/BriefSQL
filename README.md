# BriefSQL
création du tableau 1

CREATE TABLE utilisateurs(
    id int(3),
    login varchar(20) NOT NULL,
    pssword varchar (20)NOT NULL,
    superuser varchar(20)NOT NULL
    
    )  ENGINE=InnoDB DEFAULT CHARSET=utf8 ;
    
 création du tableau 2   
 
    CREATE TABLE IMC(
        nom varchar (20)NOT NULL,
        prenom varchar (20)NOT NULL,
        taille int(3)NOT NULL,
        poids int(3)NOT NULL,
        genre varchar(5),
        IMC varchar (20)NULL       
        )ENGINE=InnoDB DEFAULT CHARSET=utf8 ;
        
 Ajouts des paramétres
INSERT INTO utilisateurs(login, pssword, superuser) VALUES 

('User10','password10',0),
( 'User20','password20',0),
( 'User30','password30',1),
( 'User40','password40',1),
( 'User50','password50',0),
( 'User60','password60',1)

ajouts IMC

INSERT INTO IMC (nom,prenom,taille,poids,genre,IMC) VALUES 
('Nom30','prenom30',130,50,'homme',NULL),
('Nom40','prenom40',140,60,'femme',NULL),
('Nom50','prenom50',150,70,'femme',NULL),
('Nom60','prenom60',160,80,'homme',NULL),
('Nom65','prenom65',165,80,'femme',NULL),
('Nom68','prenom68',168,80,'homme',NULL),
('Nom70','prenom70',170,90,'homme',NULL),
('Nom80','prenom80',180,100,'homme',NULL),
('Nom90','prenom90',190,110,'femme',NULL)


Question 1
SELECT * FROM `utilisateurs`
Question 2
SELECT * FROM `IMC`
Question 3
SELECT * FROM utilisateur;
SELECT * FROM IMC;
Question 4
SELECT * FROM utilisateurs WHERE superuser = 1
Question 5
SELECT * FROM `IMC` WHERE poids >= 65
Question 6
SELECT * FROM `IMC` WHERE poids >= 65 AND taille <=172
Question 7
UPDATE IMC SET IMC = 20 WHERE poids>=80;
Question 8
DELETE FROM IMC WHERE `nom` = "nom80";

