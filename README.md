# MongoDB
Details about mongodb

###### installation steps in ubuntu 16

click here https://docs.mongodb.com/manual/tutorial/install-mongodb-enterprise-on-ubuntu/

Mongodb written in c++,


npm.org.is 

Mongodb run on top of node.js
Node.js is run on v8 engine environment

> mongod --port
27109
> mongod --directoryperdb
>mongod --dbpath c:/data/db

creating json generation json  :::https://www.json-generator.com/

###Mongodb Update or add new field "$set"  remove field "$unset"

####Order in bulkwrites and insertMany
######false (order=false) : 
If any exception come at middle it will continues the remaining documents and skips the error document

######true (order=true) :
This is called automicity all the documents will roll back when time out exceeds (this is depend on wtimeout)

###### majority
This is called priopity
Use {w :"majority",wtimeout:100} use for give the majority of the documents you want to insert and give the time out for this operation
if the time exceeds the specified time then the transaction will roll back automatically (Transaction management)

