# Deployment Guide for Real Estate Investment Platform

## Heroku Setup

1. **Create a Heroku Account**: If you haven't already, sign up for a free account on [Heroku](https://www.heroku.com/).
2. **Install Heroku CLI**: Download and install the [Heroku Command Line Interface (CLI)](https://devcenter.heroku.com/articles/heroku-cli).
3. **Login to Heroku**: Open your terminal and run:
   ```bash
   heroku login
   ```
4. **Create a New Application**:
   ```bash
   heroku create your-app-name
   ```
5. **Set Configuration Variables**:
   Set your environment variables using the CLI:
   ```bash
   heroku config:set VARIABLE_NAME=value
   ```

## MongoDB Atlas Configuration

1. **Create a MongoDB Atlas Account**: Sign up for MongoDB Atlas at [MongoDB Atlas](https://www.mongodb.com/cloud/atlas).
2. **Create a Cluster**: Follow the prompts to create a new cluster.
3. **Set Up Database User**: Add a new database user with password access.
4. **Whitelist IP Address**: Allow your IP address in the Network Access settings.
5. **Connect to Application**: Use the connection string provided by Atlas and update it in Heroku Config Vars.

## API Endpoints

- **GET /api/properties**: Retrieve list of all properties.
- **POST /api/properties**: Add a new property.
- **GET /api/properties/:id**: Retrieve details of a specific property.
- **PUT /api/properties/:id**: Update a specific property.
- **DELETE /api/properties/:id**: Delete a specific property.

## Initial Setup Instructions

1. **Clone the Repository**:
   ```bash
   git clone https://github.com/seiduabubakar1/Goodwall-
   ```
2. **Navigate to Project Directory**:
   ```bash
   cd Goodwall-
   ```
3. **Install Dependencies**:
   ```bash
   npm install
   ```
4. **Run the Application**:
   ```bash
   npm start
   
5. **Access the Application**: Open your browser and go to `http://localhost:PORT` to view your application.

## Conclusion

This document provides a complete guide for deploying the Real Estate Investment Platform on Heroku with MongoDB Atlas configuration. Follow the instructions to ensure a successful deployment.