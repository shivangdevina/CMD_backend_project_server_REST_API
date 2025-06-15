# CMD_backend_project_server_REST_API
# Subscriber API

The Subscriber API is a RESTful API that allows you to manage subscribers to a channel. It provides endpoints for creating, reading, updating, and deleting subscriber information.

## Installation

1. Clone the repository:
```
git clone https://github.com/your-username/subscriber-api.git
```

2. Install the dependencies:
```
cd subscriber-api
npm install
```

3. Create a `.env` file in the root directory and add the following environment variable:
```
DATABASE_URL=<your-mongodb-connection-string>
```

4. Start the server:
```
npm start
```

The server will start running on `http://localhost:3000`.

## Usage

### API Endpoints

#### Get All Subscribers
```
GET /subscribers
```

#### Get a Subscriber
```
GET /subscribers/:id
```

#### Create a Subscriber
```
POST /subscribers
```
Request body:
```json
{
  "name": "John Doe",
  "subscribedToChannel": "Example Channel"
}
```

#### Update a Subscriber
```
PATCH /subscribers/:id
```
Request body:
```json
{
  "name": "Jane Doe",
  "subscribedToChannel": "New Channel"
}
```

#### Delete a Subscriber
```
DELETE /subscribers/:id
```

## API

The Subscriber API provides the following endpoints:

| Endpoint | HTTP Method | Description |
| --- | --- | --- |
| `/subscribers` | `GET` | Get all subscribers |
| `/subscribers/:id` | `GET` | Get a specific subscriber |
| `/subscribers` | `POST` | Create a new subscriber |
| `/subscribers/:id` | `PATCH` | Update an existing subscriber |
| `/subscribers/:id` | `DELETE` | Delete a subscriber |

## Contributing

1. Fork the repository
2. Create a new branch: `git checkout -b feature/your-feature`
3. Make your changes and commit them: `git commit -am 'Add some feature'`
4. Push to the branch: `git push origin feature/your-feature`
5. Submit a pull request

## License

This project is licensed under the [MIT License](LICENSE).

## Testing

To run the tests, use the following command:
```
npm test
```
