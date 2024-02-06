# Jobly Backend

## Overview

Jobly Backend is the server-side component of the Jobly application, responsible for handling data storage, authentication, and API endpoints.

## Technologies Used

- **Express**: Fast, unopinionated, minimalist web framework for Node.js.
- **Cors**: Cross-Origin Resource Sharing middleware for Express.
- **Jsonwebtoken**: JSON Web Token implementation for Node.js.
- **Bcrypt**: Library for hashing passwords.
- **Pg**: PostgreSQL client for Node.js.
- **Dotenv**: Module for loading environment variables from a .env file into process.env.
- **Colors**: Library for adding color to console output.
- **Morgan**: HTTP request logger middleware for Node.js.
- **Jsonschema**: JSON schema validator.

## Setup

1. Clone the repository.
2. Install dependencies using `npm install`.
3. Create a `.env` file in the root directory and add necessary environment variables (e.g., database connection details, JWT secret).
4. Start the server with `npm start`.
5. The server will be running at the specified port (default: 3001).
6. Query endpoints with Insomnia or any other tool.
7. To interact with the API on a client please visit the frontend repo [here](https://github.com/brendenGit/jobly-frontend)

## Database Setup

1. Install PostgreSQL if not already installed.
2. Create a new database for Jobly.
3. Update the `.env` file with the database connection details.

## API Endpoints

### Authentication

- #### POST /auth/token
  - Returns a JWT token for authentication.

- #### POST /auth/register
  - Registers a new user.

### Companies

- #### POST /companies
  - Adds a new company.

- #### GET /companies
  - Returns a list of all companies.

- #### GET /companies/:handle
  - Returns details of a specific company.

- #### PATCH /companies/:handle
  - Updates details of a specific company.

- #### DELETE /companies/:handle
  - Deletes a specific company.

### Jobs

- #### POST /jobs
  - Adds a new job.

- #### GET /jobs
  - Returns a list of all jobs.

- #### GET /jobs/:id
  - Returns details of a specific job.

- #### PATCH /jobs/:id
  - Updates details of a specific job.

- #### DELETE /jobs/:id
  - Deletes a specific job.

### Users

- #### POST /users
  - Adds a new user.

- #### GET /users
  - Returns a list of all users.

- #### GET /users/:username
  - Returns details of a specific user.

- #### PATCH /users/:username
  - Updates details of a specific user.

- #### DELETE /users/:username
  - Deletes a specific user.

- #### POST /users/:username/jobs/:id
  - Applies for a job.


## Contributing

Contributions are welcome! Please fork the repository and submit pull requests with any improvements, bug fixes, or new features.

