# API Test Cases

| ID | Scenario | Method and endpoint | Expected result | Recorded result |
| --- | --- | --- | --- | --- |
| API-TC-001 | Retrieve all users | `GET /users` | `200`; array contains 10 users | Pass |
| API-TC-002 | Retrieve an existing user | `GET /users/1` | `200`; ID is 1; required user fields exist; email contains `@` | Pass |
| API-TC-003 | Retrieve a nonexistent user | `GET /users/999` | `404`; response is an empty object; response time below 2000 ms | Pass |
| API-TC-004 | Create a post | `POST /posts` | `201`; response includes an ID and submitted post values | Pass (request manually verified); automated assertions added after recorded run |
| API-TC-005 | Update a post | `PUT /posts/1` | `200`; ID, title, and body match submitted values | Pass |
| API-TC-006 | Delete a post | `DELETE /posts/1` | `200`; response is an empty object; response time below 2000 ms | Pass |

Base URL: `https://jsonplaceholder.typicode.com`

## Test data

The create request uses user ID `1`, title `Learning API Testing`, and a short portfolio description. The update request uses post ID `1` and fixed values so the assertions remain repeatable.
