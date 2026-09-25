1) Authenticate to mongodb container for listing/creating databses/collection etc.

 docker-compose exec -it <svcName> mongosh -u <username> -p <password>

2)show databases;

3) Create a database.Name it as myapp

use myapp

4) create a collection. Name it as users. Inside it Sonali document

db.users.insertOne({
  name: "Sonali",
  role:"Devops"
})

5) Now read the data which we have stored just now
db.users.find()
