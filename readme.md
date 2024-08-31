# User Registration System

## Overview

This project is an Express.js application designed to handle user registration requests. It includes custom validation logic and an error handling middleware to ensure that the provided input data meets specific requirements. The application is intended to accept requests from Postman or any other API client for user registration.

## Features

- Validates that the first and last names start with an uppercase letter.
- Ensures the password contains at least one special character, one uppercase letter, one numeric character, and is a minimum of 8 characters long.
- Validates that the email address contains an "@" symbol.
- Checks that the phone number is at least 10 digits long.
- Returns detailed error messages if any validation criteria are not met.

## Prerequisites

- [Node.js](https://nodejs.org/) (version 14 or later)
- [npm](https://www.npmjs.com/)

## Getting Started

## Installation

1. Clone the repository:

   ```bash
   git clone `https://github.com/yatikbudhrani/ErrorHandlingMiddlewareforUserRegistration.git`
   ```

2. Navigate to the project directory:

   ```bash
   cd ErrorHandlingMiddlewareforUserRegistration
   ```

3. Install dependencies:

   ```bash
   npm install
   ```

4. Start the server:

   ```bash
   node index.js
   ```

5. The server will run on `http://localhost:3000`.

## API Endpoints

- **POST** `/register`: Request Body should be of the format-  
-       {  
         "firstName": "John",  
         "lastName": "Doe",  
         "password": "Secure@123",  
         "email": "john.doe@example.com",  
         "phoneNumber": "1234567890"  
        }

## Testing

You can test the API using Postman or curl:

- **Postman**: Make a POST request to `http://localhost:3000/register
