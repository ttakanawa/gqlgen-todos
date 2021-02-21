# gqlgen-todos

The CRUD API of todo app. This is for practicing.

## Examples GraphQL

Example for GetAll

http://localhost:8080/query
```graphql
# Write your query or mutation here
{
  todos {
    id
    text
    done
    doneAt
    createdAt
  }
}
```

Examples for Create and update

http://localhost:8080/query
```graphql
mutation Create {
  createTodo(input: {text: "Test A"}) {
    id
    text
    done
    doneAt
    createdAt
  }
}

mutation Update {
  updateTodo(input: {
    id: "some id that data you created before"
    text: "Test A!"
    done: true
  }) {
    id
    text
    done
    doneAt
    createdAt
  }
}
```
