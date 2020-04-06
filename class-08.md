# SQL

- What is SQL?
- SQL, or Structured Query Language, is a language designed to allow both technical and non-technical users query, manipulate, and transform data from a relational database. And due to its simplicity, SQL databases provide safe and scalable storage for millions of websites and mobile applications.

- By learning SQL, the goal is to learn how to answer specific questions about this data, like "What types of vehicles are on the road have less than four wheels?", or "How many models of cars does Tesla produce?", to help us make better decisions down the road.

###  SELECT queries

 - we need to write SELECT statements, which are often colloquially refered to as queries to retrieve data. A query in itself is just a statement which declares what data we are looking for, where to find it in the database, and optionally, how to transform it before it is returned. It has a specific syntax though, which is what we are going to learn in the following exercises.

* Select query for a specific columns
  SELECT column, another_column,\…
  FROM mytable\;

### Queries with constraints

- In order to filter certain results from being returned, we need to use a WHERE clause in the query. The clause is applied to each row of data by checking specific column values to determine whether it should be included in the results or not.

###  Queries with constraints

- When writing WHERE clauses with columns containing text data, SQL supports a number of useful operators to do things like case-insensitive string comparison and wildcard pattern matching.

- All strings must be quoted so that the query parser can distinguish words in the string from SQL keywords.


### Filtering and sorting Query results

-  SQL provides a convenient way to discard rows that have a duplicate column value by using the DISTINCT keyword.

- Ordering results:
SQL provides a way to sort your results by a given column in ascending or descending order using the ORDER BY clause.

Another clause which is commonly used with the ORDER BY clause are the LIMIT and OFFSET clauses, which are a useful optimization to indicate to the database the subset of the results you care about.
The LIMIT will reduce the number of rows to return, and the optional OFFSET will specify where to begin counting the number rows from.




