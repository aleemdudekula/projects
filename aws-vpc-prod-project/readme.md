# AWS-VPC-PROD-PROJECT

<img width="611" height="481" alt="image" src="https://github.com/user-attachments/assets/8b3c30a6-00b4-4021-b2fa-ba1c549aa772" />

# Built a Production-Ready AWS VPC Architecture from Scratch

I designed and deployed a highly available infrastructure using Amazon Web Services:

🔹 Multi-AZ VPC with public & private subnets

🔹 Application Load Balancer for traffic distribution

🔹 Auto Scaling Group for high availability

🔹 Bastion Host for secure access

🔹 NAT Gateway for private subnet internet access

# 💡 Key Learning:

I faced a real-world issue where my application worked intermittently and returned 502 errors.

After debugging, I found:

One instance in the target group was unhealthy

Traffic was being routed inconsistently

Backend service configuration was not identical across instances

# 🔧 Fix:

Ensured consistent app setup across all instances

Corrected security group rules

Verified health checks and target group configuration

# 📌 Outcome:

Stable, highly available web application accessible via Load Balancer

This project helped me understand not just AWS services — but how real production systems behave under load and failure. 










