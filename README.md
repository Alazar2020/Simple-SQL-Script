# Simple-SQL-Script

-- create a new database
create database my_database;

/*
	CREATE TABLE [IF NOT EXISTS] table_name (table_def);
*/
create table if not exists my_table (
	-- col_name datatype constraints,
	id int primary key,
	my_value varchar(10) not null,
	my_other_value float default 0.0
);

/*
	ALTER TABLE table_name ADD COLUMN col_name col_definition
*/
alter table my_table add column my_last_value boolean default true;

/*
	drop [TABLE] table_name
*/
drop table my_table;

/*
	alter table table_name rename to new_table_name;
*/
alter table my_table rename to my_new_table;

/*
 	truncate [table] table_name
*/
truncate table my_new_table;

/*
 * Create a database named library
	In the library database create a table name books
	column: id int primary key
	column: title varchar(100) not null
	column: author varchar(50) not null
	Alter the books
	Add column: publication_date not null timestamp
	Add constraint: title unique
*/


