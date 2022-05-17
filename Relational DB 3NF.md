The objectives of normalisation beyond 1NF (first normal form) were stated as follows by Codd:

- To free the collection of relations from undesirable insertion, update and deletion dependencies.
- To reduce the need for restructuring the collection of relations, as new types of data are introduced, and thus increase the life span of application programs.
- To make the relational model more informative to users.
- To make the collection of relations neutral to the query statistics, where these statistics are liable to change as time goes by.

[Wikipedia](https://en.wikipedia.org/wiki/Database_normalization)


1NF:
- Atomic values: each cell contains unique and single values
- Each record needs to be unique

2NF:
- Have reached 1NF
- All columns in the table must rely on the Primary Key


3NF:
- Must be in 2nd Normal Form
- No transitive dependencies
