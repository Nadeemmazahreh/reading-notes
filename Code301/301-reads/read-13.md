## In your own words, describe what each group of status code represents:
    - 100’s = These are informational status codes, to tell the client that the reqest has been recieved
    - 200’s = These are the success codes, to tell the client that the request has been accepted
    - 300’s = These are redirection codes, to tell the client that the recources aren't available at the specified location anymore
    - 400’s = These are the client error codes, to tell the client that the request is invalid
    - 500’s = These are the server error codes, often problebs with the server 

## What is a status code 202?
    202 Accepted - If the deletion is asynchronous and takes some time, which is the case in distributed systems, it can be appropriate to return this code with some information or URL to tell the client when it will be deleted.

## What is a status code 308?
    Permanent Redirect - This is the right code if the resource will now be available at a new URL and the client should directly access it via the new URL in the future. The current endpoint can’t control the clients’ behavior after the request and a subsequent redirect if the resource URL changes again have to be issued from the new URL.

## What code would you use if an update didn’t return data to a client?
    204 

## What code would you use if a resource used to exist but no longer does?
    308 

## What is the ‘Forbidden’ status code?
     The client has authorized or doesn’t need to authorize itself, but still has no permissions to access the resource.