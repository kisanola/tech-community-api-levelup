## Tech Community Backend Levelup

In this challenge, you are part of a team building a blog platform. One requirement is for a REST API service to provide posts information using the Nodejs Express framework. The requirements include filtering and ordering requirements, response codes and error messages for the queries you must implement.

The definitions and a detailed requirements list follow. You will be graded on whether your application performs data retrieval and manipulation based on given use cases exactly as described in the requirements.

### Required features
- Users should be able to add a new post
- Users should be able to update a single post
- Users should be able to retrieve a sinle post
- Users should be able to delete a single post
- Users should be able to retrive all posts
  
### Schema
- Post
```
  {
    id: String|Required,
    slug: String|Required,
    poster: String|Required,
    title: String|Required,
    description: String|Required,
    createdAt: Date|Required,
    updatedAt: Date|Required,
  }
```
### Responses
#### Generic Responses
- Success reposnse
  ```js
    {
      status: Integer,
      message: String,
      data: Object|Array
    }
  ```

- Error response
  ```js
  {
    status: Integer,
    error: Object|Array
  }
  ```

#### Success Posts response
- POST /posts
  ```js
  {
    status: 201,
    data : {
      id: String|Required,
      slug: String|Required,
      poster: String|Required,
      title: String|Required,
      description: String|Required,
      createdAt: Date|Required,
      updatedAt: Date|Required,
    }
  }
  ```
- POST /posts/postId
  ```js
  {
    status: 200,
    data : {
      id: String|Required,
      slug: String|Required,
      poster: String|Required,
      title: String|Required,
      description: String|Required,
      createdAt: Date|Required,
      updatedAt: Date|Required,
    }
  }
  ```
- GET /posts
  ```js
  {
    status: 200,
    data : [
      {
        id: String|Required,
        slug: String|Required,
        poster: String|Required,
        title: String|Required,
        description: String|Required,
        createdAt: Date|Required,
        updatedAt: Date|Required,
      }
    ]
  }
  ```

### Technologies
  - Node/Express
  - Mongodb


### Recommended packages
  - [Celebrate](https://www.npmjs.com/package/celebrate): celebrate is an express middleware function that wraps the joi validation library
  - [Mongoose](https://www.npmjs.com/package/mongoose): Mongoose is a MongoDB object modeling tool designed to work in an asynchronous environment.
  - [Babel-watch](https://www.npmjs.com/package/babel-watch): Reload your babel-node app on JS source file changes. And do it fast.
