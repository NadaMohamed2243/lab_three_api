# Lab Three API

## Description
This project implements a simple application using scaffolding for **User 1:M Post**. The repository is created to demonstrate CRUD functionality for managing users and posts. The project follows the API-only mode with all necessary associations, and APIs are created using Postman.

## Project Setup

### 1. Create the App with Scaffold and Associations

Run the following command to create the app:

```bash
rails new lab_three_api --api
```

Then, scaffold the User and Post models, ensuring the necessary associations are set:

```bash
rails generate scaffold User name:string email:string
rails generate scaffold Post title:string content:text user:references
```

The User model will have a has_many relationship with the Post model, and the Post model will belong to the User.

After generating the models, run the migrations:

```bash
rails db:migrate
```

This will set up the tables in your database.

2. Create APIs with Postman
Start the server by running:

```bash
rails server
```

Use Postman to create, read, update, and delete users and posts.

Add the API routes for users and posts in the Postman tool.

Test each CRUD operation to ensure everything works correctly.

APIs
Here are the available APIs for CRUD operations:

Users

GET /users: Retrieve all users

POST /users: Create a new user

GET /users/:id: Retrieve a single user by ID

PUT /users/:id: Update an existing user

DELETE /users/:id: Delete a user

Posts

GET /posts: Retrieve all posts

POST /posts: Create a new post

GET /posts/:id: Retrieve a single post by ID

PUT /posts/:id: Update an existing post

DELETE /posts/:id: Delete a post

