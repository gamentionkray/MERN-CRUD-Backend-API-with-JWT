# MERN CRUD Backend API with JWT

---

> To start using,
>
> 1. yarn install
> 2. yarn dev

```diff
! Note:- You need to have MongoDB installed and running locally on your machine.
```

> To learn how to install MongoDB on windows 10, click [here](https://www.youtube.com/watch?v=FwMwO8pXfq0)

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
+ Babel is used here to use import/export and async/await commands which is not supported ususally.
```

---

#### A special thanks to Packt Publishing's book [Full-Stack React Projects - Second Edition](https://www.packtpub.com/product/full-stack-react-projects-second-edition/9781839215414)
