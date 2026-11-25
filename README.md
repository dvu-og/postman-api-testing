# Postman API Testing

API testing project using Postman and Newman on the jsonplaceholder and postman-echo practice APIs.

## What's covered

- GET, POST, PUT, PATCH, DELETE requests
- Automated tests (status code, response body, headers)
- Environment variables and request chaining
- Authorization: Basic Auth, Bearer Token, API Key
- Negative testing
- Data-driven testing with a CSV file
- Running the collection with Newman
- query params, assertions and the Postman Runner result

## How to run

1. Install Node.js, then Newman:

```
npm install -g newman
```

2. Run the collection:

```
newman run "API test library.postman_collection.json" -e dev.json -d posts.csv --env-var "base_url=https://jsonplaceholder.typicode.com" --env-var "post_id=101"
```

## Result

3 iterations, 39 assertions, 0 failed
