# MERN CRUD Backend API with JWT

---

> To start using,
> yarn install then,
> yarn dev

#### Configure your port, MongoDB URI and JWT secret key in config folder

---

**API endpoints for user CRUD**

| Operation      | API route          | HTTP method |
| -------------- | ------------------ | ----------- |
| Create a user  | /api/users         | POST        |
| List all users | /api/users         | GET         |
| Fetch a user   | /api/users/:userId | GET         |
| Update a user  | /api/users/:userId | PUT         |
| Delete a user  | /api/users/:userId | DELETE      |
| User sign-in   | /auth/signin       | POST        |
| User signout   | /auth/signout      | GET         |

---

**Folder and file structure**

```bash

server
 ┣ config
 ┃ ┗ config.js
 ┣ controllers
 ┃ ┣ auth.controller.js
 ┃ ┗ user.controller.js
 ┣ helpers
 ┃ ┗ dbErrorHandler.js
 ┣ models
 ┃ ┗ user.model.js
 ┣ routes
 ┃ ┣ auth.routes.js
 ┃ ┗ user.routes.js
 ┣ .babelrc
 ┣ .gitignore
 ┣ express.js
 ┣ package.json
 ┣ readme.MD
 ┣ server.js
 ┗ yarn.lock

```

---

**The JSON Web Token must be included in the request Authorization header as a Bearer for fetching single user: _Authorization: Bearer <JSON_Web_Token>_**

---

```diff
+ Compiles ES6+ code using Babel.
```

---

##### A special thanks to Packt Publishing's book [Full-Stack React Projects - Second Edition(https://www.packtpub.com/product/full-stack-react-projects-second-edition/9781839215414)
