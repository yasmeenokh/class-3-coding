
# Heroku Deploy
[logo](http://photos.prnewswire.com/prnfull/20110712/SF33967LOGO?max=200)

Heroku is a cloud platform as a service supporting several programming languages. it is a container-based cloud Platform as a Service (PaaS). Developers use Heroku to deploy, manage, and scale modern apps.

![heroku](https://lh3.googleusercontent.com/proxy/ETkzOeBqo1zFvRQWO1ZsRvuwpLhwVX2sCO1Y_2FTFTG3aC88dPYsEyc-M3XsnVr8i_aaZ0RkvXFqBoAxwcBbMSxqa0C_T_ih6g6dX7HT2FBX9GNwGk-JdJy9J9Kk7kBZreEacTBhgQXi)

## focus on apps 
Heroku is the quickest way for a company to become an apps company. Heroku is a service that enables companies to spend their time developing and deploying apps that immediately start producing value.

## Node JS
Node.js is an open source, cross-platform runtime environment, which allows you to build server-side and networking applications. It’s written in JavaScript and can be run within the Node.js runtime on any platform.

## Set up
1. install heroku in the terminal.
2. Command opens your web browser to the Heroku login page.
3. Command creates an app on Heroku, which prepares Heroku to receive source code.
4. Command deploys your code.
5. Command ensures that at least one instance of the app is running.
6. Command allows to visit deployed app

**NOTE**
you can view information about the running app by running this code **heroku logs --tail**.


### Run the following from your terminal: 
$ sudo snap install heroku --classic When installation completes, you can use the heroku command from your terminal.
On Windows, start the Command Prompt (cmd.exe) or Powershell to access the command shell. Use the heroku login command to log in to the Heroku CLI:

This command opens your web browser to the Heroku login page. 

This authentication is required for both the heroku and git commands to work correctly.

$ node --version

$ npm --version

$ git --version

Prepare the app $git clone
$ cd node-js-getting-started

$ heroku create

$ git push heroku main

$ heroku ps:scale web=1

$ heroku open

$ heroku logs --tail

web: npm start

**Scale the app** 
$ heroku ps

$ heroku ps:scale web=0

$ heroku ps:scale web=1

**Declare app dependencies**
Heroku recognizes an app as Node.js by the existence of a package.json file in the root directory. For your own apps, you can create one by running npm init --yes.

Run this command in your local directory to install the dependencies, preparing your system for running the app locally: $ npm install

Run the app locally
$ heroku local web

Push local changes
$ npm install cool-ascii-faces




