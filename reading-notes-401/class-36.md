# Application State with Redux


## Review, Research, and Discussion

1. What are the advantages of storing tokens in “Cookies” vs “Local Storage”
  * Local storage is vulnerable because it’s easily accessible using JavaScript and an attacker can retrieve your access token and use it later. However, while httpOnly cookies are not accessible using JavaScript, this doesn't mean that by using cookies you are safe from XSS attacks involving your access token.

* Explain 3rd party cookies.
    - cookies that are set by a website other than the one you are currently on.

1. How do pixel tags work?
  - Pixels are used to identify groups of users based on actions that they take on a website

## Vocab

* cookies
  * These are 4kb files that persist between pages
  * They store information in key:value pairs and can be persisted

* authorization
  * This is the process of allowing/denying access to resources
* access control
  * This is typically a list of permissions sometimes based on a user's role. Access control adds a second layer of defense after authentication.
* conditional rendering
  * Something is conditionally rendered if it's dependent on some conditional logic.




[Dan Abramov – Redux Tutorials](https://egghead.io/courses/fundamentals-of-redux-course-from-dan-abramov-bd5cc867)

[what-is-redux](https://dev.to/mmeurer00/what-is-redux-toolkit-b94)