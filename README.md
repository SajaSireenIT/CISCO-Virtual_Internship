# CISCO-Virtual_Internship


Diagram Explanation:
1.	Route 53: Manages DNS queries and routes traffic to the Application Load Balancer.
2.	AWS WAF (Web Application Firewall): Filters and monitors HTTP/HTTPS requests to protect against common web exploits and DDoS attacks targeting the application layer.
3.	Application Load Balancer: Distributes incoming traffic across multiple EC2 instances within an Auto Scaling group across multiple Availability Zones (AZs), ensuring high availability and scalability.
4.	EC2 Instances: Hosts the application logic and services. Auto Scaling adjusts the number of instances based on traffic demand to handle burst traffic during sales events efficiently.
5.	Amazon RDS (Multi-AZ): Provides a highly available and scalable database solution with automatic failover across multiple AZs. Automated backups are stored in Amazon S3, and point-in-time recovery ensures data integrity and rapid recovery.
6.	Amazon S3: Stores database backups, logs, and other essential data, providing secure and durable storage.
7.	AWS Shield: Provides protection against DDoS attacks by detecting and mitigating malicious traffic before it reaches the application.
