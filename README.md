# Coffee Shop Full Stack

## Full Stack Nano - IAM Final Project

Udacity has decided to open a new digitally enabled cafe for students to order drinks, socialize, and study hard. But they need help setting up their menu experience.

You have been called on to demonstrate your newly learned skills to create a full stack drink menu application. The application must:

1. Display graphics representing the ratios of ingredients in each drink.
2. Allow public users to view drink names and graphics.
3. Allow the shop baristas to see the recipe information.
4. Allow the shop managers to create new drinks and edit existing drinks.

## Tasks

There are `@TODO` comments throughout the project. We recommend tackling the sections in order. Start by reading the READMEs in:

1. [`./backend/`](./backend/README.md)
2. [`./frontend/`](./frontend/README.md)

## About the Stack

We started the full stack application for you. It is designed with some key functional areas:

### Backend

The `./backend` directory contains a partially completed Flask server with a pre-written SQLAlchemy module to simplify your data needs. You will need to complete the required endpoints, configure, and integrate Auth0 for authentication.

[View the README.md within ./backend for more details.](./backend/README.md)

### Frontend

The `./frontend` directory contains a complete Ionic frontend to consume the data from the Flask server. You will only need to update the environment variables found within (./frontend/src/environment/environment.ts) to reflect the Auth0 configuration details set up for the backend app.

[View the README.md within ./frontend for more details.](./frontend/README.md)

## Auth0 Setup
### Create Auth0 Application
![application](./images/application.png)

### Create Auth0 API and Permissions
![api_permissions](./images/api_permissions.png)

### Create Auth0 Roles and Users
![role](./images/role.png)

## Backend
### Install Dependencies
```
cd backend
pip install -r requirements.txt
```
### Run Backend Server
```
cd src
flask run
```
URL backend: http://localhost:5000/

## Frontend
### Install Dependencies
```
cd frontend
npm install
```

### Run Frontend Server
```
ionic serve
```
URL Frontend: http://localhost:8100

***Node:<br>***
`Because this project uses a fairly old library, when running the frontend server with a new node.js version like 20.8.0, do the following:`
#### On Windows with Command Prompt
```
set NODE_OPTIONS=--openssl-legacy-provider

ionic serve
```

### Sign In Page
![signin](./images/sign_in.png)

### Redirect to Auth0
![redirect](./images/redirect.png)

### Home Page
![home_page](./images/home_page.png)

### Create Drink
![create_drink](./images/create_drink.png)

### Edit Drink
![edit_drink](./images/edit_drink.png)