Project 1 – EC2 Web Application with ALB & Auto Scaling
Step-by-Step Implementation Plan
1. Launch a Web Application
•	Create a simple HTML/PHP site (can even be a static HTML page)
•	Package it in an AMI for EC2 instances
2. EC2 Auto Scaling Group
•	Launch EC2 instances in 2 Availability Zones for high availability
•	Use a Launch Template/Configuration with the AMI
3. Application Load Balancer (ALB)
•	Create ALB → forward traffic to EC2 instances in the ASG
•	Configure health checks → ensure failed instances are replaced
4. IAM Roles & Security Groups
•	EC2 role → minimal permissions (read from S3 if needed)
•	Security groups → allow HTTP/HTTPS from ALB only
5. Monitoring & Alerts
•	CloudWatch → monitor CPU/Memory, scale-out/scale-in policies
•	SNS → alert notifications


<img width="975" height="692" alt="image" src="https://github.com/user-attachments/assets/98c308e6-1b70-4f58-bca7-b96b81593168" />
