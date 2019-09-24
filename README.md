## Tech Community Backend Levelup

In this challenge, you are part of a team building a blog platform. One requirement is for a REST API service to provide posts information using the Nodejs Express framework. The requirements include filtering and ordering requirements, response codes and error messages for the queries you must implement.

The definitions and a detailed requirements list follow. You will be graded on whether your application performs data retrieval and manipulation based on given use cases exactly as described in the requirements.

### Schema
#### Post
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
