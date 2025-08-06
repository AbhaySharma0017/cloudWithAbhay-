# AWS Route 53 - Notes

## 📌 Introduction
Amazon **Route 53** is a **highly available and scalable Domain Name System (DNS) web service** by AWS.  
It is used to:
- Register domain names
- Manage DNS records
- Route end-user requests to applications

---

## 📖 Topics Covered

### 1️⃣ What is Route 53?
- Managed DNS service by AWS.
- Converts **human-readable domain names** (e.g., `example.com`) into **IP addresses** (e.g., `192.0.2.1`).
- Supports health checks, traffic routing, and domain registration.

---

### 2️⃣ How Route 53 Works
1. **User enters a domain name** in browser (e.g., `mywebsite.com`).
2. **DNS Resolver** sends request to Route 53.
3. **Route 53** checks hosted zones for matching DNS records.
4. Returns **IP address** of the resource.
5. Browser connects to the server using that IP.

---

### 3️⃣ Domain Registration in Route 53
- You can register new domains directly via AWS.
- AWS becomes the **registrar**.
- Domains can be managed entirely from the Route 53 console.
- Supports DNSSEC for security.

---

### 4️⃣ Hosted Zones
- **Public Hosted Zone** → For domains accessible from the internet.
- **Private Hosted Zone** → For domains accessible only within a VPC.
- Hosted zone contains **DNS records** for the domain.

---

### 5️⃣ DNS Records in Route 53
| Record Type | Purpose |
|-------------|---------|
| **A**       | Maps domain to IPv4 address |
| **AAAA**    | Maps domain to IPv6 address |
| **CNAME**   | Maps one domain name to another |
| **MX**      | Mail server settings for a domain |
| **NS**      | Nameservers for the hosted zone |
| **PTR**     | Reverse DNS lookup |
| **SOA**     | Authoritative info about the domain |
| **TXT**     | Text info (SPF, DKIM, verification) |
| **SRV**     | Defines services like SIP, XMPP |
| **Alias**   | AWS-specific shortcut to AWS resources (S3, CloudFront, etc.) |

---

### 6️⃣ Routing Policies
- **Simple Routing** → One record, basic routing.
- **Weighted Routing** → Split traffic by percentage.
- **Latency Routing** → Route to region with lowest latency.
- **Failover Routing** → Switch to backup if primary fails.
- **Geolocation Routing** → Based on user’s location.
- **Geoproximity Routing** → Based on location bias.
- **Multivalue Answer Routing** → Returns multiple IPs.

---

## 📝 Summary
AWS Route 53 is a powerful DNS service that:
- Registers and manages domains
- Routes traffic intelligently
- Integrates with AWS services for high availability

---

## 📚 References
- [AWS Route 53 Documentation](https://docs.aws.amazon.com/Route53/latest/DeveloperGuide/Welcome.html)
- [Amazon Route 53 FAQs](https://aws.amazon.com/route53/faqs/)

