### Review, Research, and Discussion

1. When is Basic Authorization used vs. Bearer Authorization?
 * The Basic and Digest authentication schemes are dedicated to the authentication using a username and a secret (see RFC7616 and RFC7617). The Bearer authentication scheme is dedicated to the authentication using a token and is described by the RFC6750

 ![img](https://i.stack.imgur.com/HQF1L.png)


2. What does the JSON Web Token package do?
  * A JSON Web Token is used to send information that can be verified and trusted by means of a digital signature. It comprises a compact and URL-safe JSON object, which is cryptographically signed to verify its authenticity, and which can also be encrypted if the payload contains sensitive information.
  ![img](https://miro.medium.com/max/1200/1*u3a-5xZDeudKrFGcxHzLew.png)


3. What considerations should we make when creating and storing a SECRET?
  * Storing the secret someplace secure, (.env files are good) and storing secrets with some level of encryption.

## Terms 

* encryption => Encryption is a means of securing digital data using one or more mathematical techniques, along with a password or "key" used to decrypt the information. ... For example, websites that transmit credit card and bank account numbers should always encrypt this information to prevent identity theft and fraud.
* token => A security token (sometimes called an authentication token) is a small hardware device that the owner carries to authorize access to a network service. The device may be in the form of a smart card or may be embedded in a commonly used object such as a key fob. ... Unlike a password, a security token is a physical object.
* bearer => According to RFC6750-The OAuth 2.0 Authorization Framework: Bearer Token Usage, the bearer token is: A security token with the property that any party in possession of the token (a "bearer") can use the token in any way that any other party in possession of it can.
* secret => The secret key method of encryption, which involves the use of a single key, is used to encrypt and decrypt the information and is sometimes referred to as symmetric key cryptography.
* JSON Web Token => A JSON Web Token is used to send information that can be verified and trusted by means of a digital signature. It comprises a compact and URL-safe JSON object


1. Which 3 things had you heard about previously and now have better clarity on?
  * JSON Web Token

2. Which 3 things are you hoping to learn more about in the upcoming lecture/demo?
  * bearer auth
3. What are you most excited about trying to implement or see how it works?
  * code challenges are my fav
 

