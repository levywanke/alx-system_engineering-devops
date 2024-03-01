

* Introduction:
This project sets up a web infrastructure with a focus on understanding the differences between an application server and a web server. It involves deploying components like servers, load balancers, and splitting services such as web server, application server, and database onto separate servers.

* Infrastructure Setup
1. Server: One server is deployed to host the web infrastructure.
2. Load Balancer (HAproxy): HAproxy is configured as a cluster with another instance to distribute incoming traffic among multiple servers, improving scalability and availability.
3. Split Components: Each component (web server, application server, database) is hosted on its own server for better resource management, isolation, and scalability

- Server: Deploying a server is fundamental to host the web infrastructure. It provides the computing resources and environment necessary for running the different components.
- Load Balancer: Adding a load balancer ensures that incoming traffic is evenly distributed among multiple servers, enhancing performance and fault tolerance. Configuring HAproxy as a cluster ensures redundancy and high availability.
- Split Components: Separating components onto dedicated servers improves resource utilization, isolation, and scalability. The web server handles HTTP requests, the application server executes application logic, and the database stores and manages data.

Conclusion:
This setup demonstrates a scalable and resilient web infrastructure with clear separation of concerns between different components. It provides insights into the roles of application servers and web servers in a web environment.

Further Improvements:
- Implementing monitoring and logging solutions to track performance, troubleshoot issues, and ensure system reliability.
- Adding security measures such as firewalls, intrusion detection systems, and regular security audits to protect against threats and vulnerabilities.


This README provides an overview of the infrastructure setup and the rationale behind each component. It serves as a guide for understanding the project and its objectives.
