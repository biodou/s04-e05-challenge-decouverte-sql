Auteurs
Lister les auteurs
SELECT  name FROM author

Afficher l'auteur ayant l'id 2
SELECT  name FROM author WHERE id = 2


Articles
Lister tous les articles
SELECT content FROM post

Afficher l'article ayant l'id 1
SELECT  content FROM post WHERE id = 1

++++++++++

Bonus SQL


Auteurs
Lister les auteurs par ordre alphabétique (sur le nom) (doc)
SELECT  name  FROM author ORDER BY  name


Lister les auteurs dont l'e-mail contient @gmail.com (doc)
SELECT  name  FROM author  WHERE email LIKE '%@gmail.com%'


Lister les auteurs qui n'ont pas d'image de profil (doc)
SELECT  name  FROM author  WHERE image IS NULL



Articles
Lister le titre et la date de publication de tous les articles (doc)
SELECT  title ,  published_date  FROM post


Afficher le titre d'un article en particulier (en passant l'id de l'article) (doc)
SELECT  title  FROM post WHERE id=1


Lister les 2 derniers articles publiés (doc & doc)
SELECT content FROM post ORDER BY published_date LIMIT 2 


Compter le nombre d'articles (doc) et renommer la colonne en nbArticles (doc)
SELECT COUNT(*) FROM post 