# ER-To-Relational Mapping Algorithm
1. Mapping of Regular Entity Types.
2. Mapping of Weak entity Types.
3. Mapping of Binary 1:1 Realtion Types.
4. Mapping of Binary 1:N Realationship Types.
5. Mapping of Binary M:N Realationsship Type.
6. Mapping of Multivalued attributes.
7. Mapping of N-ary Realationship Types.
---
## Mapping of Regular Entity Types.
* set it's attributes in table contain one row.
* set under-line in `Primary-key`
* if there `Multivalued-attribute` set it in new table with the `Primary-key` as `foreign-key` then set arrow from `foreign-Key` to `Primary-Key`
* if there `Composit-attribute` break it donw into its emponent elements.
---
## Mapping of Binary 1:1 Realtion Types.
* 1 (Total)   : 1 (Total)     => 1 Table , chose `PK` of any Entity to this table
* 1 (partial) : 1 (Total)     => 2 tables, take `PK` of Parital as `FK` in total Table
* 1 (partial) : 1 (partial)   => 3 tables , `PK` of third table is the `PK` of any table
---
## Mapping of Binary 1:N Realtion Types.
* 1 : M (Total) => 2 tables , chosse `PK` of one as `FK` in `many`
* 1 : M (Partial) => 3 tables , `PK` of third table is `Many`
---
## Mapping of Binary M:N Realtion Types.
* 3 tables , `PK` of third Table is compsite `PK` of PKs of 2 tables
---
## Mapping of N-ary Realationship Types.
* Table for Each Entity + Table for relationship Contains `PK` of each table as `FK` (its `PK` is `composite-PK`).
