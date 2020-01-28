# Exercise tracker

I created this microservice in fulfillment of [freeCodeCamp](https://freecodecamp.org)'s APIs and Microservices Project [Exercise tracker](https://www.freecodecamp.org/learn/apis-and-microservices/apis-and-microservices-projects/exercise-tracker), using [Node.js](https://nodejs.org/en/) and [Express](https://expressjs.com/), [Mongoose](https://mongoosejs.com/), [shortId](https://github.com/dylang/shortid), and a free [MongoDB Atlas](https://www.mongodb.com/cloud/atlas) database. The front end API on the home page also uses [Bootstrap](https://getbootstrap.com/), [jQuery](https://jquery.com/), [jQuery UI](https://github.com/dylang/shortid), and [highlight.js](https://highlightjs.org/). The API fulfills the following user stories:

1. I can create a user by posting form data username to `/api/exercise/new-user` and returned will be an object with `username` and `_id`.
2. I can get an array of all users by getting `api/exercise/users` with the same info as when creating a user.
3. I can add an exercise to any user by posting form data `userId` (`_id`), `description`, `duration`, and optionally `date` to `/api/exercise/add`. If no date supplied it will use current date. Returned will the the user object with also with the exercise fields added.
4. I can retrieve a full exercise log of any user by getting `/api/exercise/log` with a parameter of `userId` (`_id`). Return will be the user object with added array log and count (total exercise count).
5. I can retrieve part of the log of any user by also passing along optional parameters of `from` & `to` or `limit`. (Date format `yyyy-mm-dd`, `limit` = int)
