# Authentication

authentication is a method for an HTTP user agent to provide a user name and password when making a request.

A- Features :

HTTP Basic authentication (BA) implementation is the simplest technique for enforcing access controls to web resources because it does not require cookies, session identifiers, or login pages;

B- Security :

The BA mechanism does not provide confidentiality protection for the transmitted credentials. They are merely encoded with Base64 in transit and not encrypted or hashed in any way.

C- Protocol :

1.Server side :

When the server wants the user agent to authenticate itself towards the server, the server must respond appropriately to unauthenticated requests.

2. Client side :

When the user agent wants to send authentication credentials to the server, it may use the Authorization header field.

# Bcrypt or Hashing

Hashing is the greatest way for protecting passwords and considered to be pretty safe for ensuring the integrity of data or password.

The benefit of hashing is that if someone steals the database with hashed passwords, they only make off with the hashes and not the actual plaintext passwords.

## PROBLEMS WITH CRYPTOGRAPHIC HASH ALGORITHM

Brute Force attack: Hashes can't be reversed, so instead of reversing the hash of the password, an attacker can simply keep trying different inputs until he does not find the right now that generates the same hash value, called brute force attack.

Hash Collision attack: Hash functions have infinite input length and a predefined output length, so there is inevitably going to be the possibility of two different inputs that produce the same output hash.

const bcrypt = require('bcrypt');

const saltRounds = 10;

const myPlaintextPassword = 's0/\/\P4$$w0rD';

const someOtherPlaintextPassword = 'not_bacon';

To hash a password:

bcrypt.genSalt(saltRounds, function(err, salt) {

    bcrypt.hash(myPlaintextPassword, salt, function(err, hash) {

        // Store hash in your password DB.

    });
    
});