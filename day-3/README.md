# 📘 What Will You Learn?

# 🚀 Introduction to EC2
# Amazon EC2 (Elastic Compute Cloud) is a cloud service that provides secure, resizable virtual servers (instances) to run your applications.

# ✅ Key Benefits:
# - 🧩 Resizable and scalable compute power
# - 🔒 Built-in security with AWS Nitro System
# - 💰 Cost-effective pricing with Spot instances & Savings Plans
# - ⚡ High performance and 99.99% uptime SLA

# 💡 EC2 Use Cases
# - 🛡️ Run secure and high-performance applications
# - 📊 Perform big data or scientific processing
# - 💻 Host websites or backend apps
# - 🤖 ML/AI workloads using GPU instances
# - ⚙️ Build dev/test environments on demand

# 🧠 EC2 Instance Types

# 1️⃣ General Purpose
# ⚖️ Balanced compute, memory, and networking — good for web servers and testing

# 2️⃣ Compute Optimized
# 💪 CPU-intensive workloads like gaming, scientific jobs

# 3️⃣ Memory Optimized
# 🧠 For memory-heavy tasks like in-memory DBs or analytics

# 4️⃣ Storage Optimized
# 💾 High disk throughput, ideal for big data and logs

# 5️⃣ Accelerated Computing
# 🚀 Use GPU/FPGAs for ML, AI, and rendering workloads

# 🔗 Docs: https://docs.aws.amazon.com/AWSEC2/latest/UserGuide/instance-types.html

# 🧬 EC2 Instance Family Codes

# C  – Compute optimized
# M  – General purpose
# R  – Memory optimized
# G, P – GPU-based
# I  – IO / Storage optimized
# T  – Burst performance (e.g. t2.micro)
# F  – FPGA
# U, X – Ultra / Extra memory

# Example: t2.micro → T family (Turbo)

# 🧩 EC2 Instance Basics

# 🔑 Key Concepts:
# - Instance = Your virtual server
# - AMI = Pre-built OS image
# - Instance Type = Power/Size of VM
# - Instance State = Running / Stopped / Terminated

# 💸 EC2 Pricing Options:
# - On-Demand → Pay per use
# - Reserved → Long-term savings
# - Spot → Cheapest, but can be interrupted

# 🚀 How to Launch an EC2 Instance (AWS Console)

# 1. Go to EC2 Dashboard → Launch Instance
# 2. Choose an AMI (like Ubuntu)
# 3. Select instance type (e.g., t2.micro)
# 4. Configure networking (VPC, subnet)
# 5. Add security group (allow SSH port 22)
# 6. Create/download key pair
# 7. Launch the instance!

# 🔧 Managing EC2 Instances

# - ▶️ Start, ⏹️ Stop, or ❌ Terminate anytime
# - 📈 Monitor usage via CloudWatch
# - 🐧 Access instance using SSH:

# Example SSH command:
# ssh -i "your-key.pem" ubuntu@<your-ec2-public-ip>
