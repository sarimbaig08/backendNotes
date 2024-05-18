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


11/5/24
Environment variables
System env
Project env are used mostly

Npm I dotenv
Import ‘dotenv/config’
Process.env.<name of variable>

Otp through mail
Package used is nodemailer
Mailinater for temp mails

16/5/24
Cloudinary: used to handle images online
Api have some content types, by default its json
Multipart api type: bring request in chunks, e.g img will be breaked in parts and will be send to server in pieces not whole img is send
Node js by default don’t handle multipart request, So we need to use 3rd party application named Multer
Setup cloudnary
Npm install cloudnary
Follow documention

Two ways to handle multer
Read all the chunks makes a file and give it to server
Server get chunks of image and store it in memory


Images can be handled in 2 ways using multer
•	Create a session in memory
•	Make folder of image and save chunks in it, diskStorage, takes an object({destination, filename)}
Cb(true,false) : through error
Cb(false,true): send request to controller
Cb = callback works as next in api
18/5/24
Steps to config Cloudinary
Npm I cloudinary
cloudinary config file
make cloudinary uploader
call cloudinary in app.js file
make api
image comes in multipart so we have to initialize multer in our project
npm I multer
we want multer on some specific apis
so make a middleware in image api
after making api go to postman, body, formdata, write key same so passing in api, 
now in api controller
set cloudinaryuploader
make fs.unlinkSync(req.file.path) : this is used to remove the coming image from server
send response
send image from front end
multipart don’t go in object
multipart api only support form data
make a function of onchange in react app, which will run when file is selected
make formData new object 
form.append(key,value)
now make axios api
axios.post(url,data,header)




Images can be handled in 2 ways using multer
•	Create a session in memory
•	Make folder of image and save chunks in it, diskStorage, takes an object({destination, filename)}
Cd(true,false) : through error
Cd(false,true): send request to controller


