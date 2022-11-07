# mongoClone

{
"info": {
"_postman_id": "f16969c9-5982-4b65-b13a-15652f8c792d",
"name": "MONGO SCRIPT",
"schema": "https://schema.getpostman.com/json/collection/v2.0.0/collection.json"
},
"item": [
{
"name": "MONGO DUMP",
"id": "ff4ad3e6-b771-44ce-8488-23fae3343296",
"request": {
"method": "POST",
"header": [],
"body": {
"mode": "raw",
"raw": "{ "from": { "url": "mongodb+srv://admin:result2022@cluster0.efn7p.mongodb.net/lms", "username": "root", "password": "root" }, "to": { "url": "localhost", "username": "root", "password": "root" }, "deleteFlag": false, "isSourceAtlasLink":true, "isDestAtlasLink":false, "dbName":"lms" }",
"options": {
"raw": {
"language": "json"
}
}
},
"url": "localhost:3000/api/mongodump"
},
"response": []
},
{
"name": "Delete Colletions",
"id": "6fb4643c-4dd6-49e0-b36c-04f496c03e8b",
"request": {
"method": "POST",
"header": [],
"body": {
"mode": "raw",
"raw": "{ "from": { "url": "localhost", "username": "root", "password": "root" }, "to": { "url": "localhost", "username": "root", "password": "root" }, "deleteFlag": true, "isSourceAtlasLink":false, "dbName":"lms" }",
"options": {
"raw": {
"language": "json"
}
}
},
"url": "localhost:3000/api/deleteColletion"
},
"response": []
},
{
"name": "MONGO RESTORE",
"id": "fad7fa36-f9e3-41fa-aa10-b121b40461ac",
"request": {
"method": "POST",
"header": [],
"body": {
"mode": "raw",
"raw": "{ "from": { "url": "mongodb+srv://admin:result2022@cluster0.efn7p.mongodb.net/lms", "username": "root", "password": "root" }, "to": { "url": "mongodb+srv://root:root@cluster0.e1lhf.mongodb.net", "username": "root", "password": "root" }, "deleteFlag": false, "isSourceAtlasLink":true, "isDestAtlasLink":true, "dbName":"lms" }",
"options": {
"raw": {
"language": "json"
}
}
},
"url": "localhost:3000/api/mongorestore"
},
"response": []
}
]
}