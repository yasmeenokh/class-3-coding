# Sending form data

##  defining how to send the data
The <form> element defines how the data will be sent. All of its attributes are designed to let you configure the request to be sent when a user hits a submit button. The two most important attributes are action and method.

- action => defines where the data gets sent. Its value must be a valid relative or absolute URL. 

- method => defines how data is sent. The HTTP protocol provides several ways to perform a request; HTML form data can be transmitted via a number of different methods, the most common being the GET method and the POST method. 

**GET** : is the method used by the browser to ask the server to send back a given resource.

**POST** : It's the method the browser uses to talk to the server when asking for a response that takes into account the data provided in the body of the HTTP request.

**NOTE**
1. If you need to send a password (or any other sensitive piece of data), never use the GET method or you risk displaying it in the URL bar, which would be very insecure.

2. If you need to send a large amount of data, the POST method is preferred because some browsers limit the sizes of URLs. In addition, many servers limit the length of URLs they accept.

### sending files
1. Set the method attribute to POST because file content can't be put inside URL parameters.

2. Set the value of enctype to multipart/form-data because the data will be split into multiple parts, one for each file plus one for the text data included in the form body (if text is also entered into the form).

3. Include one or more <input type="file"> controls to allow your users to select the file(s) that will be uploaded.

### Security issues
Escape potentially dangerous characters. The specific characters you should be cautious with vary depending on the context in which the data is used and the server platform you employ, but all server-side languages have functions for this. 