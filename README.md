The sample client should be able to connect to the sample server, the following will have to be configured for this to work.

Inside the `oauth_client` collection the following record will have to be added

```
{
    "_id" : "oAuthTest",
    "redirectUri" : "http://localhost:3334/auth/provider/callback",
    "secret" : "$2a$10$uXE9L6J5Xq3wW2UCxI11juqVU3xIhNSP2ZoFaiSH//XnfPdQCOU6W"
}
```

after this if the sample server and sample client are launched the two should connect together and you should be able to login with the username "jsmith" and password "password"

##Sample Server

###Constants

```
var MONGO_DB_HOST = 'localhost';
var MONGO_DB = 'toy_auth_manager_sample';
var USERNAME = 'jsmith';
var PASSWORD = 'password';
```

####MONGO_DB_HOST

The sample server currently connects to a mongodb running on `localhost`, change this to connec the sample code to a separate server.

####MONGO_DB

Database to store records relating to authentication in.

####USERNAME

Our test username that can be use to login to the server.

####PASSWORD

Our test users password that can be used to login to the server.


