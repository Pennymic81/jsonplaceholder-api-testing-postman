# API Test Plan

## Objective

Verify that the selected JSONPlaceholder endpoints respond correctly for common read, create, update, delete, and negative-test scenarios.

## In scope

- `GET /users`
- `GET /users/1`
- `GET /users/999`
- `POST /posts`
- `PUT /posts/1`
- `DELETE /posts/1`
- Status-code validation
- Response-body and field validation
- Basic response-time validation

## Out of scope

- Authentication and authorization
- Database verification
- Performance, load, and security testing
- Persistent-data validation
- Testing every JSONPlaceholder resource

## Test approach

Requests are executed individually during development and together through Postman Collection Runner. Automated assertions validate expected response codes, structures, values, and selected response times.

## Entry criteria

- Internet access is available.
- Postman is installed or accessible in a browser.
- The JSONPlaceholder API is available.
- The collection imports successfully.

## Exit criteria

- All six requests execute.
- Expected status codes are returned.
- All automated assertions pass.
- Any unexpected result is documented with evidence.

## Risks and limitations

JSONPlaceholder simulates write operations. A successful POST, PUT, or DELETE response does not mean data was permanently changed. Response times can also vary with network conditions.
