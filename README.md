<h2 align="center">GraphQl-Boot</h2>

<p align="center">
    <img src="https://www.vectorlogo.zone/logos/graphql/graphql-icon.svg" width="150px" height="auto">
</p>

> ☄️ Simple GraphQL API using graphpack

### ⚙️ Run the server

To start, use the commands:

```bash
    cd graphql-server
    npm install
    npm run dev
```

It should launch a server at http://localhost:4000, where a GraphQL playground will be available.

### 🔗 API methods

**Query**

- users: returns data of all users.
- user(id: ID!): returns an user by ID.

**Mutation**

- createUser(id: ID!, name: String!, email: String!, age: Int): creates user and returns data about it.
- updateUser(id: ID!, name: String, email: String, age: Int): finds an user by ID and updates it.
- deleteUser(id: ID!): finds an user by ID and deletes it.