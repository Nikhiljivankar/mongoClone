# mongoClone

POSTMAN Collection Link <br />
https://www.getpostman.com/collections/cc263cd7508e79d25499 <br />
https://documenter.getpostman.com/view/13151747/2s8YehUwaE <br />

API'S :&nbsp; <br />
1. &nbsp; MongoDump &nbsp; <br />
Method: &nbsp;  POST <br />
API: &nbsp;  /api/mongodump <br />
Body:  <br />
{
    "from": {
        "url": "mongodb+srv://{username}:{password}@cluster0.edbbp.mongodb.net/lms",
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

2.&nbsp; Delete Collection <br />
Method:  &nbsp; POST <br />
API: &nbsp;  /api/deleteColletion <br />
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

3.&nbsp; MongoRestore  <br />
Method: &nbsp;  POST <br />
API: &nbsp;  /api/mongorestore <br />
Body: <br />
{
    "from": {
        "url": "mongodb+srv://{username}:{password}@cluster0.edbbp.mongodb.net/lms",
        "username": "root",
        "password": "root"
    },
    "to": {
        "url": "mongodb+srv://root:root@cluster0.e1ah d.mongodb.net",
        "username": "root",
        "password": "root"
    },
    "deleteFlag": false,
    "isSourceAtlasLink":true,
    "isDestAtlasLink":true,
    "dbName":"lms"
}