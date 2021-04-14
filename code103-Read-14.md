# Database Normalization
is the process of organizing data in a database. This includes creating tables and establishing relationships between those tables according to rules designed both to protect the data and to make the database more flexible by eliminating redundancy and inconsistent dependency.

## Reasons for Database Normalization:
1. To minimize duplicate data.
2. To minimize or avoid data modification issues.
3. To simplify queries.

### Database normalization forms

1. **1NF:**
- Eliminate repeating groups in individual tables.
- Create a separate table for each set of related data.
- Identify each set of related data with a primary key.

2. **2NF:**
- Create separate tables for sets of values that apply to multiple records.
- Relate these tables with a foreign key.

3. **3NF:** 
- the table is in second normal form and all of its columns are not transitively dependent on the primary key.
- Eliminate fields that do not depend on the key.
