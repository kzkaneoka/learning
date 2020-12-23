# Learning

This repository is for taking notes while learning technologies.

## MERN File Structure

- [How to organise file structure of backend and frontend in MERN](https://www.semicolonworld.com/question/72662/how-to-organise-file-structure-of-backend-and-frontend-in-mern)

```sh
$ npm init # start new node project
$ npm i -D concurrently # install packages only in development mode
```

```json
"scripts": {
    "dev": "concurrently \"cd server && npm run dev\" \"cd client && npm start\" "
}
```

## MEARN Server Side

```sh
(./server)$ npm init # start new node project
(./server)$ npm i express dotenv morgan mongoose colors slugify express-fileupload jsonwebtoken bcryptjs cookie-parser # install packages
(./server)$ npm i -D nodemon concurrently # install packages only in development mode
(./server)$ npm run dev # run server with development mode
```

```json
"scripts": {
    "start": "NODE_ENV=production node server", // Set environment as production
    "dev": "nodemon server"
}
```

- Middleware
  - It needs 3 parameters (req, res, next)
  - It can be used the code after `app.use(SOME_MIDDLEWARE)`;
  - [asyncHandler](https://www.acuriousanimal.com/blog/2018/03/15/express-async-middleware)
  - [Mongoose documents about middleware](https://mongoosejs.com/docs/middleware.html)
- Mongoose
  - Sometimes you want to show the fields in the class that not belongs to -> use [virtuals](https://mongoosejs.com/docs/tutorials/virtuals.html)

## MEARN Client Side

```sh
(./client)$ npx create-react-app . # start new react project locally not globally
(./client)$ npm i axios react-router-dom # install packages
```

## License

Distributed under the MIT License. See [LICENSE.md](LICENSE.md) for more information.
