mysql -u ROOT
show databases;
CREATE DATABASE [database_name];
USE [database_name];
show tables;
CREATE TABLE table_name (field1 data_type, field2 data_type2);
INSERT INTO table_name VALUES(value1 , value2);
INSERT INTO table_name (specific_field1,specific_field2,specific_field3) values(value1,value2,value2);
UPDATE table_name SET column1 = value1, column2 = value2 WHERE condition;
DELETE FROM table_name WHERE condition;
ALTER TABLE table_name ADD column field data_type;
ALTER TABLE table_name DROP column field;
ALTER TABLE table_name MODIFY COLUMN column_name datatype;
CREATE TABLE table_name (field1 data_type NOT NULL, field2 data_type2 NOT NULL);/* prevant null values*/
CREATE TABLE table_name (field1 data_type NOT NULL, field2 data_type2 NOT NULL UNIQUE);/* unique value*/
CREATE TABLE table_name (field1 data_type NOT NULL, field2 data_type2 NOT NULL , PRIMARY KEY (field_name));/* unique value*/
CREATE TABLE table_name (field1 data_type NOT NULL, field2 data_type2 FOREIGN KEY (field1) REFERENCES table_name(field_name));/*foreign value*/
SELECT MIN(column_name) FROM table_name WHERE condition;
SELECT MAX(column_name) FROM table_name WHERE condition;
SELECT AVG(column_name) FROM table_name WHERE condition;
SELECT SUM(column_name) FROM table_name WHERE condition;
SELECT COUNT(column_name) FROM table_name WHERE condition;
SELECT column1, column2 FROM table_name WHERE CustomerName LIKE 'a%';/* start with a */
SELECT column1, column2 FROM table_name WHERE CustomerName LIKE 'a%';/* end with a */
SELECT column1, column2 FROM table_name WHERE CustomerName LIKE '%a%';/* start with a */
SELECT column1, column2 FROM table_name WHERE CustomerName LIKE 'a_%';/*start with a at least length of 3*/
SELECT column1, column2 FROM table_name WHERE CustomerName LIKE 'a%o';/*start with a end with o*/
