# mongoClone

POSTMAN Collection Link
https://www.getpostman.com/collections/cc263cd7508e79d25499

API'S :-
1. MongoDump
Method: POST
API: /api/mongodump
Body: 
{
    "from": {
        "url": "mongodb+srv://admin:result2022@cluster0.efn7p.mongodb.net/lms",
        "username": "root",
        "password": "root"
    },
    "to": {
        "url": "localhost",
        "username": "root",
        "password": "root"
    },
    "deleteFlag": false,
    "isSourceAtlasLink":true,
    "isDestAtlasLink":false,
    "dbName":"lms"
}

2. Delete Collection
Method: POST
API: /api/deleteColletion
Body: 
{
    "from": {
        "url": "localhost",
        "username": "root",
        "password": "root"
    },
    "to": {
        "url": "localhost",
        "username": "root",
        "password": "root"
    },
    "deleteFlag": true,
    "isSourceAtlasLink":false,
    "dbName":"lms"
}

3. MongoRestore
Method: POST
API: /api/mongorestore
Body: 
{
    "from": {
        "url": "mongodb+srv://admin:result2022@cluster0.efn7p.mongodb.net/lms",
        "username": "root",
        "password": "root"
    },
    "to": {
        "url": "mongodb+srv://root:root@cluster0.e1lhf.mongodb.net",
        "username": "root",
        "password": "root"
    },
    "deleteFlag": false,
    "isSourceAtlasLink":true,
    "isDestAtlasLink":true,
    "dbName":"lms"
}