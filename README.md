# forgo-prisma

This example demonstrates how to implement a **GraphQL server with an email-password-based authentication workflow authorized with GraphQL Shield**, [graphql-yoga](https://github.com/prisma/graphql-yoga) and [graphqlgen](https://github.com/prisma/graphqlgen).

## Get started

### 1. Install the Prisma CLI

You need to have the Prisma CLI installed on your machine to run this example. If you don't have it yet, execute the following command to install it globally on your machine:

```
npm i -g prisma
```

### 2. Download example & Install dependencies

Install Node dependencies:

```
npm i
```

### 3. Deploy the Prisma API

You will now deploy the Prisma API that's backing this example. This requires you to have [Docker](https://www.docker.com) installed on your machine (if you don't have Docker follow the collapsed instructions below the code block):

Launch Prisma via Docker:

```
docker-compose up -d
```

Navigate into the `prisma` directory and deploy the Prisma API:

```
cd prisma
prisma deploy
```

<details>
 <summary><strong>I don't have Docker installed on my machine</strong></summary>

To deploy your service to a demo server (rather than locally with Docker), follow these steps:

- Run the following command:
  ```
  cd prisma
  prisma deploy --new
  ```
- In the interactive CLI wizard:
  - Select the **Demo server**
  - For all following questions, choose the suggested values by just hitting **Enter**

</details>

### 4. Start the server

```
cd ..
npm run start
```

Navigate to [http://localhost:4000](http://localhost:4000) in your browser to explore the API of your GraphQL server in a [GraphQL Playground](https://github.com/prisma/graphql-playground).

### 5. Modify resolvers

Read the [graphqlgen](https://github.com/prisma/graphqlgen) readme to learn how to scaffold resolvers.
