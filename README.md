# GraphQL Demo with Node.js and React (Apollo)

This repository contains a basic demonstration of GraphQL using Node.js for the backend and React with Apollo Client for the frontend.

## Features

- **Backend**: Node.js GraphQL server with Express
- **Frontend**: React application with Apollo Client
- **GraphQL**: Sample queries and mutations
- **Type System**: GraphQL schema definition

## Prerequisites

Before you begin, ensure you have met the following requirements:
- Node.js (v14 or later)
- npm or yarn
- Basic knowledge of GraphQL, React, and Node.js

## Installation

1. Clone the repository:
   ```bash
   git clone https://github.com/SinghTanmay024/GrapgQl.git
   cd your-repo-name
   ```

2. Install backend dependencies:
   ```bash
   cd server
   npm install
   ```

3. Install frontend dependencies:
   ```bash
   cd ../client
   npm install
   ```

## Running the Application

1. Start the GraphQL server:
   ```bash
   cd server
   npm start
   ```
   The server will run on `http://localhost:4000/graphql`

2. In a separate terminal, start the React app:
   ```bash
   cd client
   npm start
   ```
   The client will run on `http://localhost:3000`

## Project Structure

```
/
├── server/                 # Backend GraphQL server
│   ├── schema.js           # GraphQL type definitions and resolvers
│   ├── server.js           # Express server setup
│   └── package.json        # Backend dependencies
│
├── client/                # Frontend React application
│   ├── src/
│   │   ├── components/     # React components
│   │   ├── App.js          # Main application component
│   │   ├── index.js        # Application entry point
│   │   └── client.js       # Apollo Client configuration
│   └── package.json       # Frontend dependencies
│
└── README.md              # This file
```

## Sample Queries

Here are some example GraphQL queries you can try:

### Query all items
```graphql
query {
  items {
    id
    name
    description
  }
}
```

### Add a new item
```graphql
mutation {
  addItem(name: "New Item", description: "Item description") {
    id
    name
    description
  }
}
```

## Technologies Used

- **Backend**:
  - Node.js
  - Express
  - Apollo Server
  - GraphQL

- **Frontend**:
  - React
  - Apollo Client
  - GraphQL

## Contributing

Contributions are welcome! Please follow these steps:
1. Fork the repository
2. Create a new branch (`git checkout -b feature-branch`)
3. Commit your changes (`git commit -am 'Add new feature'`)
4. Push to the branch (`git push origin feature-branch`)
5. Create a new Pull Request

## License

This project is open source and available under the [MIT License](LICENSE).

## Contact

For questions or feedback, please contact [Your Name] at [your-email@example.com]
