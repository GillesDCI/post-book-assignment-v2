# Bonus Post-Book API 

This is the bonus exercise for when you're ready with the frontend and backend. 

## Bonus Task - Create route handlers in postsRoutes.js

  1. Create a GET route `/post/posts/:id` which gets the post by id

  2. Create a DELETE route `/post/posts/delete/:id` which deletes the post by ID


  3. Create a PUT route `/post/posts/update/:id` which allows you to update an existing post using the body of the HTTP request: 
     ```json
      {
          "title":"My title",
          "content":"The content of my updated post"
      }
     ```


