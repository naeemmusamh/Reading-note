# OAuth

OAuth allows websites and services to share assets among users. It is widely accepted, but be aware of its vulnerabilities.

OAuth is an framework that describes how unrelated servers and services can safely allow authenticated access to their assets without actually sharing the initial, related, single logon credential.

## OAuth examples

The simplest example of OAuth is when you go to log onto a website and it offers one or more opportunities to log on using another website’s/service’s logon. You then click on the button linked to the other website, the other website authenticates you, and the website you were originally connecting to logs you on itself afterward using permission gained from the second website.

## OAuth explained

can be helpful to remember that OAuth scenarios almost always represent two unrelated sites or services trying to accomplish something on behalf of users or their software.

## How OAuth works

a user has already signed into one website or service. The user then initiates a feature/transaction that needs to access another unrelated site or service.

1. The first website connects to the second website on behalf of the user.

2. The second site generates a one-time token and a one-time secret unique to the transaction and parties involved.

3. The first site gives this token and secret to the initiating user’s client software.

4. The client’s software presents the request token and secret to their authorization provider.

5. If not already authenticated to the authorization provider, the client may be asked to authenticate.

6. The user gives the approved access token to the first website, access token at the first website.

![OAuth](https://github.com/naeemmusamh/Reading-note/blob/master/IMAGE/401/OAuth.jpg?raw=true)
