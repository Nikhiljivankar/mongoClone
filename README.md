# mongoClone

POSTMAN Collection Link <br />
https://www.getpostman.com/collections/cc263cd7508e79d25499 <br />

API'S :- <br />
1. MongoDump  <br />
Method:   POST <br />
API:   /api/mongodump <br />
Body:  <br />
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

2. Delete Collection <br />
Method:   POST <br />
API:   /api/deleteColletion <br />
Body:  <br />
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

3. MongoRestore  <br />
Method:   POST <br />
API:   /api/mongorestore <br />
Body: <br />
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