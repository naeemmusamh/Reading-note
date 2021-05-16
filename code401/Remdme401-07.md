# JSON Web Token

## what is JSON Web Token???

1. open standard ==> can any one use it.

2. securely transfer information between any two bodies ===> any two user and any two server and any two bodies.

3. digitally signed - information is verified and trusted ===> there is no alteration of data between the transfer.

4. compact ===> you can send it be URL, POST request, HTTP Header and it fast transmission.

5. self-contained ===> contains information about the user and avoiding query the database more than once.

6. can be signed using a secret ===>  public/private key.

## why the JSON Web Token usefully???

1. authentication ===> just explained you.

Once the user is logged in, each subsequent request will include the JWT, allowing the user to access routes, services, and resources that are permitted with that token.

2. information exchange ===> can change between any two body and you can be sure the senders are who they say they are.

## What is the JSON Web Token structure???

consist of three parts separated by dots :

![JWT](https://github.com/naeemmusamh/Reading-note/blob/master/IMAGE/401/JWT.jpg?raw=true)

1. Header :

consists of two parts : 

A-  type of the token, which is JWT.

B- the signing algorithm being used (HMAC SHA256 or RSA).

{
  "alg": "HS256",
  "typ": "JWT"
}

2. Payload : 

contains the claims ==> statements about an entity and additional data.

There are three types of claims :

A- registered :

are not mandatory but recommended, to provide a set of useful, interoperable claims.
like : iss(issuer), exp(expiration time), sub(subject), aud(audience)

B-public : 

can be defined at will by those using JWTs. But to avoid collisions they should be defined in the IANA JSON Web Token Registry or be defined as a URI that contains a collision resistant namespace.

C- private claims :

are the custom claims created to share information between parties that agree on using them and are neither registered or public claims.

{
  "sub": "1234567890",
  "name": "John Doe",
  "admin": true
}

3. Signature : 

the signature part you have to take the encoded header, the encoded payload, a secret, the algorithm specified in the header, and sign that.

HMACSHA256(
  base64UrlEncode(header) + "." +
  base64UrlEncode(payload),
  secret)


## How do JSON Web Tokens work???

In authentication, when the user successfully logs in using their credentials, a JSON Web Token will be returned.

## Why should we use JSON Web Tokens?

As JSON is less verbose than XML, when it is encoded its size is also smaller, making JWT more compact than SAML. This makes JWT a good choice to be passed in HTML and HTTP environments.

## how to work with JSON Web Tokens???

there is package provided for us by npm [jsonwebtoken](https://www.npmjs.com/package/jsonwebtoken)

1. install

npm install jsonwebtoken

2. Synchronous Sign with default

var jwt = require('jsonwebtoken');
var token = jwt.sign({ foo: 'bar' }, 'shhhhh');

3. Sign asynchronously

jwt.sign({ foo: 'bar' }, privateKey, { algorithm: 'RS256' }, function(err, token) {
  console.log(token);
});

4. Signing a token with 1 hour of expiration:

jwt.sign({
  exp: Math.floor(Date.now() / 1000) + (60 * 60),
  data: 'foobar'
}, 'secret');


5. Another way to generate a token like this with this library is:

jwt.sign({
  data: 'foobar'
}, 'secret', { expiresIn: 60 * 60 });
 
//or even better:
 
jwt.sign({
  data: 'foobar'
}, 'secret', { expiresIn: '1h' });