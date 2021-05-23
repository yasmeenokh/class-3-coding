# Write the following steps in the correct order
1. Register your application to get a client_id and client_secret
2. Ask the client if they want to sign in via a third party
3. Redirect to a third party authentication endpoint
4. Make a request to the third-party API endpoint
5. Receive authorization code
6. Make a request to the access token endpoint
7. Receive access token

# What can you do with an authorization code?
Authoriztion code can be used to set privilages to a user, or enter information or modify them.

# What can you do with an access token?
Access tokens are used in token-based authentication to allow an application to access an API.

# What’s a benefit of using OAuth instead of your own basic authentication?
Better security, token management provides you with a means of tracking each connected device that uses your API.also used to identify the users.

## Vocabulary Terms
#### Client ID : 
Is used to identify the application. As per oAuth standard you need both Client ID & Client Secret along with user credentials to generate an access token.
#### Client Secret : 
secret known only to the application and the authorization server
#### Authentication Endpoint: 
The Authentication API enables you to manage all aspects of user identity when you use Auth0.
#### Access Token Endpoint: 
where apps make a request to get an access token for a user
#### API Endpoint : 
is a point at which an application program interface connects with the software program.
#### Authorization Code : 
temporary code that the client will exchange for an access token
#### Access Token : 
is an object encapsulating the security identity of a process or thread.

#### Which 3 things had you heard about previously and now have better clarity on?
1. basic auth 
2. encoding 
3. hashing

#### Which 3 things are you hoping to learn more about in the upcoming lecture/demo?
basic auth mongodb data structure

# Preparation Materials
JSON Web Token (JWT): is a JSON object encoded as a long string. We use them to identify users. It’s similar to a passport or driver’s license.

Although JWTs can be encrypted to also provide secrecy between parties, we will focus on signed tokens. Signed tokens can verify the integrity of the claims contained within it, while encrypted tokens hide those claims from other parties. When tokens are signed using public/private key pairs, the signature also certifies that only the party holding the private key is the one that signed it.

**When to use JSON web token:**

authorization and information exchange

JSON web token consists of three parts separated by dots: header, payload, signature
JSON web tokens are a good choice to be passed in HTML and HTTP environments