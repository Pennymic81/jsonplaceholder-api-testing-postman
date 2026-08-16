# API Test Summary Report

## Execution summary

| Metric | Result |
| --- | --- |
| Collection Runner date | 16 August 2026 |
| Iterations | 1 |
| Automated assertions executed | 17 |
| Passed | 17 |
| Failed | 0 |
| Errors | 0 |
| Recorded average response time | 298 ms |

## Result

The recorded Postman Collection Runner execution completed successfully. All 17 assertions passed with no failures or execution errors. Positive GET scenarios, the negative `404` scenario, update behavior, and delete behavior returned the expected results.

The Create New Post request separately returned `201 Created` during manual execution. Its exported request did not yet contain tests, so three automated assertions were added while cleaning the portfolio collection. A fresh run of the cleaned collection is expected to execute 20 assertions.

## Observations

- The negative test correctly returned `404 Not Found`; this is an expected pass, not a defect.
- JSONPlaceholder simulates POST, PUT, and DELETE operations without permanently changing server data.
- The collection contains no authentication credentials or production data.

## Conclusion

The tested endpoints behaved as expected in the recorded execution. The project demonstrates request creation, negative testing, automated assertions, collection execution, and evidence-based reporting in Postman.
