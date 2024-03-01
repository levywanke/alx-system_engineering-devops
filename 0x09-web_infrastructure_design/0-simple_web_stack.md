
1. Server: Physical or virtual machine hosting the web infrastructure.
2. Domain Name: Human-readable address translating to server's IP.
3. DNS Record: "www" is typically a CNAME record pointing to the main domain's A record.
4. Web Server (Nginx): Handles HTTP requests, serves static content, and passes dynamic requests to the application server.
5. Application Server: Hosts and executes application codebase, handles dynamic content generation.
6. Database (MySQL): Stores and manages website data.
7. Communication Protocol: Server communicates with user's computer using HTTP protocol.
8. Issues:
   - SPOF: Vulnerable to complete failure if server goes down.
   - Downtime During Maintenance: Web server restarts cause downtime.
   - Limited Scalability: Difficult to handle high traffic volumes due to single server setup
