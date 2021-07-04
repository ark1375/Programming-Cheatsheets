
# Mongo DBCheatSheet

Note that the main structure of this cheat sheet is based on [MongoDB Documentation](https://docs.mongodb.com/manual/tutorial/getting-started/).

## Table of Contents

## Basic Comands

- `db` to show which database is currently selected  

- `use <database name>` for switching to another database.
  >You do not need to create the database before you switch. MongoDB creates the database when you first store data in that database (such as create the first collection in the database).

## Analogy

> MongoDB stores data records as documents (specifically [BSON documents](https://docs.mongodb.com/manual/core/document/#std-label-bson-document-format)) which are gathered together in [collections](https://docs.mongodb.com/manual/reference/glossary/#std-term-collection). A [database](https://docs.mongodb.com/manual/reference/glossary/#std-term-database) stores one or more collections of documents.

_Collection:_ A grouping of MongoDB documents. A collection exists within a single database. _Typically, all documents in a collection have a similar or related purpose._ __Collections are analogous to tables in relational databases.__<br>  
_Database:_ A physical container for collections. Each database gets its own set of files on the file system. A single MongoDB server typically has multiple databases.<br>  
_Document_: A record in a MongoDB collection and the basic unit of data in MongoDB. Documents are analogous to JSON objects but exist in the database in a more type-rich format known as BSON.

## Populate a Collection (Insert)

- `db.collection.insertMany(doc)` insert new documents into the inventory collection.<br>
Returns an array of `_id` and an acknowledgement object.

## Select Documents

- `db.collection.find(qf)` select all documents in the collection, pass an empty document (`{}`) as the query filter document to the method.

### Specify Equality Matches

[link](https://docs.mongodb.com/manual/tutorial/getting-started/)

### Select All Documents

## Refrences

- [BSON Types](https://docs.mongodb.com/manual/reference/bson-types/)