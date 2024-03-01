addition of 2 Server: To improve reliability and redundancy by distributing the workload across multiple servers.

2. Load Balancer (HAproxy): To evenly distribute incoming traffic among multiple servers, improving scalability and availability.

3. Distribution Algorithm: The load balancer is configured with a round-robin distribution algorithm, which routes each new request to the next server in line. This ensures a fair distribution of traffic across all available servers.

4. Active-Active vs. Active-Passive Setup:
   - Active-Active: Both servers actively handle incoming requests simultaneously, distributing the load between them. This setup offers high performance and scalability.
   - Active-Passive: One server (active) handles incoming requests while the other server (passive) remains on standby. In case of failure, the passive server takes over to ensure high availability.

5. Database Primary-Replica Cluster (Master-Slave):
   - The primary node (master) handles write operations and updates the replica nodes.
   - The replica nodes (slaves) replicate data from the primary node and handle read operations. They serve as backups in case the primary node fails.

6. Difference between Primary and Replica Node
   - Primary Node: Handles write operations, updates data, and serves as the main point of interaction for the application.
   - Replica Node: Replicates data from the primary node, handles read operations, and serves as a backup. It doesn't accept write operations directly from the application.

Issues with this Infrastructure:

1. Single Points of Failure (SPOF):
   - Load balancer: If the load balancer fails, traffic won't be distributed properly.
   - Database primary node: If the primary node fails, write operations will be unavailable until failover occurs.

2. Security Issues:
   - Lack of Firewall: Exposes servers to potential security threats from unauthorized access or attacks.
   - No HTTPS: Data transmitted between the server and clients is not encrypted, risking interception or tampering.

3. No Monitoring: Without monitoring, it's challenging to identify and address performance issues, security breaches, or system failures proactively.
