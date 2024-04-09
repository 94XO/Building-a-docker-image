# Building-a-docker-image
#Building a docker image for a nodeJS application.

#kindly find the server.js file
const express = require('express');
#this imports the express framework into the nodeJS app
const app = express();
#the 'app' variable is used to define routes and start the server

app.get('/', (req,res)=>{
     res.send("Welcome to my awesome app!"); 
 });

app.listen(3000, function () {
    console.log("app listening on port 3000");
#listening for incoming HTTP requests on port 3000.
});

#simple nodejs app using the express framework.


#the docker file sets up a docker image within the Node.js runtime environment,installs dependencies, and configures it to run a Node.js application using server.js as the entry point.



