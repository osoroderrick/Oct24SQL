# Oct24Sql
\\\
mysql> show databases;
+--------------------+
| Database           |
+--------------------+
| homeworkoct24      |
| information_schema |
| mysql              |
| performance_schema |
| sakila             |
| sys                |
| world              |
+--------------------+
7 rows in set (0.00 sec)

mysql> use homeworkOct24;
Database changed
mysql> describe movies;
+----------+--------------+------+-----+---------+----------------+
| Field    | Type         | Null | Key | Default | Extra          |
+----------+--------------+------+-----+---------+----------------+
| id       | int unsigned | NO   | PRI | NULL    | auto_increment |
| title    | varchar(20)  | NO   |     |         |                |
| genre    | varchar(100) | NO   |     |         |                |
| duration | int unsigned | NO   |     | 0       |                |
+----------+--------------+------+-----+---------+----------------+
4 rows in set (0.00 sec)

mysql> INSERT INTO movies VAlUE(1,'Metropolis','Sci-Fi',153);
Query OK, 1 row affected (0.02 sec)

mysql> INSERT INTO movies VAlUE(2,'Nosferatu','Horror',94);
Query OK, 1 row affected (0.00 sec)

mysql> INSERT INTO movies VAlUE(3,'The Kid','Comedy',68);
Query OK, 1 row affected (0.02 sec)

mysql> INSERT INTO movies VAlUE(4,'The Gold Rush','Adventure',95);
Query OK, 1 row affected (0.02 sec)

mysql> SELECT * FROM movies;
+----+---------------+-----------+----------+
| id | title         | genre     | duration |
+----+---------------+-----------+----------+
|  1 | Metropolis    | Sci-Fi    |      153 |
|  2 | Nosferatu     | Horror    |       94 |
|  3 | The Kid       | Comedy    |       68 |
|  4 | The Gold Rush | Adventure |       95 |
+----+---------------+-----------+----------+
4 rows in set (0.00 sec)
