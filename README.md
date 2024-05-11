# backendNotes

25/4/24
Api responses are mostly json
Res.json sending data in json
Res.send sending data in any format
Api holds url(server address, base url), 
Api methods is of different types get, post, put, delete
 
Only get api can be directly called from url on google
Use Swager, Post man to test apis
Raw json has object in string
When client send data to server, server don’t read the body due to security purpose. Then app.use is used which reads every request
App.use(express.json()) function is to parse every request body
App.user(express.urlencoded({extexded:true})) sometime body is encoded
Headers and body is send when request is send. Header handles api behavior and some are default.
Content type header is always there in those api which have body.

Rest and restful apis

Mongo DB
It can be used on any platform

SQL:
Data is saved in entity format(rows and columns)
RDBMS( relational database management system)

Follows Schema(structure), defining it is necessary	No SQL:
Data saved in json format

Some relational and some are not

Optional to define schema

Schema gives a shape to dB like which fields and properties are required or not
Restrict front end developers or user to send us data in a particular format
27/April/24
Mongodb atlas (cloud database), compass paste URI in server provided my DB

After setup
Browse collections, 
Npm I mongoose(ORM)
Mongodb collection in mongoose is called modal
4/May/24
Npm I cors, to check request coming on server
Nest architecture
Mvc architecture
Architectures are used for scalability
Model: define data structure/schema
Controller: business logics, it’s written under api function{ apis are breaked into routes(endpoints/urls) and controllers(logics)
View: UI, front-end pages
In get api body is not supported means data cannot be send through get api, So to get a data using id or something else we pass the data through params

Encryption
Npm I bcrypt( uses # encryption method)
