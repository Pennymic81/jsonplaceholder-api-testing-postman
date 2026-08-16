# JSONPlaceholder API Testing Portfolio

This project demonstrates practical API testing with Postman using the public JSONPlaceholder REST API. It covers positive and negative scenarios across GET, POST, PUT, and DELETE requests.

## Project summary

| Item | Details |
| --- | --- |
| API | JSONPlaceholder |
| Tool | Postman |
| Test type | Functional API testing |
| Requests | 6 |
| Methods | GET, POST, PUT, DELETE |
| Recorded runner result | 17 passed, 0 failed, 0 errors |
| Recorded average response time | 298 ms |

## Coverage

- Retrieve all users.
- Retrieve one user by ID.
- Verify a nonexistent user returns `404 Not Found`.
- Create a new post.
- Update an existing post.
- Delete an existing post.
- Validate status codes, response structures, field values, and response time.

## Repository contents

- `JSONPlaceholder_API_Testing_Portfolio.postman_collection.json` — clean importable Postman collection.
- `docs/test-plan.md` — scope, approach, entry criteria, and exit criteria.
- `docs/test-cases.md` — test cases and expected results.
- `docs/test-summary-report.md` — execution outcome and observations.
- `evidence/postman-collection-runner.png` — screenshot of the successful collection run.

## How to run

1. Open Postman.
2. Select **Import**.
3. Choose `JSONPlaceholder_API_Testing_Portfolio.postman_collection.json`.
4. Open the imported collection.
5. Select **Run collection**.
6. Keep **Functional** selected and set **Iterations** to `1`.
7. Select all six requests, then click **Start run**.

The exported collection was cleaned to remove blank requests and the unrelated Restful Booker work. Three automated assertions were also added to the Create New Post request, so a new complete run should execute 20 assertions.

## Important note

JSONPlaceholder is a simulated API. POST, PUT, and DELETE responses behave like successful operations, but changes are not permanently stored on the server.
