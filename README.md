# Learning

This repository is for taking notes while learning technologies.

## Technology

- Express
- Node

## Node

```sh
$ npm init      # start new node project
$ npm i express dotenv # install packages
$ npm i -D nodemon # install packages for only in development mode
$ npm i morgan # logger middleware
```

### package.json

```json
"scripts": {
    "start": "NODE_ENV=production node server", // Set environment as production
    "dev": "nodemon server"
}
```

### Middleware

- It needs 3 parameters (req, res, next)
- It can be used the code after `app.use(SOME_MIDDLEWARE)`;

## License

Distributed under the MIT License. See [LICENSE.md](LICENSE.md) for more information.
