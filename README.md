## 📌 Most Challenging Problem I Solved


- The most challenging problem I solved in this project was handling duplicate orders and race-condition issues during peak traffic on my food-ordering website.  
- When many users submitted orders simultaneously, the system sometimes created multiple order entries or reduced inventory incorrectly.  
- To fix this, I implemented a queue system so that all order-creation tasks were processed in a strict sequential flow.  
- I also used database transaction locks to ensure that inventory updates and order confirmations happened safely and atomically.  
- Additionally, I added idempotency keys to prevent repeated or retried requests from generating duplicate orders.  
- After implementing these improvements, the entire checkout workflow became stable, accurate, and resistant to concurrency problems.  
- These changes significantly improved the overall reliability of order processing and user experience.
