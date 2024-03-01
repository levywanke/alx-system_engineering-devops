servers: Adding multiple servers improves reliability and scalability by distributing the workload and providing redundancy.

2. Firewalls: Firewalls are added to control and monitor incoming and outgoing network traffic to and from the servers. They help protect against unauthorized access, malicious attacks, and data breaches.

3. SSL Certificate: An SSL certificate is added to enable HTTPS, encrypting traffic between the server and clients. This ensures data privacy and security, preventing unauthorized access or tampering.

4. Monitoring Clients: Monitoring clients are installed on each server to collect performance metrics, logs, and other data for monitoring and analysis. This helps identify and troubleshoot issues, optimize performance, and ensure uptime.

5. Why Firewalls Firewalls are added to restrict access to the servers, filtering incoming and outgoing traffic based on predefined security rules. This helps prevent unauthorized access, data breaches, and malicious attacks.

6. HTTPS Traffic Serving traffic over HTTPS encrypts data transmitted between the server and clients, ensuring confidentiality, integrity, and authenticity. This protects sensitive information such as login credentials, payment details, and personal data from interception or tampering.

7. Monitoring Purpose Monitoring is used to track the performance, availability, and security of the web infrastructure. It provides insights into server health, resource usage, application performance, and security incidents, helping detect and resolve issues proactively.

8. Data Collection The monitoring tool collects data by deploying monitoring agents or clients on each server. These agents gather metrics, logs, and events from the server's operating system, applications, and network, sending them to a centralized monitoring platform for analysis and visualization.

9. Monitoring QPS: To monitor web server QPS (Queries Per Second), you can configure the monitoring tool to track the number of HTTP requests handled by the web server over a specific time period. This helps assess server load, performance bottlenecks, and scalability requirements.

Issues with this Infrastructure:

Terminating SSL at Load Balancer Level: Terminating SSL at the load balancer exposes decrypted traffic within the internal network, potentially compromising data confidentiality and security.

 Single MySQL Server Accepting Writes: Having only one MySQL server capable of accepting writes introduces a single point of failure. If the server fails, write operations will be unavailable until failover occurs.

Identical Components Across Servers: Having servers with identical components (database, web server, application server) may lead to uniform vulnerabilities and dependencies. If a critical vulnerability is exploited, it can impact all servers simultaneously, increasing the risk of widespread outages or breaches.
