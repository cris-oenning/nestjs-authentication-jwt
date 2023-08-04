# Nest.Js Application with Authentication (Login System) using JWT Token

This repository contains a Nest.Js project that implements an authentication system with JWT Tokens, utilizing the following features and technologies:

- Prisma with SQLite for data persistence
- Visualization of the local database using Prisma Studio
- Thunder Client extension for testing routes
- Used libraries and dependencies:

# Dependencies and Usage

- @nestjs/passport
  @nestjs/passport is a Nest.Js module for authentication. It provides a flexible way to handle different authentication strategies, such as JWT, OAuth, and more.

- @nestjs/jwt
  @nestjs/jwt is a module that facilitates the creation and verification of JSON Web Tokens (JWT) for secure authentication and authorization in protected routes.

- bcrypt
  The bcrypt library is used to securely hash and verify passwords. This helps protect user passwords stored in the database.

- class-validator
  class-validator is a library that offers an easy way to validate TypeScript objects based on classes, ensuring that data meets certain criteria before processing.

- class-transformer
  class-transformer allows you to transform and validate complex objects, such as database entities, into simpler representations like JSON objects, and vice versa.

- passport and passport-related packages
  passport is an authentication middleware for Node.js that works well with Nest.Js. The dependencies passport-jwt, passport-local, @types/passport-jwt, and @types/passport-local are used to implement different authentication strategies, such as JWT-based authentication and local authentication.

# Execution Steps

Follow the steps below to run the application on your machine:

1 - Clone the repository.

2 - Install dependencies:
Navigate to the project directory and execute the following command to install dependencies:

npm install

3 - Configure the Database:
Make sure you have SQLite installed on your machine. Then, run migrations to create the database:

npx prisma migrate dev

4 - Run Prisma Studio:
Use Prisma Studio to visualize the database on localhost:

npx prisma studio

5 - Set Environment Variables:
Rename the .env.example file to .env and fill in the environment variables as needed.

6 - Run the Application:
Start the development server:

npm run start:dev

# Using Thunder Client

The Thunder Client extension in Visual Studio Code can be used to test the application's routes. Import the available requests from the thunder_client_requests.json file to start testing authentication functionalities.

# Project Structure

The project structure follows Nest.Js conventions:

- src/auth: Contains components related to authentication (strategies, guards, controllers, and services).
- src/user: Defines the user resource, including controllers and services to manage users.
- src/app.module.ts: Main configuration file of the application.
- src/main.ts: Entry point of the application.

# Importance of Security

Application security is of utmost importance. Make sure to follow best security practices when developing and deploying your Nest.Js project. Using JWT-based authentication, encrypting passwords, and validating inputs are some of the recommended practices to ensure the security of data and users.

Always remember to keep your dependencies up to date and perform regular security audits.

This project was developed based on the latest technologies and practices to ensure the security and efficiency of the application. Feel free to explore, contribute, and customize according to your needs.
