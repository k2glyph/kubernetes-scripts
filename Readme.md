# For Configurating Mongodb and scaling up and down change rs.conf()
```
config = {
 "_id" : "rs0",
 "members" : [
   {
     _id: 1,
     host: 'mongo-0.mongo.default.svc.cluster.local:27017'
   },
   {
     _id: 2,
     host: 'mongo-1.mongo.default.svc.cluster.local:27017',
   },
   {
     _id: 3,
     host: 'mongo-2.mongo.default.svc.cluster.local:27017'
   }
 ]
}
rs.initiate(config)
```