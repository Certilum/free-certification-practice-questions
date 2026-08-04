<table width="100%">
  <tr>
    <td align="center" valign="middle" width="50%">
      <p align="center"><img src="https://pub-6a9f8dede1194a7786cba69e7dcdad9f.r2.dev/certifications/Amazon%20Web%20Services%20Training%20and%20Certification/AWS%20Certified%20Solutions%20Architect%20–%20Professional" width="50%"></p>
    </td>
    <td align="center" valign="middle" width="50%">
      <h1>AWS Certified Solutions Architect – Professional</h1>
    </td>
  </tr>
</table>

## 📑 Table of Contents

- [Design Cost-Optimized Architectures](#design-cost-optimized-architectures) (8 questions)
- [Design High-Performing Architectures](#design-high-performing-architectures) (7 questions)
- [Design Resilient Architectures](#design-resilient-architectures) (7 questions)
- [Design Secure Architectures](#design-secure-architectures) (8 questions)

## 📋 Exam Information

| Field | Value |
|-------|-------|
| Total Questions | 30 |
| Level | Foundation |
| Exported At | 2026-08-04T06:25:39.760Z |
| Domains | 4 |

## 📊 Domain Distribution

| Domain | Questions |
|--------|-----------|
| Design Cost-Optimized Architectures | 8 |
| Design High-Performing Architectures | 7 |
| Design Resilient Architectures | 7 |
| Design Secure Architectures | 8 |

---

### **Design Cost-Optimized Architectures**

### 1. Which AWS compute pricing model offers the highest discount for a steady-state workload with a fixed instance family and term?

- [ ] **A)** Standard Reserved Instances
- [ ] **B)** Convertible Reserved Instances
- [ ] **C)** Compute Savings Plan
- [ ] **D)** On-Demand Instances

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Standard RIs provide the highest discount (up to 72%) for a specific instance family and term, offering no flexibility but maximum savings.
 
 
</details>

### 2. Which two AWS services are covered by a Compute Savings Plan? (Choose 2)

- [ ] **A)** Amazon EC2
- [ ] **B)** AWS Lambda
- [ ] **C)** Amazon RDS
- [ ] **D)** Amazon DynamoDB

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> A Compute Savings Plan covers EC2, Lambda, and Fargate usage. RDS and DynamoDB are not included.
 
 
</details>

### 3. Use the following scenario: A company wants to run fault-tolerant batch jobs. Which compute option best suits their cost-optimization needs?

```bash
aws ec2 request-spot-fleet --spot-fleet-request-config file://config.json
```

- [ ] **A)** Spot Instances
- [ ] **B)** On-Demand Instances
- [ ] **C)** Reserved Instances
- [ ] **D)** Dedicated Hosts

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Spot Instances offer up to 90% discount and are ideal for fault-tolerant, stateless, or batch workloads that can handle interruptions.
 
 
</details>

### 4. What is the minimum storage duration charge for objects transitioned to S3 Standard-IA?

- [ ] **A)** 30 days
- [ ] **B)** 90 days
- [ ] **C)** 180 days
- [ ] **D)** No minimum

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> S3 Standard-IA has a minimum 30-day storage charge. Objects deleted earlier incur a cost equal to 30 days of storage.
 
 
</details>

### 5. Which two EBS volume types provide baseline performance independent of volume size? (Choose 2)

- [ ] **A)** gp3
- [ ] **B)** io2 Block Express
- [ ] **C)** st1 (Throughput Optimized HDD)
- [ ] **D)** sc1 (Cold HDD)

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> gp3 provides baseline 3,000 IOPS and 125 MiB/s regardless of size. io2 and HDD types have performance tied to capacity.
 
 
</details>

### 6. Examine the scenario: A company stores 10 KB log files and wants to archive them after 30 days. Which storage class should they avoid due to per-object overhead?

```bash
aws s3api put-object --bucket my-bucket --key logs/2024/01/01/file-001.log --body /tmp/file-001.log
```

- [ ] **A)** S3 Standard-IA
- [ ] **B)** S3 Glacier Deep Archive
- [ ] **C)** S3 One Zone-IA
- [ ] **D)** S3 Glacier Instant Retrieval

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Standard-IA and One Zone-IA have a minimum 128 KB charge per object, making small objects more expensive than Standard.
 
 
</details>

### 7. What is the default baseline IOPS for an Amazon EBS gp3 volume regardless of size?

- [ ] **A)** 3,000 IOPS
- [ ] **B)** 16,000 IOPS
- [ ] **C)** 125 IOPS
- [ ] **D)** Depends on volume size

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> gp3 provides 3,000 IOPS baseline and 125 MiB/s throughput, independent of the volume's capacity.
 
 
</details>

### 8. Which two strategies reduce data transfer costs within AWS? (Choose 2)

- [ ] **A)** Use VPC Gateway Endpoints for S3
- [ ] **B)** Place resources in the same Availability Zone
- [ ] **C)** Route traffic through a NAT Gateway
- [ ] **D)** Use public internet for all transfers

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> VPC endpoints keep traffic within AWS network; same AZ avoids cross-AZ charges; NAT and internet increase costs.
 
 
</details>


---

### **Design High-Performing Architectures**

### 9. Which AWS service provides a discount of up to 72% in exchange for a one- or three-year commitment to a specific instance family in a region?

- [ ] **A)** Savings Plans
- [ ] **B)** Spot Instances
- [ ] **C)** Reserved Instances
- [ ] **D)** On-Demand Instances

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: C**
 
> 💡  **Explanation** 
> 
> Reserved Instances (RIs) provide a significant discount of up to 72% for a one- or three-year commitment to a specific instance family in a region. Savings Plans offer similar discounts but with more flexibility across instance families and services.
 
 
</details>

### 10. Which of the following are valid S3 storage classes that can be used as part of a lifecycle policy to reduce costs? (Select two.)

- [ ] **A)** S3 Standard
- [ ] **B)** S3 Standard-IA
- [ ] **C)** S3 One Zone-IA
- [ ] **D)** S3 Glacier Instant Retrieval

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B, C**
 
> 💡  **Explanation** 
> 
> S3 Standard-IA and S3 One Zone-IA are both valid storage classes that can be transitioned to via lifecycle policies. S3 Glacier Instant Retrieval is also valid, but the question asks for two classes; Standard-IA and One Zone-IA are correct examples. S3 Standard is the default class, not typically used as a cost-saving transition target.
 
 
</details>

### 11. You have a set of log files stored in an S3 bucket. The logs are accessed frequently for the first 30 days, then rarely afterward. You want to minimize storage costs without losing immediate access to older logs. Based on the AWS documentation, which S3 storage class should you transition the logs to after 30 days? The lifecycle policy configuration is shown below.

```json
{
  "Rules": [
    {
      "Id": "LogTransition",
      "Status": "Enabled",
      "Prefix": "logs/",
      "Transitions": [
        {
          "Days": 30,
          "StorageClass": "STANDARD_IA"
        }
      ]
    }
  ]
}
```

- [ ] **A)** S3 Glacier Deep Archive
- [ ] **B)** S3 Glacier Flexible Retrieval
- [ ] **C)** S3 Standard-IA
- [ ] **D)** S3 One Zone-IA

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: C**
 
> 💡  **Explanation** 
> 
> S3 Standard-IA is designed for data that is accessed less frequently but requires rapid access when needed. It offers lower storage cost than S3 Standard and immediate retrieval. Glacier classes have retrieval delays, which do not meet the requirement for immediate access.
 
 
</details>

### 12. Which AWS service provides static Anycast IP addresses to route traffic to the nearest healthy endpoint using the AWS global network?

- [ ] **A)** Amazon CloudFront
- [ ] **B)** AWS Global Accelerator
- [ ] **C)** AWS Direct Connect
- [ ] **D)** AWS Transit Gateway

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> AWS Global Accelerator uses two static Anycast IP addresses and routes user traffic over the AWS global network to the nearest healthy endpoint, offering low latency and fast failover. CloudFront provides domain names and caches content; it does not offer fixed Anycast IPs.
 
 
</details>

### 13. Which of the following statements about VPC peering are accurate? (Select two.)

- [ ] **A)** VPC peering supports transitive routing across multiple peered VPCs.
- [ ] **B)** VPC peering creates a direct, one-to-one connection between two VPCs.
- [ ] **C)** VPC peering can route traffic between VPCs in different AWS Regions.
- [ ] **D)** VPC peering allows you to route traffic through a third VPC to reach another VPC.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B, C**
 
> 💡  **Explanation** 
> 
> VPC peering is a one-to-one connection that can be established between VPCs in the same or different regions (inter-region VPC peering). It does not support transitive routing – you cannot route traffic through a third VPC. Route tables must be manually configured.
 
 
</details>

### 14. You need to connect a corporate data center to AWS with a dedicated, low-latency link that bypasses the public internet. You also require encrypted traffic over this connection. Based on the AWS documentation, which two components must you use together? The configuration block shows a virtual interface and a VPN attachment.

```hcl
resource "aws_dx_private_virtual_interface" "dx_private" {
  connection_id = aws_dx_connection.main.id
  name           = "dx-private-vif"
  vlan           = 100
  address_family = "ipv4"
  bgp_asn        = 65000
}

resource "aws_vpn_connection" "dx_vpn" {
  customer_gateway_id = aws_customer_gateway.cgw.id
  transit_gateway_id  = aws_ec2_transit_gateway.tgw.id
  type                = "ipsec.1"
}
```

- [ ] **A)** Direct Connect private VIF and a VPN connection over the VIF
- [ ] **B)** Direct Connect public VIF and a VPN connection
- [ ] **C)** Site-to-Site VPN over the internet and Direct Connect public VIF
- [ ] **D)** Direct Connect private VIF and a transit gateway attachment

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> To have a dedicated link plus encryption, you use a Direct Connect private virtual interface (VIF) to provide a private path into AWS, then create an IPsec VPN tunnel over that private VIF. A public VIF only provides access to AWS public services and does not encrypt traffic.
 
 
</details>

### 15. Which AWS service is purpose-built for real-time, low-latency data ingestion with per-record processing and custom consumer logic?

- [ ] **A)** Amazon Kinesis Data Firehose
- [ ] **B)** Amazon Kinesis Data Streams
- [ ] **C)** AWS Glue Streaming
- [ ] **D)** Amazon Managed Streaming for Apache Kafka (MSK)

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> Amazon Kinesis Data Streams provides real-time ingestion with custom consumers (e.g., Lambda, KCL) for per-record, low-latency processing. Data Firehose is for near-real-time delivery without custom consumption. Glue Streaming and MSK are different services.
 
 
</details>


---

### **Design Resilient Architectures**

### 16. What is the primary purpose of a Multi-AZ deployment for Amazon RDS?

- [ ] **A)** Synchronous replication across AWS Regions for disaster recovery
- [ ] **B)** Automated failover to a standby instance in a different Availability Zone within the same region
- [ ] **C)** Read scalability by allowing the standby instance to serve traffic
- [ ] **D)** Asynchronous replication to multiple Regions for low-latency reads

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> RDS Multi-AZ provides a synchronous standby replica in a different Availability Zone within the same region. Automatic failover occurs if the primary fails, ensuring high availability. The standby cannot serve reads.
 
 
</details>

### 17. Which of the following are characteristics of DynamoDB Global Tables? (Select TWO)

- [ ] **A)** Supports multi-master writes across multiple AWS Regions
- [ ] **B)** Provides synchronous replication for zero data loss
- [ ] **C)** Replication is eventually consistent across regions
- [ ] **D)** Requires manual conflict resolution using custom application logic

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, C**
 
> 💡  **Explanation** 
> 
> DynamoDB Global Tables are multi-master and offer eventual consistency across regions. Conflict resolution is automatic using 'last writer wins'. Replication is asynchronous, not synchronous.
 
 
</details>

### 18. Examine the following Terraform configuration for an Auto Scaling group. What does the 'desired_capacity' attribute represent?

```hcl
resource "aws_autoscaling_group" "web_asg" {
  desired_capacity = 3
  min_size         = 1
  max_size         = 10
  vpc_zone_identifier = ["subnet-abc", "subnet-def"]
  launch_template {
    id      = aws_launch_template.web.id
    version = "$Latest"
  }
}
```

- [ ] **A)** The minimum number of instances that must always be running
- [ ] **B)** The initial number of instances the Auto Scaling group launches and maintains
- [ ] **C)** The maximum number of instances the Auto Scaling group can launch
- [ ] **D)** The number of instances that will be running in each Availability Zone

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> Desired capacity is the target number of instances the Auto Scaling group tries to maintain. It can be adjusted by scaling policies. It is not the minimum or maximum.
 
 
</details>

### 19. Which disaster recovery strategy keeps a minimal copy of core services (e.g., database) running in the DR region, with the rest of the environment powered off?

- [ ] **A)** Backup and Restore
- [ ] **B)** Pilot Light
- [ ] **C)** Warm Standby
- [ ] **D)** Multi-Site Active/Active

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> Pilot Light keeps a small core of persistent data services (like a database) running in the DR region. Other compute resources are not active; they are started only upon failover.
 
 
</details>

### 20. Which of the following are characteristics of Amazon SQS FIFO queues? (Select THREE)

- [ ] **A)** Guarantees exactly-once processing, even with multiple consumers
- [ ] **B)** Provides first-in-first-out delivery of messages
- [ ] **C)** Supports a throughput of up to 3,000 messages per second with batching
- [ ] **D)** Supports unlimited throughput by adding more consumers

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B, C**
 
> 💡  **Explanation** 
> 
> FIFO queues guarantee exactly-once processing and preserve message order. Throughput is limited to 3,000 TPS with batching (300 without). Adding more consumers does not increase throughput; that applies to Standard queues.
 
 
</details>

### 21. Review the CloudFormation snippet below for an RDS instance. What does the 'MultiAZ' parameter set to 'true' accomplish?

```yaml
MyDB:
  Type: AWS::RDS::DBInstance
  Properties:
    Engine: MySQL
    MasterUsername: admin
    MasterUserPassword: secret
    DBInstanceClass: db.m5.large
    MultiAZ: true
    StorageType: gp3
    AllocatedStorage: 100
```

- [ ] **A)** It creates a cross-region read replica
- [ ] **B)** It provisions a synchronous standby in a different Availability Zone within the same region
- [ ] **C)** It enables automated backups across multiple regions
- [ ] **D)** It allows the standby instance to serve read traffic

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> MultiAZ=true creates a synchronous standby in a different AZ within the same region for automatic failover. It does not create read replicas or cross-region capabilities.
 
 
</details>

### 22. Which AWS service can be used to achieve sub-second failover across multiple AWS Regions for an Internet-facing application?

- [ ] **A)** Amazon Route 53 with failover routing
- [ ] **B)** AWS Global Accelerator
- [ ] **C)** Application Load Balancer with cross-zone load balancing
- [ ] **D)** Amazon CloudFront with multiple origins

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> AWS Global Accelerator provides two static anycast IPs that route traffic to healthy region endpoints. It can achieve sub-second failover, faster than DNS-based routing like Route 53 failover (which is limited by TTL and health check intervals).
 
 
</details>


---

### **Design Secure Architectures**

### 23. What is the primary function of a Service Control Policy (SCP) in AWS?

- [ ] **A)** Grants permissions to IAM users
- [ ] **B)** Restricts permissions at the account level
- [ ] **C)** Manages user identities across accounts
- [ ] **D)** Encrypts data at rest for services

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> SCPs are permission guardrails that only restrict what IAM policies can allow; they never grant permissions themselves.
 
 
</details>

### 24. Which two statements about Service Control Policies (SCPs) are correct?

- [ ] **A)** They can be applied to the management account.
- [ ] **B)** They only deny or allow actions; they never grant permissions.
- [ ] **C)** They grant permissions to IAM roles.
- [ ] **D)** They apply to all principals in an account except the management account.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B, D**
 
> 💡  **Explanation** 
> 
> SCPs are evaluated before IAM policies. They cannot grant permissions and do not affect the management account.
 
 
</details>

### 25. Based on the provided key policy, which principal can use this KMS key for encryption?

```json
{
  "Version": "2012-10-17",
  "Id": "key-consolepolicy-3",
  "Statement": [
    {
      "Sid": "Enable IAM User Permissions",
      "Effect": "Allow",
      "Principal": {
        "AWS": "arn:aws:iam::111122223333:role/AdminRole"
      },
      "Action": "kms:Encrypt",
      "Resource": "*"
    }
  ]
}
```

- [ ] **A)** IAM role AdminRole in account 111122223333
- [ ] **B)** Any user in account 111122223333
- [ ] **C)** The root user of account 111122223333
- [ ] **D)** All IAM users in the organization

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The key policy explicitly grants kms:Encrypt to the IAM role AdminRole in the specified account.
 
 
</details>

### 26. What does AWS Secrets Manager primarily do?

- [ ] **A)** Store and rotate database credentials automatically
- [ ] **B)** Create encryption keys for S3
- [ ] **C)** Manage TLS certificates for load balancers
- [ ] **D)** Monitor VPC flow logs

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Secrets Manager securely stores secrets like database credentials and can automatically rotate them using Lambda.
 
 
</details>

### 27. Which two services are supported by Gateway VPC Endpoints?

- [ ] **A)** Amazon S3
- [ ] **B)** Amazon DynamoDB
- [ ] **C)** Amazon Kinesis
- [ ] **D)** AWS Lambda

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> Only S3 and DynamoDB support Gateway Endpoints; all other AWS services use Interface Endpoints.
 
 
</details>

### 28. Based on the NACL rule table, which inbound traffic is allowed?

```plaintext
# Inbound NACL rules
# Rule 100: Allow SSH from 10.0.0.0/16
# Rule 200: Deny all other inbound (implicit deny)
# Format: Rule#, Type, Protocol, Port Range, Source, Allow/Deny
100, SSH (22), TCP, 22, 10.0.0.0/16, ALLOW
200, All traffic, ALL, ALL, 0.0.0.0/0, DENY
```

- [ ] **A)** SSH on port 22 from 10.0.0.0/16
- [ ] **B)** HTTP on port 80 from 0.0.0.0/0
- [ ] **C)** HTTPS on port 443 from 192.168.0.0/24
- [ ] **D)** All inbound traffic is denied

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The NACL rule explicitly allows TCP port 22 from the 10.0.0.0/16 range. Other rules deny or do not apply.
 
 
</details>

### 29. Which AWS service provides a centralized backup management across services?

- [ ] **A)** AWS Backup
- [ ] **B)** Amazon S3
- [ ] **C)** AWS CloudTrail
- [ ] **D)** AWS Config

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> AWS Backup provides a unified console to configure backup plans, set retention, and monitor backups across supported services.
 
 
</details>

### 30. Which two features provide immutability for backups in AWS?

- [ ] **A)** Backup Vault Lock
- [ ] **B)** S3 Object Lock
- [ ] **C)** S3 Versioning
- [ ] **D)** Lifecycle policies

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> Backup Vault Lock (for AWS Backup) and S3 Object Lock (for S3 buckets) prevent deletion of backups, ensuring immutability.
 
 
</details>
