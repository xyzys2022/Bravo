# Bravo
Bravo hopes to provide common components of databases and big data, which can help you reduce a lot of development costs when writing databases.

First of all, Bravo will implement an SQL parser to parse MySQL's DML, DDL, DCL syntax (including stored procedures), and further increase syntax support for PostgreSQL, SQLServer, Spark, Hive and so on.

In the future, Bravo will provide more components. For example, Bravo may provide a plug-in of connection pool, so that you can coordinate the behavior between redis and the database in a simpler way.


## Phase 1: Complete common syntax, extend MySQL syntax
references: 
https://en.wikipedia.org/wiki/SQL-92
http://www.contrib.andrew.cmu.edu/~shadow/sql/sql1992.txt
https://www.mysqlzh.com/doc/129/652.html
https://www.mysqlzh.com/doc/225/510.html

TODO:
1. Build code structure.
2. Define basic keywords and implement the tokenizer. (reference resources: com.alibaba.druid)
3. Parse basic keywords, data type, value, table, column, expression, clauses
4. Parse SELECT, UPDATE, DELETE, INSERT, TRUNCATE syntaxes under standard SQL, it contains with clause
5. Parse CREATE, ALTER, DROP, Rename syntax for table, view, database syntaxes under standard SQL

6. Extended MySQL keywords and expressions.
7. Parse SELECT, UPDATE, DELETE, INSERT, TRUNCATE syntaxes under MySQL.
8. Parse CREATE, ALTER, DROP, RENAME, SHOW CREATE syntax for table, partition table, view, database syntaxes under MySQL
9. Parse ANALYZE, OPTIMIZE, CHECK, REPAIR for table syntaxes under MySQL
10. Parse CREATE, DROP, Rename syntax for index syntaxes under MySQL
11.  Parse SHOW, DO, DESCRIBE, SET, START, BEGIN, STOP, COMMIT, ROLLBACK, LOCK, UNLOCK, XA, LOAD, CACHE, FLUSH, KILL, RESET, PURGE, CHANGE, PREPARE, EXECUTE, DEALLOCATE syntaxes under MySQL
12.  Parse CREATE, DROP, GRANT, REVOKE, SET PASSWORD, RENAME for user syntaxes under MySQL
13.  Parse CREARE, ALTER, DROP, SHOW CREATE, SHOW STATUS, CALL, BEGIN ... END, DECLARE, DO, Define Variables, SET Variables, CONDITION, SELECT ...INTO, CONTINUE, EXIT, UNDO, SQLWARNING, NOT FOUND, SQLEXCEPTION, DECLARE CURSOR, OPEN CURSOR, FETCH CURSOR, CLOSE CURSOR, IF, CASE, LOOP, LEAVE, ITERATE, REPEAT, WHILE, FOR EACH ROW for PROCEDURE, FUNCTION, EVENT, TRIGGER under MySQL


## Phase 1: PostgreSQL 14 syntax
references: 
http://www.postgres.cn/docs/14/index.html

TODO：
1. 
