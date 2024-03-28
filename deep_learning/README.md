# deep_learning
This requires setting up a PosgreSQL database connection on AIVEN and obtaining a URI from this.
You can then set up a table in your terminal once it's up and running:

psql '<INSERT-YOUR-URI>'

defaultdb=> CREATE EXTENSION vector;
CREATE EXTENSION
defaultdb=> CREATE TABLE pictures (picture text PRIMARY KEY, embedding vector(768));
CREATE TABLE

And this same URI will be used in the database. It definitely recognised Brad Pitt! :) 