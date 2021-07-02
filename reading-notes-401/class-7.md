## Modern Token Authentication in Node with Express

![img](https://res.cloudinary.com/practicaldev/image/fetch/s--pYFra1r_--/c_imagga_scale,f_auto,fl_progressive,h_420,q_auto,w_1000/https://thepracticaldev.s3.amazonaws.com/i/r6vazxuvcmeuh6044zo0.png)

###### Token authentication is the hottest way to authenticate users to your web applications nowadays. There’s a lot of interest in token authentication because it can be faster than traditional session-based authentication in some scenarios, and also allows you some additional flexibility. In this post, I’m going to teach you all about token authentication: what it is, how it works, why you should use it, and how you can use it in your Node applications. Let’s get to it!

### What Is Token Authentication?

###### Token authentication is a way to authenticate users into an application using a temporary token (typically a JSON Web Token) instead of actual credentials.

###### The way this works in the context of web authentication is like so:

- A user wants to log into a website
- A user supplies their email address and password to the website (their credentials)
- The website generates a token for the user
- The user’s browser stores the token
- When the user makes subsequent requests to the website, their token will be sent along with their request
- The website will validate the token and use it to figure out who the user is

###### The benefit of this approach is that tokens contain embedded information about the user, so the website can receive the token and discover who the user is and what permissions they have without necessarily needing to talk to a central database. This means you may not need to maintain a session store.

###### Here’s a visualization of what the flow typically looks like:

![img](https://res.cloudinary.com/practicaldev/image/fetch/s--ynel2BK2--/c_limit%2Cf_auto%2Cfl_progressive%2Cq_auto%2Cw_880/https://developer.okta.com/assets-jekyll/blog/node-token-auth/token-authentication-flow-69804c12334715c597128cd9273bca5e32ed516b62987902310efc54d1840a40.png)

### What are JSON Web Tokens?

###### Before we talk about JSON Web Tokens, let’s clarify some terms:

###### Authentication is the process of verifying a user’s identity.

###### A token is an object that can be used to authenticate a user to a server. Tokens contain embedded user data that is used to identify and authenticate the user.

###### JSON Web Tokens (JWTs) are an open standard [(learn more about JWTs here)](https://developer.okta.com/blog/2018/06/20/what-happens-if-your-jwt-is-stolen) that define a secure way to transmit information between parties using a JSON object. JWTs are always cryptographically signed (sometimes encrypted) and can be signed using a secret key (symmetrical) or a public/private key pair (asymmetrical).

###### JWTs are the most popular type of tokens and are often what people mean when they refer to “token authentication” in general.

###### Here’s what a typical JWT might look like in it’s compacted, URL-safe form:

<div class="highlight"><pre class="highlight plaintext"><code>eyJraWQiOiJ1dURLVTMxZWRvTi0wd0xMUnl1TW1vbmtBdi1OaFEwejZhWmxjdTN5NU8wIiwiYWxnIjoiUlMyNTYifQ.eyJ2ZXIiOjEsImp0aSI6IkFULnVfT094R3pXd1RjRFlseGZwcDVYXzNxdVIwdlJuc25YbXdMZld0TDFjdG8iLCJpc3MiOiJodHRwczovL2Rldi04MTk2MzMub2t0YXByZXZpZXcuY29tL29hdXRoMi9kZWZhdWx0IiwiYXVkIjoiYXBpOi8vZGVmYXVsdCIsImlhdCI6MTU0NjcyNjIyOCwiZXhwIjoxNTQ2NzI5ODI4LCJjaWQiOiIwb2Fpb3g4Ym1zQktWWGt1MzBoNyIsInNjcCI6WyJjdXN0b21TY29wZSJdLCJzdWIiOiIwb2Fpb3g4Ym1zQktWWGt1MzBoNyJ9.fhZRWThFxhiS6Pgrup6hM08oSqDPd1JrZSDIH_blD5S20c2hQQ3D3RZyhNKMnYclyus_mo-H-mS-Ak3YzM8S0JwZ8m3Vid4smW953peBMnmBNotAE--yE0toc2dIUG3BWQR34hah253bKmp17Yh6bWGwH60oQxnuM_NVUpa-NJMBc6-Mu5ra0lKfr60ne9-jKVFcavd9ZnVTLiug_sXFlhxgaQm4V_hhcvcLSwCXTiIcQsJkI0rP7WuVvjYVyK_sPeW3A44_T5qhyDR_E_mk1rHORlkMYGPg34mcwob5iA7alNZOnzN_7ApcbylDbK5KS1umBqqevtghEyjOEWQQmQ

</code></pre></div>

###### While this may look complicated and unreadable at first glance, it isn’t actually all that tricky! JWTs consist of three parts, separated by dots (.): xxxxxx.yyyyyy.zzzzzz. These sections represent the JWT header, payload, and signature, respectively.

### Review, Research, and Discussion

#### Explain what a “Singleton” is (in Computer Science terms)

[Singleton in JavaScript](https://dev.to/tomekbuszewski/singleton-in-javascript-1d5i)

###### A Singleton is an object which can only be instantiated one time. Repeated calls to its constructor return the same instance and in this way one can ensure that they don't accidentally create, say, two Users in a single User application.

#### Explain how the Singleton pattern can be used with Node modules, specifically with classes

[Singleton Pattern in JavaScript](https://dev.to/aakatev/singleton-pattern-in-javascript-31gd)

###### The Singleton Pattern limits the number of instances of a particular object to just one. This single instance is called the singleton.

##### If you were tasked with building a middleware system like Express uses, what approach might you take to construct/operate it?

## Term

- Router Middleware => Router level middleware can be defined in the same way as application-level middleware

- Dynamic Module Loading => The dynamic module loader library allows code to retrieve Node modules from a web server, install them locally and serve them up as though they'd been manually deployed to the running server.
- Singleton Pattern => The Singleton Pattern limits the number of instances of a particular object to just one. This single instance is called the singleton.

- Mock Testing => Mock testing is an approach to unit testing that lets you make assertions about how the code under test is interacting with other system modules. In mock testing, the dependencies are replaced with objects that simulate the behaviour of the real ones. ... Such a service can be replaced with a mock object.

## Preview

- Which 3 things had you heard about previously and now have better clarity on?

  - bcrypt
  - auth
  - express router

- Which 3 things are you hoping to learn more about in the upcoming lecture/demo?
  - testing
  - linked list
- What are you most excited about trying to implement or see how it works?
  - bcrypt
  - auth
