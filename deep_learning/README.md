# Setting up PostgreSQL Database Connection on AIVEN

This guide assumes that you've set up a PostgreSQL database connection on AIVEN and obtained a URI from it. 

Once you have the URI, follow these steps to set up a table in your terminal:

```bash
psql 'INSERT-YOUR-URI'
```

Replace 'INSERT-YOUR-URI' with the URI you obtained.

```sql
defaultdb=> CREATE EXTENSION vector;
CREATE EXTENSION

defaultdb=> CREATE TABLE pictures (picture text PRIMARY KEY, embedding vector(768));
CREATE TABLE
```

And this same URI will be used in the database. It definitely recognised Brad Pitt! :)