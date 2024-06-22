Web Stack Outage on ALX THE ROOM FELLOWSHIP KENYA
Issue Summary
Duration of the Outage:
Start Time: 2024-06-15 14:00 EAT
End Time: 2024-06-15 16:30 EAT

Impact:
Imagine trying to get through a crowded market on a hot day – that's what our website felt like. Pages were loading slower than a snail on vacation. Approximately 85% of our users were affected, leading to frustration and numerous complaints.

Root Cause:
Our database decided to take a nap instead of working efficiently. Misconfigurations led to inefficient queries that overloaded the server, causing delays.

Timeline

14:00 - 🚨 Issue detected: Monitoring alert for high latency.
14:05 - 👀 Confirmed: Manual check by on-call engineer.
14:10 - 🕵️‍♂️ Investigated: Assumed a DDoS attack or high traffic.
14:25 - 🔍 Misleading Path: Checked network traffic and firewall – no issues.
14:45 - 🚀 Escalated: Passed to the database team.
15:00 - 📜 Logs Reviewed: Found slow queries and table locks.
15:15 - 🛠 Analyzed: Suboptimal query caching and indexing discovered.
15:30 - 🔧 Optimized: Adjusted cache size and added indexes.
16:00 - 📈 Improvements: Page load times reduced.
16:30 - 🎉 Resolved: Normal performance restored, alerts cleared.
Root Cause and Resolution
Root Cause:
Our database was like a poorly organized library – finding anything took forever. The query cache was too small, and our indexing was non-existent, making data retrieval painfully slow.

Resolution:

Query Cache Adjustment: Increased the cache size from 64MB to 256MB – like giving the librarian a coffee.
Indexing: Added indexes to frequently accessed tables – organized the library.
Query Optimization: Reviewed and optimized common queries – streamlined the search process.
These changes turned our database from a sleepy librarian into a speed-reading champion.

Corrective and Preventative Measures
Improvements and Fixes:

Enhanced Monitoring: Implement more granular monitoring for database performance metrics, including query execution times and cache hit rates.
Regular Audits: Schedule regular database configuration and performance audits to ensure optimal settings are maintained.
Query Optimization: Conduct periodic reviews and optimization of frequently executed queries.
Tasks to Address the Issue:

Patch Database Server: Apply the latest patches and updates to the database server software.
Add Monitoring: Implement monitoring tools specifically for database performance, such as slow query logs and table lock alerts.
Optimize Queries: Continuously review and optimize new and existing queries, especially those that show high execution times.
Training: Conduct training sessions for the engineering team on best practices for database configuration and query optimization.
By addressing these areas, we can significantly reduce the likelihood of similar outages occurring in the future and ensure a more resilient and performant web stack for our users.