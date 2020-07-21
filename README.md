# W5D2 - Database Design

### To Do
- [x] Primary Keys/Foreign Keys
- [x] Data Types
- [x] Relationship Types
- [x] Naming Conventions
- [x] Normalization
- [x] Design Concepts
- [x] Entity Relationship Diagrams
- [x] Breakout: Convert 2 Spreadsheets [15 mins]
- [x] Student Suggestion ERD(s)

ORM - Object Relational Mapper
user.posts
knex

select('users').where('id', 7);

### Primary Keys
* Uniquely identify a particular entity
* Use only autoincrementing integers
* PK should not contain metadata
* Foreign key is a primary key stored in another table
* FK and PK MUST be the same data type

### Data Types
* Used to be a huge concern
* VARCHAR(1 - 255), TEXT, INTEGER, BIGINTEGER, BOOLEAN

### Relationships
* One-to-one: one record in the 1st table is related to only 1 record in 2nd table
* One-to-many: 1 record in the 1st table is related to 1 or more in the 2nd
* Many-to-many: 1 or more in the 1st table related to 1 or more in the 2nd (through a junction/join table)

### Naming Conventions
* opinionated vary from company to company
* Pick a convention and stick with it
* Primary key is always `id`
* Table names are always lowercase and plural (users, posts, animals, pets)
* FK should be the singular table name plus `_id` (user_id, post_id)

### Normalization
* 1NF, 2NF, 3NF
* We want to reduce redundancy/duplicated in our data
* Single source of truth
* Improve the structure of our data

### Design Concepts
* Required: based on the initial state of the record
* Defaults: timestamps (date_created) NOW()
* Calculated fields: values that can derived from one or more other fields
* Pull repeating values out to a lookup table

vancouver, Vancouver, Vancover, vancity, van

1 Calgary
2 Vancouver
3 Toronto

* Try not to delete anything, `active` boolean

### ERD
* Entity Relationship Diagrams



### Breakout: Convert Two Spreadsheets
- [Gist with instruction](https://gist.github.com/andydlindsay/20e7305e853bad7b587f294b054cf8de)
