# Create Post-Book API 

In this project we will create our own API of posts. 

## What you will be doing

This project will allow you to practise using:

> CORS 
> Configuring application to allow cross origin requests. 


This project assumes you've already had experience with:

> - ExpressJS Routing
> - Http methods


## Task 1 - Getting ready

1. Initialise npm into your project
   `npm init -y`
2. Install the express.js npm package
   `npm i express`
3. Create a file for your server (`server.js`)


## Task 2 - Set up your server

##### starter code
```javascript
import express from 'express'
const app = express();

app.use(express.json());

app.listen(4000, () => {
   console.log("The server is listening to requests") 
});
```

## Task 3 - Setting up routes and controllers

  1. Create a folder `/routes`
  2. Create a folder `/controllers`
  3. Create a `postsRoutes.js` file 
  4. Create a `postsController.js`  file
  5. Import the router application into your `server.js` file.
  6. Assign the router applications to their respective route. `/post`


## Task 4 - Create routes with their respective controller methods in postsRoutes.js
  1. Create a GET route `/post/posts/` which exposes all the posts from dataposts.js

  2. Create a POST route `/post/newpost/` which allows you to add a new post using the body: 
     ```json
      {
          "title":"My title",
          "content":"The content of the newly created post"
      }
     ```


  3. Make sure the POST route automatically assigns the highest id to the new post :
   ```javascript
      maxId = Math.max.apply(Math, data.map(function(o) { return o.id; }));
   ```
   

## Task 5 - Configure Cors
 1. Install the cors module
    `npm i cors`
 2. Import the cors module in `server.js` using require
 3. Configure the server to accept all origins using app.use : 
   ```javascript
      app.use(cors());
   ````


## Task 6 - Test everything
 1. Test your backend using postman or insomnia. 


## Bonus - exercise (optional)
- Link to bonus exercise
  [Bonus](./BONUS.md) 










