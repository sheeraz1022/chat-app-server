# Chat App Server

This is basically a GraphQL server which is serving Chat application to run on client side. It is a nodejs application

## Structure of GraphQL Server application

This is graphql server is using graphql-yoga library to serve. It has schema as follow

```
query {
  messages {
    id
    user
    content
  }
}
```

This query is used to fetch the messages sent over the chat. 

```
mutation {
  postMessage(user: "Sheeraz", content: "Hello, this is test message")
}
```

This mutation is used to sent a message to server

## Hosting

This application is hosted under heroku. You can access this live application on this url https://sheeraz-chat-server.herokuapp.com/

## Client Application

Hosted client application: https://thirsty-almeida-074cb5.netlify.app/
Git Repo of client application: https://github.com/sheeraz1022/chat-app
