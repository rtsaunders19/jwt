# JWT

To help prepare for API authentication tomorrow, research [JSON Web Tokens](https://jwt.io) (known as JWTs). This should take about 30 minutes. Answer the following questions and submit this README as your homework:

1. What are the 3 parts of a JWT?
There is the header, the payload, and the signature. All separated by a '.'
2. What information does each part contain?
The header has two key value pairs or claims. The 'typ' which tells you it is a JWT and the 'alg' which is the algorithm used to encrypt the JWT. In the payload there are attributes defined as public claims and reserved claims. The 'iss' is the issuer which is the value of the API we are trying to access (reserved claim). The 'user' is the users username to authenticate that the user has logged on to your server. The payload usually has a lot more information than just these two things. The signature is your coded header and payload that is signed with a secret. The secret is held with the sender and the receiver so they are able to encrypt it and no one else.
3. Why do people use JWTs for authentication? A great resource to read would be https://jwt.io/introduction/.
Less data to send back and forth than XML. Very secure and hard to hack. Easy for developers to set up rather than hashing passwords themselves.
