// We install mongodb and mongo compass on ubuntu 20.04 LTS

> show dbs
admin   0.000GB
config  0.000GB
local   0.000GB
test1   0.000GB
> use te
TestData            testingReplication
> use test1
switched to db test1
> show collections
products
> db.dropDatabase()
{ "dropped" : "test1", "ok" : 1 }
> show dbs
admin   0.000GB
config  0.000GB
local   0.000GB
> use test2
switched to db test2
> show dbs
admin   0.000GB
config  0.000GB
local   0.000GB
> db
test2
> db.createCollection('posts')
{ "ok" : 1 }
> show dbs
admin   0.000GB
config  0.000GB
local   0.000GB
test2   0.000GB
> show collections
posts
>
