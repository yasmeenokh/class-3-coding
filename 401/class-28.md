# Review, Research, and Discussion

1. Why is the Context API useful?

it is useful because it helps in passing the data (states or others) from parent to all the children without the need of props.

2. Can a component outside of a provider get its context?

No

3. What are some common use cases for using the Context API?
Describe “Context Hell”

To put some specific configuration and allow changing it easily by the user.

4. Describe “Context Hell”.

the React Context hell is the nasty code you get taking advantage of the React Context API (Providers inside Providers).




# Vocabulary Terms

**global state"** State of Component that is used and accessible by other Component.

**global context:** Context Provider that is used for the whole App and wrap all the components.

**provider:** Context API that is considered as (parent) and share it's state to all its children.

**consumer:** Context API that is considered as (Child) and have access to whatever the parent is sharing.

# Preview

## What is Role-Based Access Control (RBAC)? 

**DEFINITION:**

Role-based access control (RBAC) restricts network access based on a person's role within an organization and has become one of the main methods for advanced access control. The roles in RBAC refer to the levels of access that employees have to the network.

**BENEFITS OF RBAC**

1. Reducing administrative work and IT support
2. Maximizing operational efficiency.
3. Improving compliance.

## react-cookies

**To be able to access user cookies while doing server-rendering, you can use plugToRequest or setRawCookie.**

**How to Set a cookie value :**

    setCookie(name, value, [options])

* name (string): cookie name
* value (string	object): save the value and stringify the object if needed
options (object): Support all the cookie options from RFC 6265
* path (string): cookie path, use / as the path if you want your cookie to be accessible on all pages
* expires (Date): absolute expiration date for the cookie
* maxAge (number): relative max age of the cookie from when the client receives it in seconds
* domain (string): domain for the cookie (sub.domain.com or .allsubdomains.com)
* secure (boolean): Is only accessible through HTTPS?
* httpOnly (boolean): Can only the server access the cookie?
* sameSite (boolean	none	lax	strict): Strict or Lax enforcement

**How to Remove a cookie :**

    removeCookie(name, [options])

* name (string): cookie name
* options (object): Support all the cookie options from RFC 6265
* path (string): cookie path, use / as the path if you want your cookie to be accessible on all pages
* expires (Date): absolute expiration date for the cookie
* maxAge (number): relative max age of the cookie from when the client receives it in seconds
* domain (string): domain for the cookie (sub.domain.com or .allsubdomains.com)
* secure (boolean): Is only accessible through HTTPS?
* httpOnly (boolean): Can only the server access the cookie?
* sameSite (boolean	none	lax	strict): Strict or Lax enforcement


**How to Give access to your cookies anywhere :**

    withCookies(Component)

* cookies: Cookies instance allowing you to get, set and remove cookies.
* allCookies: All your current cookies in an object.
