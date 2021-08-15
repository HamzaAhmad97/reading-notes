# Mongo and Mongoose

## nosql vs sql (text)

| SQL             | NoSQL          | 
| -------------       |:-------------:| 
|  table based     |       document based        |
|    good fit for the complex query intensive environment |    not good fit for complex queries    |
|      vertically scalable     |    horizontally scalable    |

1. Data that is considered a good fit to be stored in a SQL data base should be: not that complex or entangled compared to that strored in NoSQL DBs, but most importantly, it should not be hierarchical.

2. As an example on a SQL db we have mySql.

3. Data that is considered a good fit to be stored in a NoSQL data base should be: or can be more complex, talking about objects having other objects as values and so on, which means it can be hierarchical.

4. An example on NoSQL db is MongoDB.

5. The best type of database for hierarchical is NoSQL database since the complexity of the stored object can grow exponentially which is suitable to be stored in NoSQL data bases since they use the traditional key value pairs.

6. It looks like it is just matter of preference which is also based on what you aim your data base to be best in, meaning that with NoSQL you have some drawbacks when it comes to handling complex query intensive environment but on the other hand, they are easier to scale since you only need to add more servers the thing that SQL databases lack, which means that they require more inforastructure, so it refers to the one whose job is to select the suitable type of database.

--------------------------------------

## nosql vs sql (video)

1. SQL stands for Structured Query Language.

2. Relational databases are type of databases that stores and provides access to data points that are related to one another meaning that they have a relational model, so for example a table might store customers' data and each customer is related to another table storing his orders and so on, this can also be explained by bringing the terms one-to-one relations and one-to-may relations.

3. Relational databases have a structure that is similar to normal tables.

4.  A schema can  be thought of as being the type of data and the order they are stored in, meaning that they data points or rows should follow the one appearing in the header.

5. NoSQL databases are based on documents so instead of having different tables that are connected, we have attributes or properties and each one of them points or holds the relted data.

6. They work by using the key value pair model.

7. Inside a MongoDB we have collections and documents .

8. MongoDB is more flexible than SQL databases since you can have different formats for the data as you also can remove the ones that do not have values or null as in SQL databases.

9. Disadvanages of NoSQL databases include having thier own syntax for querying data, and the lack of a rigid schema, as they also do not offer a lot of consistancy compared to SQL databases.