## MONGO URI FORMAT

MONGO_URI="mongodb://<MONGO_USERNAME>:<MONGO_PASSWORD>@localhost:<MONGO_PORT_1>/<DB_NAME>?authSource=admin"

### MONGO URI EXAMPLE

MONGO_URI="mongodb://mongo-db-admin:mongo-password@localhost:27017/db?authSource=admin"

Here all the collections will be created in db

To see all the collections

1.  docker exec -it mongo-db sh
2.  mongo -u mongo-db-admin
3.  mongo-password
4.  use db
5.  show collections

### For application which is in the same docker network as the mongodb container

MONGO_URI="mongodb://mongo-db-admin:mongo-password@<mongo_db_container_name>>:27017/db?authSource=admin"