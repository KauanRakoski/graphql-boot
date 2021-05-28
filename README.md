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

It should launch a server at **_localhost:4000_**, where a GraphQL playground will be available. _User fields, such as id, name and email (excluding age) are non-nullable, which means every query should contain those_. It uses a JavaScript JSON-based database, for test purposes. Changes won't be persistent.

### 🔗 API methods

**Query (retrieve data):**

```graphql
# Returns an array with all users
users: [User!]!

# Finds an user by ID and returns data about the user.
user(id: ID!): User!
```

**Mutation (update data):**

```graphql
# Creates an user and returns data about it.
createUser(id: ID!, name: String!, email: String!, age: Int): User!

# Finds an user by ID and updates it.
updateUser(id: ID!, name: String, email: String, age: Int): User!

# Finds an user by ID and deletes it.
deleteUser(id: ID!): User!
```
