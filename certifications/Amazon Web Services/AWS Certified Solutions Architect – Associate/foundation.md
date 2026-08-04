<table width="100%">
  <tr>
    <td align="center" valign="middle" width="50%">
      <p align="center"><img src="https://pub-6a9f8dede1194a7786cba69e7dcdad9f.r2.dev/certifications/Amazon%20Web%20Services%20Training%20and%20Certification/AWS%20Certified%20Solutions%20Architect%20%E2%80%93%20Associate" width="50%"></p>
    </td>
    <td align="center" valign="middle" width="50%">
      <h1>AWS Certified Solutions Architect – Associate</h1>
    </td>
  </tr>
</table>

## 📑 Table of Contents

- [Design Cost-Optimized Architectures](#design-cost-optimized-architectures) (6 questions)
- [Design High-Performing Architectures](#design-high-performing-architectures) (7 questions)
- [Design Resilient Architectures](#design-resilient-architectures) (8 questions)
- [Design Secure Architectures](#design-secure-architectures) (9 questions)

## 📋 Exam Information

| Field | Value |
|-------|-------|
| Total Questions | 30 |
| Level | Foundation |
| Exported At | 2026-08-04T06:25:36.916Z |
| Domains | 4 |

## 📊 Domain Distribution

| Domain | Questions |
|--------|-----------|
| Design Cost-Optimized Architectures | 6 |
| Design High-Performing Architectures | 7 |
| Design Resilient Architectures | 8 |
| Design Secure Architectures | 9 |

---

### **Design Cost-Optimized Architectures**

### 1. Which S3 storage class is designed for frequently accessed data with the highest durability?

- [ ] **A)** S3 Standard
- [ ] **B)** S3 Standard-IA
- [ ] **C)** S3 One Zone-IA
- [ ] **D)** S3 Glacier Deep Archive

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> S3 Standard provides low-latency access and 99.999999999% durability for frequently accessed data.
 
 
</details>

### 2. Which of the following are true about S3 Standard-IA? (Select two)

- [ ] **A)** Lower storage cost than S3 Standard
- [ ] **B)** No retrieval fee
- [ ] **C)** 30-day minimum storage duration
- [ ] **D)** Retrieval time of minutes to hours

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, C**
 
> 💡  **Explanation** 
> 
> S3 Standard-IA has a lower storage cost than S3 Standard and a 30-day minimum storage duration. It incurs retrieval fees and provides millisecond retrieval.
 
 
</details>

### 3. Based on the provided lifecycle configuration, which storage class do objects with the 'logs/' prefix move to after 90 days?

```json
{
  "Rules": [
    {
      "Id": "LogLifecycle",
      "Status": "Enabled",
      "Filter": {"Prefix": "logs/"},
      "Transitions": [
        {
          "Days": 30,
          "StorageClass": "STANDARD_IA"
        },
        {
          "Days": 90,
          "StorageClass": "GLACIER"
        }
      ]
    }
  ]
}
```

- [ ] **A)** S3 Standard
- [ ] **B)** S3 Standard-IA
- [ ] **C)** S3 Glacier Flexible Retrieval
- [ ] **D)** S3 Glacier Deep Archive

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: C**
 
> 💡  **Explanation** 
> 
> The lifecycle rule transitions objects from S3 Standard (default) to STANDARD_IA after 30 days, then to GLACIER after 90 days, which corresponds to S3 Glacier Flexible Retrieval.
 
 
</details>

### 4. Which Amazon EBS volume type provides a baseline performance of 3,000 IOPS and is recommended as a cost-effective choice for most workloads?

- [ ] **A)** gp2
- [ ] **B)** gp3
- [ ] **C)** io1
- [ ] **D)** st1

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> EBS gp3 offers a baseline of 3,000 IOPS and 125 MB/s throughput at a 20% lower cost than gp2, making it cost-effective for most workloads.
 
 
</details>

### 5. Which of the following are features of S3 Intelligent-Tiering? (Select two)

- [ ] **A)** No retrieval fees
- [ ] **B)** Fixed monthly storage fee per object
- [ ] **C)** Requires a 30-day minimum storage commitment
- [ ] **D)** Only moves objects between two tiers

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> S3 Intelligent-Tiering charges a small monthly monitoring fee per object but no retrieval fees, and it automatically moves objects between four access tiers. It has no minimum storage commitment.
 
 
</details>

### 6. The following AWS CLI command describes an EC2 instance purchase. What purchase model is being used?

```json
{ "InstanceId": "i-0abcdef1234567890", "InstanceType": "t3.medium", "InstanceLifecycle": "spot", "State": "running" }
```

- [ ] **A)** On-Demand
- [ ] **B)** Reserved Instance
- [ ] **C)** Spot Instance
- [ ] **D)** Dedicated Host

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: C**
 
> 💡  **Explanation** 
> 
> The 'InstanceLifecycle' field set to 'spot' indicates this is a Spot Instance, which offers significant discounts but can be reclaimed.
 
 
</details>


---

### **Design High-Performing Architectures**

### 7. What is the maximum number of GET/HEAD requests per second that a single S3 prefix can support?

- [ ] **A)** 3,500
- [ ] **B)** 5,500
- [ ] **C)** 10,000
- [ ] **D)** 15,000

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> A single S3 prefix supports 5,500 GET/HEAD requests per second. Exceeding this requires prefix sharding.
 
 
</details>

### 8. Which of the following are valid EBS volume types? (Select two.)

- [ ] **A)** gp3
- [ ] **B)** io2
- [ ] **C)** st2
- [ ] **D)** ef1

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> Valid EBS types include gp3 (general purpose) and io2 (provisioned IOPS). st2 and ef1 do not exist.
 
 
</details>

### 9. Review the following CloudFormation snippet. Which EBS volume type is being provisioned?

```yaml
Resources:
  MyVolume:
    Type: AWS::EC2::Volume
    Properties:
      Size: 100
      VolumeType: gp3
      AvailabilityZone: us-east-1a
```

- [ ] **A)** gp2
- [ ] **B)** gp3
- [ ] **C)** io1
- [ ] **D)** st1

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> The code specifies VolumeType: gp3, which is a general purpose SSD volume with baseline performance.
 
 
</details>

### 10. Which AWS service provides a fully managed NFS file system that can be mounted on multiple EC2 instances?

- [ ] **A)** Amazon EBS
- [ ] **B)** Amazon EFS
- [ ] **C)** Amazon S3
- [ ] **D)** Amazon FSx

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> Amazon EFS is a fully managed NFS file system that can be concurrently accessed by multiple EC2 instances.
 
 
</details>

### 11. Which of the following are performance modes available for Amazon EFS? (Select two.)

- [ ] **A)** General Purpose
- [ ] **B)** Max I/O
- [ ] **C)** High Throughput
- [ ] **D)** Low Latency

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> EFS offers General Purpose (low latency) and Max I/O (high throughput) performance modes.
 
 
</details>

### 12. Review the following Terraform snippet. Which EFS performance mode is being set?

```hcl
resource "aws_efs_file_system" "my_efs" {
  creation_token = "my-efs"
  performance_mode = "generalPurpose"
  throughput_mode = "bursting"
}
```

- [ ] **A)** generalPurpose
- [ ] **B)** maxIO
- [ ] **C)** bursting
- [ ] **D)** provisioned

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The code sets performance_mode = \"generalPurpose\", which provides low latency for latency-sensitive applications.
 
 
</details>

### 13. Which AWS service offers a file system optimized for high-performance computing (HPC) with sub-millisecond latency?

- [ ] **A)** Amazon EFS
- [ ] **B)** Amazon FSx for Lustre
- [ ] **C)** Amazon S3
- [ ] **D)** Amazon EBS

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> FSx for Lustre is a high-performance file system optimized for HPC, machine learning, and media processing.
 
 
</details>


---

### **Design Resilient Architectures**

### 14. What is the primary purpose of an Auto Scaling Group in AWS?

- [ ] **A)** Manually adjust EC2 instance count
- [ ] **B)** Automatically adjust EC2 instance count based on demand
- [ ] **C)** Create EC2 instances in a single Availability Zone
- [ ] **D)** Provide a static set of EC2 instances

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> Auto Scaling automatically adjusts the number of EC2 instances to meet demand, improving scalability and cost-efficiency.
 
 
</details>

### 15. Which two components are essential for building a loosely coupled architecture on AWS? (Choose two.)

- [ ] **A)** Amazon SQS
- [ ] **B)** Amazon SNS
- [ ] **C)** Elastic Load Balancing
- [ ] **D)** AWS Lambda

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> SQS decouples with message queues, SNS decouples with pub/sub. ELB and Lambda are load balancing and compute, not decoupling mechanisms.
 
 
</details>

### 16. Given the provided CloudFormation snippet, what resource is being created that enables horizontal scaling?

```yaml
Resources:
  MyASG:
    Type: AWS::AutoScaling::AutoScalingGroup
    Properties:
      MinSize: '1'
      MaxSize: '5'
      DesiredCapacity: '2'
      LaunchConfigurationName: !Ref MyLaunchConfig
      VPCZoneIdentifier: [!Ref PublicSubnet1, !Ref PublicSubnet2]
```

- [ ] **A)** Auto Scaling Group
- [ ] **B)** Launch Configuration
- [ ] **C)** Elastic Load Balancer
- [ ] **D)** EC2 Instance

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The AWS::AutoScaling::AutoScalingGroup resource defines an Auto Scaling Group for automatic scaling.
 
 
</details>

### 17. What is the maximum Lambda function execution timeout?

- [ ] **A)** 5 minutes
- [ ] **B)** 15 minutes
- [ ] **C)** 30 minutes
- [ ] **D)** 60 minutes

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> Lambda functions have a maximum timeout of 15 minutes (900 seconds).
 
 
</details>

### 18. Which two statements about SQS Standard queues are true? (Choose two.)

- [ ] **A)** At-least-once delivery
- [ ] **B)** Exactly-once processing
- [ ] **C)** Best-effort ordering
- [ ] **D)** Strict FIFO ordering

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, C**
 
> 💡  **Explanation** 
> 
> Standard queues offer at-least-once delivery and best-effort ordering. FIFO queues offer exactly-once and strict ordering.
 
 
</details>

### 19. Examine the Terraform snippet. Which service is used to distribute traffic across multiple targets?

```hcl
resource "aws_lb" "my_alb" {
  name               = "my-alb"
  internal           = false
  load_balancer_type = "application"
  subnets            = ["subnet-abc", "subnet-def"]
}
```

- [ ] **A)** Application Load Balancer
- [ ] **B)** Network Load Balancer
- [ ] **C)** Classic Load Balancer
- [ ] **D)** Route 53

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The resource 'aws_lb' with type 'application' creates an Application Load Balancer.
 
 
</details>

### 20. Which AWS service decouples producers and consumers using a message queue?

- [ ] **A)** Amazon SNS
- [ ] **B)** Amazon SQS
- [ ] **C)** AWS Lambda
- [ ] **D)** Amazon Kinesis

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> SQS is a fully managed message queuing service for decoupling application components.
 
 
</details>

### 21. Which two types of Elastic Load Balancers operate at Layer 7? (Choose two.)

- [ ] **A)** Application Load Balancer
- [ ] **B)** Network Load Balancer
- [ ] **C)** Classic Load Balancer
- [ ] **D)** Gateway Load Balancer

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Only ALB operates at Layer 7. NLB and GLB operate at Layer 4, CLB is legacy.
 
 
</details>


---

### **Design Secure Architectures**

### 22. What type of credentials does an IAM role provide when assumed?

- [ ] **A)** Temporary credentials
- [ ] **B)** Long-term access keys
- [ ] **C)** SSH key pairs
- [ ] **D)** MFA device serial numbers

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> IAM roles provide temporary credentials via AWS Security Token Service (STS). These credentials are automatically rotated and are the best practice for granting permissions to services or federated users.
 
 
</details>

### 23. Which two types of IAM policies are available in AWS? (Choose two.)

- [ ] **A)** Identity-based policies
- [ ] **B)** Resource-based policies
- [ ] **C)** Service control policies
- [ ] **D)** Session policies

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> IAM policies can be identity-based (attached to users, groups, or roles) or resource-based (attached to resources like S3 buckets). SCPs are a separate feature of AWS Organizations.
 
 
</details>

### 24. Examine the IAM trust policy below. Which entity is allowed to assume the role?

```json
{
  "Version": "2012-10-17",
  "Statement": [
    {
      "Effect": "Allow",
      "Principal": {
        "Service": "ec2.amazonaws.com"
      },
      "Action": "sts:AssumeRole"
    }
  ]
}
```

- [ ] **A)** The EC2 service
- [ ] **B)** An IAM user in the same account
- [ ] **C)** Any AWS account
- [ ] **D)** An IAM group

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The trust policy allows the EC2 service principal (ec2.amazonaws.com) to assume the role. This is commonly used to grant an EC2 instance permissions via an instance profile.
 
 
</details>

### 25. What is the primary function of Service Control Policies (SCPs) in AWS Organizations?

- [ ] **A)** Define maximum available permissions for accounts
- [ ] **B)** Grant permissions to IAM users
- [ ] **C)** Encrypt data at rest
- [ ] **D)** Monitor API activity

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> SCPs allow you to centrally control the maximum permissions for all accounts in your organization. They act as guardrails that can restrict what actions even an IAM administrator can perform.
 
 
</details>

### 26. Which AWS services are commonly used for defense in depth in a web application? (Choose two.)

- [ ] **A)** AWS WAF
- [ ] **B)** AWS Shield
- [ ] **C)** AWS Direct Connect
- [ ] **D)** AWS Data Pipeline

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> WAF and Shield are part of the defense-in-depth strategy. WAF protects against web exploits, and Shield protects against DDoS attacks. Direct Connect and Data Pipeline are not security services.
 
 
</details>

### 27. Examine the S3 bucket policy snippet. What does the condition enforce?

```json
{
  "Version": "2012-10-17",
  "Statement": [
    {
      "Effect": "Deny",
      "Principal": "*",
      "Action": "s3:*",
      "Resource": "arn:aws:s3:::my-bucket/*",
      "Condition": {
        "Bool": {
          "aws:SecureTransport": "false"
        }
      }
    }
  ]
}
```

- [ ] **A)** All requests must use HTTPS
- [ ] **B)** Only GET requests are allowed
- [ ] **C)** Only requests from a specific IP range
- [ ] **D)** All requests must include MFA

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The condition 'aws:SecureTransport': 'false' in the Deny statement forces all requests to use HTTPS (SecureTransport). Without this, HTTP requests would be allowed.
 
 
</details>

### 28. What does the principle of least privilege (PoLP) require?

- [ ] **A)** Grant only the permissions necessary to perform a function
- [ ] **B)** Grant all permissions and then remove those not needed
- [ ] **C)** Grant the same permissions to all users
- [ ] **D)** Grant administrative access to all developers

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The principle of least privilege dictates that you should grant the minimum set of permissions required for a user, role, or service to perform its intended tasks. This reduces security risk.
 
 
</details>

### 29. Which are best practices for securing an EC2 instance? (Choose two.)

- [ ] **A)** Use an IAM role to grant permissions
- [ ] **B)** Restrict inbound traffic with security groups
- [ ] **C)** Disable all encryption
- [ ] **D)** Use the same SSH key for all instances

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> Using IAM roles (instance profiles) avoids hardcoding keys, and security groups control inbound traffic. Disabling encryption and sharing SSH keys are insecure practices.
 
 
</details>

### 30. Examine the KMS key policy. Which AWS account is granted decryption permission?

```json
{
  "Version": "2012-10-17",
  "Statement": [
    {
      "Effect": "Allow",
      "Principal": {
        "AWS": "arn:aws:iam::111122223333:role/AppRole"
      },
      "Action": "kms:Decrypt",
      "Resource": "*"
    }
  ]
}
```

- [ ] **A)** 111122223333
- [ ] **B)** 444455556666
- [ ] **C)** The same account that owns the key
- [ ] **D)** Only the root user

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The policy grants kms:Decrypt to account 111122223333. The other account IDs are not listed. This enables cross-account decryption.
 
 
</details>
