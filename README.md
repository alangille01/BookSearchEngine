# MERN Book Search Engine

This is a refactored book search engine built using the MERN stack (MongoDB, Express, React, Node.js). The project was originally built with a RESTful API and has been refactored to use GraphQL API with Apollo Server for querying and mutations.

## Table of Contents
- [Description](#description)
- [Features](#features)
- [Installation](#installation)
- [Usage](#usage)
- [Deployment](#deployment)
- [Technologies Used](#technologies-used)
- [License](#license)

## Description
The Book Search Engine allows users to search for books using the Google Books API, save books to their personal profile, and view saved books. The application has been refactored from a RESTful API to use GraphQL and Apollo Server. Users can log in, search for books, and save their favorite ones for later viewing.

## Features
- User authentication using JWT (JSON Web Tokens)
- Search for books using the Google Books API
- Save favorite books to a personal profile
- View and delete saved books
- Responsive design for mobile and desktop devices

## Installation 

If you are interested in running the application locally, please use the following steps:
1. Clone this repository to your local machine. (For reference, visit the [Cloning a Repository](https://docs.github.com/en/repositories/creating-and-managing-repositories/cloning-a-repository) GitHub Docs article.)
2. Run `npm install && npm run build` in your CLI to download the npm package dependencies and build the app using vite.
3. Run `npm run develop` to start up the backend and serve the client.
4. Navigate to `http://localhost:3000` on your local web browser to use the application. 

## Usage
- Open your browser and navigate to `http://localhost:3000` to access the application.
- Use the search bar to search for books using the Google Books API.
- Create an account or log in to save your favorite books and view your saved collection.

See Deployed App on [Render](https://booksearchengine-7l7c.onrender.com/)

## Deployment
To deploy the application to [Render](https://render.com):

1. Create a new **Web Service** on Render and link it to your GitHub repository.
2. Set the following environment variables in Render's settings:
    - `MONGODB_URI`
    - `JWT_SECRET`
    - `REACT_APP_GRAPHQL_ENDPOINT`
3. Set the **Build Command** to:
    ```bash
    npm install --legacy-peer-deps && npm run build
    ```
4. Set the **Start Command** to:
    ```bash
    npm start
    ```
5. Render will handle the deployment process. Once deployed, you will get a live URL for your app.

## Technologies Used
- **MongoDB**: For database and storing user and book data
- **Express.js**: Backend framework to handle routing and GraphQL API
- **React.js**: Frontend library to build user interfaces
- **Node.js**: Backend runtime environment
- **Apollo Server**: For handling GraphQL queries and mutations
- **JWT**: JSON Web Tokens for authentication
- **Google Books API**: To fetch book data

## License
This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for more details.
