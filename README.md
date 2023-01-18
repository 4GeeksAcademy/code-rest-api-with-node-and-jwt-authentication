<!--hide-->
# JWT authentication with Node, Express and MongoDB
<!--endhide-->

Almost all websites in the world have user authentication, in this project you must create a REST API implementing user authentication using javascript and the NodeJS framework with express and you must implement the necessary changes to store the data in the database and use MongoDB.

The use of the previous code of the task api is recommended to start the development, since it meets all the necessary endpoints and you should only add two additional endpoints and create a middleware that must validate that the user is valid within our REST API.

## 🗒️ Instructions

Implement an authentication system in the following parts:

1. **Registration**: The user must be able to enter an email, any password and submit the form, a new user must be created in the database and the user must be redirected to the login page after this.
2. **Login**: The user must fill in their email and password and must be redirected to a private menu after successful authentication.
3. **Validation**: Any page considered "private" must always be validating that the current user is valid through middleware, if not, it should return an error message that this endpoint is private.

At least the following pages and React components must be implemented in the project:


| Ruta          | Metodo      | Funcionalidad                                                            | 
| ------------- | ----------- | -----------------------------------------------------------------------  |
| `/signup`.    | `POST`      | Route that allows me to register in the REST                             |
| `/signin`.    | `POST`      | Route that allows me to login to the REST API                   |
| `/todos`      | `GET`       | Task list (public)                    |
| `/todos`      | `POST`      | Route that allows me to create a task in the REST API (private)         |
| `/todos/:id`  | `PUT`       | Route that allows me to update a task in the REST API (private)     |
| `/todos/:id`  | `DELETE`    | Route that allows me to delete a task in the REST API (private) |

## More details about authentication:

Usually an authentication system is implemented in 4 parts:

![Authentication Diagram](https://github.com/breatheco-de/jwt-authentication-with-flask-react/blob/main/.learn/login_diagram.jpeg?raw=true)
