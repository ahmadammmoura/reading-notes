# What is JWT? How does it work? Why JWT?

![img](https://res.cloudinary.com/practicaldev/image/fetch/s--S1SRzR1m--/c_limit%2Cf_auto%2Cfl_progressive%2Cq_auto%2Cw_880/https://dev-to-uploads.s3.amazonaws.com/uploads/articles/68hk5xfjwabf6k9wxypo.png)

### What is JWT?

###### JWT stands for “ JSON web token ” it is an open standard (RFC 7519) that defines a compact and self-contained way for securely transmitting information between parties as a JSON object.

###### JWT is simply a token that is written in JSON format. It is really safe to use because it can be signed in using a secret (with the HMAC algorithm) or a public/private key pair using RSA or ECDSA.

### How does JWT work?

###### JWT contains 3 parts 1) The header 2) The payload 3) The signature

![img](https://res.cloudinary.com/practicaldev/image/fetch/s--_Fjuyaut--/c_limit%2Cf_auto%2Cfl_progressive%2Cq_auto%2Cw_880/https://dev-to-uploads.s3.amazonaws.com/uploads/articles/26p8pwkq1viwi8ed5654.png)

###### The header of the JWT token is just some metadata for the token such as the algorithm name and type.

![img](https://res.cloudinary.com/practicaldev/image/fetch/s--hDYEY8_d--/c_limit%2Cf_auto%2Cfl_progressive%2Cq_auto%2Cw_880/https://dev-to-uploads.s3.amazonaws.com/uploads/articles/w2qyjsjzqmu0z82pftwk.png)

###### The payload is some data that you can encode into the jwt which will be saved in the token payload and later you can use those unique data to identify the specific user. The more data you add the bigger the jwt token will be.

![img](https://res.cloudinary.com/practicaldev/image/fetch/s--AGAWmIdK--/c_limit%2Cf_auto%2Cfl_progressive%2Cq_auto%2Cw_880/https://dev-to-uploads.s3.amazonaws.com/uploads/articles/xpu57zwitg7yj8o7h98b.png)

###### And keep in mind that the header and the payload will get added as an encoded plain text but it is not going to get encrypted so anyone can decode them so we cannot save any sensitive data in the payload.

###### The secret is created with the header, the payload, and the secret that is stored on the server and this will process the signing JWT.

###### So, the signing algorithm is just an algorithm of JWT to verify if the token is correct. The signing algorithm creates a unique signature using the header, payload, and the secret, and only these data + the secret saved in your server can create this signature. Then this signature and header+payload forms the JWT Token which then is sent to the client

![img](https://res.cloudinary.com/practicaldev/image/fetch/s--9c2hs_x7--/c_limit%2Cf_auto%2Cfl_progressive%2Cq_auto%2Cw_880/https://dev-to-uploads.s3.amazonaws.com/uploads/articles/wwbsfabpgj9x3f0aujee.png)

### So, how does this process really work?

###### First, a user sends a post request to the server with the username and the password. Then the server checks the username and password is valid if this information is valid a JWT Token is formed and then gets send to the client and save in a cookie.

###### Now every time the server receives a JWT Token and grant the user access to the protected page it needs to verify the JWT Token in order to determine if the user really is the user he/she claims to be. In other words, it's gonna check that if no one manipulated the header and the payload data of the token. So it is gonna make sure that no 3rd party has manipulated the header and the payload data.

###### So how does the verification work? Well, whenever a JWT Token is received the verification method will take the header+paylaod and add the secret to it which is still on your server so no one can manipulate your secret, and then create a Test signature. and the original signature still remains on the JWT Token itself so now the Verification will compare the Test Signature with the original signature and if these two matched then that means the Token was not modified so the verification method will be successful but if it didn't match then that means someone did something with the Token so the verification method will fail.

### /////////////////////////////////////////////////////////////////

### 1- Write the following steps in the correct order:

- Receive access token
- Redirect to a third party authentication endpoint
- Register your application to get a client_id and client_secret
- Make a request to a third-party API endpoint
- Ask the client if they want to sign in via a third party
- Receive authorization code
- Make a request to the access token endpoint

1. Register your application to get a client_id and client_secret.

2. Ask the client if they want to sign in via a third party.

3. Redirect to a third party authentication endpoint.

4. Make a request to a third-party API endpoint

5. Receive authorization code.

6. Make a request to the access token endpoint.

7. Receive access token

### 2 - What can you do with an authorization code?

###### The authorization code is a temporary code that the client will exchange for an access token. The code itself is obtained from the authorization server where the user gets a chance to see what the information the client is requesting, and approve or deny the request.

### 3- What can you do with an access token?

###### A token is used to make security decisions and to store tamper-proof information about some system entity. While a token is generally used to represent only security information, it is capable of holding additional free-form data that can be attached while the token is being created.

s

### 4- What’s a benefit of using OAuth instead of your own basic authentication?

###### It allows limited access to the user's data and allows accessing when authorization tokens expire. It has ability to share data for users without having to release personal information. It is easier to implement and provides stronger authentication.

## Document the following Vocabulary Terms

- Client ID =>A client ID is a unique eight-digit number generated by the depository participants to easily identify their clients.
- Client Secret => A client secret is a secret known only to your application and the authorization server. It protects your resources by only granting tokens to authorized requestors. Protect your client secrets and never include them in mobile or browser-based apps.
- Authentication Endpoint => The authorization code is a temporary code that the client will exchange for an access token. The code itself is obtained from the authorization server where the user gets a chance to see what the information the client is requesting, and approve or deny the request.
- Access Token Endpoint => token endpoint is where apps make a request to get an access token for a user. This section describes how to verify token requests and how to return the appropriate response and errors. Authorization Code. Password Grant. Client Credentials.
- Authorization Code => An authorization code is an alphanumeric password that authorizes its user to purchase, sell or transfer items, or to enter information into a security-protected space.
- Access Token => Access tokens are the thing that applications use to make API requests on behalf of a user.

1. Which 3 things had you heard about previously and now have better clarity on?

- OAuth
- authorization
- authentication

2. Which 3 things are you hoping to learn more about in the upcoming lecture/demo?

- JWT
- more comlex auth

3. What are you most excited about trying to implement or see how it works?

- JWT
