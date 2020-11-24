# Learning

This repository is for taking notes while learning technologies.

## Node

```sh
$ npm init # start new node project
$ npm i express dotenv morgan mongoose colors slugify express-fileupload jsonwebtoken bcryptjs cookie-parser # install packages
$ npm i -D nodemon # install packages only in development mode
$ npm run dev # run server with development mode
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
- [asyncHandler](https://www.acuriousanimal.com/blog/2018/03/15/express-async-middleware)
- [Mongoose documents about middleware](https://mongoosejs.com/docs/middleware.html)

// Mongoose

- Sometimes you want to show the fields in the class that not belongs to -> use [virtuals](https://mongoosejs.com/docs/tutorials/virtuals.html)

## License

Distributed under the MIT License. See [LICENSE.md](LICENSE.md) for more information.
