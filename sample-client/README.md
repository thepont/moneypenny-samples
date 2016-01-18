#oauth-local

This application demonstrates how to connect to the authentication server using oAuth.

The following record, will have to be added to the moneypenny server database to be able to use this sample app

###oauth_client

```
{
    "_id" : "oAuthTest",
    "redirectUri" : "http://localhost:3334/auth/provider/callback",
    "secret" : "$2a$10$uXE9L6J5Xq3wW2UCxI11juqVU3xIhNSP2ZoFaiSH//XnfPdQCOU6W"
}
```
