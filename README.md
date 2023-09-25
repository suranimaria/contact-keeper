# ContactKeeper

ContactKeeper is a comprehensive contact management application that allows users to manage their contacts seamlessly. The app is live and can be accessed at [ContactKeeper](https://contact-keeper-8e8t.onrender.com/).

## Tech Stack

- **Backend**: Node.js, Express, JWT for authentication
- **Frontend**: React (using Context API, Hooks, and Redux), Javascript, HTML, CSS
- **Database**: MongoDB
- **Deployment**: Render platform

## API Endpoints

### Contacts

- **GET** `/api/contacts`: Fetch all user contacts. Requires authentication.
- **POST** `/api/contacts`: Add a new contact for the authenticated user. Requires name in the request body.
- **PUT** `/api/contacts/:id`: Update a specific contact. Requires authentication and contact ownership.
- **DELETE** `/api/contacts/:id`: Delete a specific contact. Requires authentication and contact ownership.

### Users

- **POST** `/api/users`: Register a new user. Requires name, email, and password in the request body.

### Auth

- **GET** `/api/auth`: Fetch the authenticated user. Requires authentication token.
- **POST** `/api/auth`: Authenticate a user and get an access token. Requires email and password in the request body.

## Getting Started

### Installation

1. Clone the repository and change directory to project folder::
```bash
git clone [repository-link]
cd contact-keeper
```

2. Install server dependencies:
```
npm install

```

3. Change directory to client folder and install client dependencies:

```
cd client && npm install

```

### Running Locally

* Start the backend server:
```
npm run server

```

* In separate terminal, tart the frontend server:
```
npm run client

```

* To run both frontend and backend concurrently:
```
npm run dev

```