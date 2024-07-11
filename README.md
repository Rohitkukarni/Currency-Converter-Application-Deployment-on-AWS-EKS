# Currency-Converter-Application-Deployment-on-AWS-EKS


 Objective: To create a scalable and robust Currency Converter application for real-time currency exchange rates.

 🛠️ Technologies Used:
Containerization: Docker 🐳
Orchestration: Kubernetes ☸️
Deployment Strategy: Deployed with 6 replicas for high availability
Cloud Service: AWS EKS
Networking: Kubernetes Services, Ingress, and NGINX Ingress Controller 🛠️
DNS Provider: Hostinger via AWS Route 53

🔐 TLS Certificate Management:
Certificate Authority (CA): Let's Encrypt (open-source CA)
Certificate: tls-cert
Issuer: Let's Encrypt
Validity: Valid until [expiration date]
Subject Alternative Names (SANs): www.krishnakulkarni.online
Secrets Management: Managed Kubernetes Secret (tls-cert) for storing TLS certificate and private key securely.

🔧 Technical Details:
Application Port: 8080
Cluster IP Exposure: Using Kubernetes Ingress
Ingress Controller: NGINX Ingress Controller 🛠️
Custom Subdomain: Application is accessible at www.krishnakulkarni.online, managed via Hostinger DNS (AWS Route 53)
DNS Configuration: Added an A record in Hostinger DNS to point to the Ingress Controller’s IP address
🔍 Steps to Add DNS Record in Hostinger:
Log in to your Hostinger account.
Navigate to the DNS management section.
Add a new A record with the hostname (e.g., www) and the IP address of your Kubernetes ☸️ Ingress Controller.











