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

https://learn.udacity.com/nanodegrees/nd027/parts/9ce03188-a0b9-425b-8a8c-2f2d05e48150/lessons/1769658b-4fdd-4889-9d70-84f9a474958b/concepts/4ae8d29d-6732-4b9a-9887-e1ef948c5764
