# OAuth
![logo](https://upload.wikimedia.org/wikipedia/commons/thumb/d/d2/Oauth_logo.svg/598px-Oauth_logo.svg.png)

**OAuth**: is “an open standard for access delegation” … In other words, OAuth serves as a way to give users the ability to grant application access to services, without giving the application their password.

- Through a series of “handshakes”, an application such as an Express Web Server asks the user if it’s ok to log in as them at some remote service, and then begins the process of authentication and access.

- Remote service (i.e. Google) contacts the application with a one-time-use Code

- OAuth allows third-party services to exchange your information without you having to give away your password. Because the more you give away your password, the more you give away your passwords, the more likely it is that your passwords will get compromised.

## How OAuth works?
OAuth uses a system of tokens. Called “access tokens”. An access token gives one third-party source temporary access to a limited amount of your personal information on another third-party source.
![workflow](https://a.slack-edge.com/fbd3c/img/api/articles/oauth_scopes_tutorial/slack_oauth_flow_diagram.png)

## Who uses OAuth?
examples: Amazon, AOL, Bitly, Dailymotion, Etsy, Facebook, Goodreads, Google App Engine, Instagram, LinkedIn, Microsoft, Netflix, Tumblr, Twitter, Vimeo, WordPress, Yahoo!
![user](https://miro.medium.com/max/3344/1*Fn8AOf3awPM0EDmpVJCNhg.png)
## Access Code
First, the client needs to grant the application permission. To do this you need to provide a tag that will take them to the service’s authorization page. the tag should pass the following information through a query string to the authorization server.

## Access Token
If the users grant access to the application, the authorization server will redirect to a provided redirect URI callback with a “code”. Once you have this code, you can exchange it for an access token by making a POST request to the authorization server

## Security Benefits
The signup process (and storing passwords) is not lightweight livability. if an app can relieve itself from that, it would be a great plus.

- That is why opting for OAuth is sometimes a better option than simply architecting a signup process.

- Also, it ensures users cannot spam new accounts as they like. for example, if a website is intended for programmers, using OAuth with GitHub is a great choice. their information will be migrated and their profiles will be ready in a second.

- Some users actually like that relieving them from having to create new profiles and bios and whatnot!