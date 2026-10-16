# Getting Started

## Run locally

From the repository root, install dependencies once and start the frontend:

```sh
npm install
npm start
```

Open <http://localhost:8080>. The root start script serves the `frontend` directory, where the app entry point and static assets live.

## Backend API

The backend is a separate JSON API. From the `backend` directory, install dependencies and start it:

```sh
npm install
npm start
```

It listens on <http://localhost:3000>. The API supports `GET`, `POST`, `PATCH`, and `DELETE` at `/api/issues`; `GET /health` checks server availability. Issues are persisted in `backend/data/issues.json`.

The frontend is connected to this API and fetches issue data from the backend. Any issue created, updated, or deleted in the browser updates the shared JSON store on the server.