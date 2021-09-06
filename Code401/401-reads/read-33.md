## What is JSON Web Token?

    JSON Web Token (JWT) is an open standard (RFC 7519) that defines a compact and self-contained way for securely transmitting information between parties as a JSON object. This information can be verified and trusted because it is digitally signed. JWTs can be signed using a secret (with the HMAC algorithm) or a public/private key pair using RSA or ECDSA.  it is an authentication strategy used by client/server applications where the client is a Web application using JavaScript and some frontend framework like Angular, React or VueJS.

## When should you use JSON Web Token?

    -   Authorization: This is the most common scenario for using JWT. Once the user is logged in, each subsequent request will include the JWT, allowing the user to access routes, services, and resources that are permitted with that token.

    -   Information Exchange: JSON Web Tokens are a good way of securely transmitting information between parties. 

## How does JSON Web Token work?

    The JWT is acquired by exchanging an username + password for an access token and an refresh token. The access token is usually short-lived (expires in 5 min or so, can be customized though). The refresh token lives a little bit longer (expires in 24 hours, also customizable). It is comparable to an authentication session. After it expires, you need a full login with username + password again.

## What’s The Point of The Refresh Token?

    It is necessary to make sure the user still have the correct permissions. If your access token have a long expire time, it may take longer to update the information associated with the token. That’s because the authentication check is done by cryptographic means, instead of querying the database and verifying the data. So some information is sort of cached.

## What is WSGI?

    The Web Server Gateway Interface, is a simple calling convention for web servers to forward requests to web applications or frameworks written in the Python programming language.

