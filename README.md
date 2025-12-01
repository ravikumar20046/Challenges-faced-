## 📌 Most Challenging Problem I Solved

The most challenging problem I solved in this project was handling duplicate orders and race-condition issues during peak traffic on my food-ordering website.

When many users submitted orders at the same time, the system occasionally created multiple entries or reduced inventory incorrectly.

To address this, I implemented a queue system so that all order-creation tasks were processed in a strict sequential flow.

I also used database transaction locks to ensure that inventory updates and order confirmations happened safely and atomically.

Additionally, I added idempotency keys to prevent repeated or retried requests from generating duplicate orders.

After these improvements, the entire checkout workflow became stable, accurate, and resistant to concurrency problems.

These changes significantly improved the reliability of order processing and overall user experience.
