# JWT authentication with Node, Express, and MongoDB

Almost all Websites in the world have user authentication. In this project, you have to make a REST API implementing the user's authentication using javascript and the NodeJS framework with Express, you also have to implement the necessary changes to store data in the database and use MongoDB.

Using the previous code of the tasks API is recommended to start the development since it meets all the necessary endpoints, and you will only have to add 2 additional endpoints and create a middleware that will have to validate that the user is valid inside our REST API.

## 🗒️ Instructions

Implement an authentication system in the following steps:

1. **Registration**: the user should be able to put an email, any password and send the form. A new user must be created in the database and the user must be redirected to log in after this.

2. **Login**: the user must fill in their mail and password, and it must be redirected to a private menu after the authentication is successful.

3. **Validation**: Any page considered private should always be validating that the current user is validated via middleware, if not, it must return an error message that says that the endpoint is private

At least the following pages and react components must be implemented in the project:

| Route       | Method     | Functionality                                                           |
| ------------- | ----------- | -----------------------------------------------------------------------  |
| `/signup`.    | `POST`      | Route that allows me to register in REST
| `/signin`.    | `POST`      | Route that allows me to login into the REST API
| `/todos`      | `GET`       | To-do list (public)                                             |
| `/todos`      | `POST`      | Route that allows me to create a task in theREST API (private)          |
| `/todos/:id`  | `PUT`       | Route that allows me to update a task in the REST API (private)    |
| `/todos/:id`  | `DELETE`    | Route that allows me to delete a task in the REST API (private)    |

## More details about the authentication:

Usually, an authentication system is implemented in 4 parts:

![authentication diagram](https://github.com/breatheco-de/jwt-authentication-with-flask-react/blob/main/.learn/login_diagram.jpeg?raw=true)





