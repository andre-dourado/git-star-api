<!-- GETTING STARTED -->
## Getting Started

This backend was proposed by the TOPi development team. The idea is to set up an API in which it performs user authentication.
Through this it is possible to return the data of the previously registered user. In development, Node.js was used in conjunction with PostegreSQL.
In addition, it is worth mentioning that the project was developed respecting the SOLID principles.. 

### Requirements

It is necessary to install yarn to run the project.
* MacOS
  ```sh
  brew install yarn
  ```

### Installation

1. Clone the repository
   ```sh
   https://github.com/andrewdourado/git-star-api.git
   ```
2. Install the packages
   ```sh
   yarn
   ```
4. Run the project
   ```JS
   yarn build:server
   ```

## Routes

- **`POST /users`**: Register a new user:

```json
{
	"name": "admin",
	"email": "admin@email.com",
	"password": "123456"
}
```

- **`GET /sessions`**: Performs user authentication by returning the token:

```json
{
	"email": "admin@email.com",
	"password": "123456"
}
```

## Technologies

- [Node.js](https://nodejs.org/en/)
- [Typescript][ts]
- [TypeORM](https://typeorm.io/#/)
- [Jest](https://jestjs.io/)
- [celebrate](https://github.com/arb/celebrate)
- [bcryptjs](https://github.com/dcodeIO/bcrypt.js)
- [jsonwebtoken](https://jwt.io/)
- [express](https://expressjs.com)
- [pg](https://node-postgres.com/)
- [VS Code][vscode] with [EditorConfig][vceditconfig] and [ESLint][vceslint]

---

Made with ♥ by André Dourado :wave: [Get in touch!](https://www.linkedin.com/in/andre-dourado/)

[ts]: https://www.typescriptlang.org
[vscode]: https://code.visualstudio.com/
[yarn]: https://yarnpkg.com/
[vceditconfig]: https://marketplace.visualstudio.com/items?itemName=EditorConfig.EditorConfig
[vceslint]: https://marketplace.visualstudio.com/items?itemName=dbaeumer.vscode-eslint
