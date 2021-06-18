## User Stories

#### Feature One : 
As a user i want to be able to create an account. and sign in into that account, as well as having the ability to edit my information in the account. 
    **Feature Tasks:** 
        1. Create a form to allow users to sign up and sign in. 
        2. Save the user's information in the Database.
        2. Authenticate the user signing
        3. Authorize the user to edits his own profile and requests.

#### Feature Two : 
As a user i want to be able to send a request for a partner. 
    **Feature Tasks:** 
        1. Create a form to be filled by the user if he wants to send for a partner.
        2. Enable The user to specify in what field by implementing a dynamic list.
        3. The request is then saved into the database.

#### Feature Three : 
As a user i want to be able to check and search partners request shared by other users and to be able to join them.
    **Feature Tasks:** 
        1. Requests for partners will be displayed.
        2. Search bar to search through the request based on a specific criteria. 
        3. Button next to each request to allow users to pick that request.

#### Feature Four : 
As a user i want to receive a notification when ever the another user chooses to be my partner.
    **Feature Tasks:** 
        1. An event listener will be connect to the select button.
        2. A notification will be sent to the owner of request whenever some clicks on that button

#### Feature Five : 
As a user i want to be able to connect my partner in a suitable and easy way.
    **Feature Tasks:** 
        1. Implement rooms to allow partners to connect to each by chatting or video chat.
        2. Allow messages to stay in queue until seen by the other user. 

### Feature Six:
As a user i want to have the ability to approve or reject other user's request to my partner request
    **Feature Tasks:** 
        1. An event listener will be connect to the approve or reject button.
        2. approved user will have the ability to connect and join the other user
        3. rejected users request will be removed from the database.
