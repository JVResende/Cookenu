# Cookenu

## 📄 About

Backend of a social network, where users can share relevant information about foods and recipes they have tried.

## 🔗 Deploy Link
https://lammar-cookenu2.onrender.com

## 🔗 Link to access endpoints in Postman
https://documenter.getpostman.com/view/22376488/2s93CHtZsA

## 💻 Functionalities

### Sign Up

- Creates a new user. The email must be unique, otherwise an error message will appear and it will not be created.
- The user must pass the name, email, password and role through the body.
- After creating the user, an authentication token will be generated.

### Login

- Logs the user into the application.
- The user must pass the email and password of an already registered user through the body.
- After login, an authentication token will be generated.

### Create Recipe

- Creates a new recipe.
- To be able to use this endpoint, the user must be authenticated.
- The user must pass title and description through the body.

### Follow Another User

- Endpoint to start following another user.
- To be able to use this endpoint, the user must be authenticated.
- The user must pass the userToFollowId through the body.

### Unfollow Another User

- Unfollow another user.
- To be able to use this endpoint, the user must be authenticated.
- The user must pass the userToUnfollowId through the path params.

### Delete Recipe

- Deletes a recipe.
- To be able to use this endpoint, the user must be authenticated.
- A "normal" user should be able to delete his own recipe and an "admin" user is able to delete any recipe.
- The user must pass the id of the recipe through the path params.

### Delete User

- Deletes a user.
- To be able to use this endpoint, the user must be authenticated and his role must be "admin".
- The user must pass the user id through the path params.

### Get Profile

- Returns the information of the user who is logged in.
- The user must be authenticated to use the endpoint.

### Get Recipes Feed

- Returns recipes created by users he follows.
- The user must be authenticated to use the endpoint.

### Get User By Id

- Returns the information of a specific user.
- To use this endpoint, the user must be authenticated.
- The user id must be passed by path params.

### Get Recipe By Id

- Returns the information of a specific recipe.
- To use this endpoint, the user must be authenticated.
- The id of the recipe must be passed by path params.

### Edit Recipe

- Edit a recipe.
- To use this endpoint, the user must be authenticated.
- A "normal" user should be able to edit his own recipe.
- The user must pass title and description through the body.

### Forgot Password

- This endpoint sends an email to the user who forgot his password with a new password.
- The user must pass the email through the body.

## ⚙️ Setup

Clone down this repository. You will need Node and npm installed globally on your machine.

- Installation:

```
  $ npm install 
```

- To start the project:

```
  $ npm start
```

Now you can test using the requests.rest file.

## 🛠 Technologies

- Node.js.
- TypeScript.
- MySQL.

