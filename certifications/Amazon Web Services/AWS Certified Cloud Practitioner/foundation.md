<table width="100%">
  <tr>
    <td align="center" valign="middle" width="50%">
      <p align="center"><img src="https://pub-6a9f8dede1194a7786cba69e7dcdad9f.r2.dev/certifications/Amazon%20Web%20Services%20Training%20and%20Certification/AWS%20Certified%20Cloud%20Practitioner" width="50%"></p>
    </td>
    <td align="center" valign="middle" width="50%">
      <h1>AWS Certified Cloud Practitioner</h1>
    </td>
  </tr>
</table>

## 📑 Table of Contents

- [Billing, Pricing, and Support](#billing-pricing-and-support) (4 questions)
- [Cloud Concepts](#cloud-concepts) (7 questions)
- [Cloud Technology and Services](#cloud-technology-and-services) (10 questions)
- [Security and Compliance](#security-and-compliance) (9 questions)

## 📋 Exam Information

| Field | Value |
|-------|-------|
| Total Questions | 30 |
| Level | Foundation |
| Exported At | 2026-08-04T06:25:20.626Z |
| Domains | 4 |

## 📊 Domain Distribution

| Domain | Questions |
|--------|-----------|
| Billing, Pricing, and Support | 4 |
| Cloud Concepts | 7 |
| Cloud Technology and Services | 10 |
| Security and Compliance | 9 |

---

### **Billing, Pricing, and Support**

### 1. What is a key characteristic of AWS On-Demand pricing?

- [ ] **A)** No long-term commitment required
- [ ] **B)** Requires a 1-year commitment
- [ ] **C)** Offers up to 90% discount
- [ ] **D)** Only applies to EC2 instances

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> On-Demand pricing charges per hour/second with no upfront commitment, offering maximum flexibility at the highest cost.
 
 
</details>

### 2. Which AWS resources are used for cost management? (Select three.)

- [ ] **A)** Cost Explorer
- [ ] **B)** AWS Budgets
- [ ] **C)** AWS Config
- [ ] **D)** Consolidated Billing

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B, D**
 
> 💡  **Explanation** 
> 
> Cost Explorer, AWS Budgets, and Consolidated Billing are core cost management tools. AWS Config is for resource inventory and compliance.
 
 
</details>

### 3. Given the following support case details, which AWS Support plan provides this response time?

```json
{
  "severity": "critical",
  "response_time": "30 minutes"
}
```

- [ ] **A)** Business
- [ ] **B)** Enterprise On-Ramp
- [ ] **C)** Enterprise
- [ ] **D)** Developer

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> Enterprise On-Ramp offers <30 minute critical response time. Enterprise is <15 minutes, Business <1 hour, Developer not supported.
 
 
</details>

### 4. How long do AWS 12-month Free Tier offers last?

- [ ] **A)** 6 months
- [ ] **B)** 12 months
- [ ] **C)** 24 months
- [ ] **D)** Never expire

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> 12-month Free Tier offers are available for 12 months starting from the account creation date, not from first use.
 
 
</details>


---

### **Cloud Concepts**

### 5. Which of the following best describes the AWS Cloud's pay-as-you-go pricing model?

- [ ] **A)** It requires a large upfront capital investment and then charges monthly fees.
- [ ] **B)** It converts capital expenditure (CapEx) into variable operational expenditure (OpEx).
- [ ] **C)** It offers a fixed monthly rate for unlimited usage of all services.
- [ ] **D)** It charges a flat annual fee regardless of resource consumption.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> Pay-as-you-go pricing allows customers to pay only for the resources they consume, without upfront commitments. This shifts IT spending from CapEx (buying hardware) to OpEx (variable usage costs), improving cash flow and financial flexibility.
 
 
</details>

### 6. Which of the following are key benefits of AWS Cloud elasticity? (Select TWO.)

- [ ] **A)** Eliminates the need for capacity planning
- [ ] **B)** Automatically scales resources to match real-time demand
- [ ] **C)** Ensures a fixed amount of compute capacity at all times
- [ ] **D)** Reduces waste by avoiding over-provisioning

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B, D**
 
> 💡  **Explanation** 
> 
> Elasticity allows resources to automatically increase or decrease in response to demand, preventing both under-provisioning (performance issues) and over-provisioning (wasted cost). It does not eliminate capacity planning entirely (you still set scaling policies), and it does not fix capacity—it adjusts dynamically.
 
 
</details>

### 7. Analyze the following AWS CLI command. What does it primarily demonstrate about cloud computing?

```bash
aws ec2 run-instances --image-id ami-0abcdef1234567890 --instance-type t2.micro --key-name MyKeyPair
```

- [ ] **A)** Multi-tenancy
- [ ] **B)** Broad network access
- [ ] **C)** Rapid elasticity
- [ ] **D)** Self-service provisioning

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: D**
 
> 💡  **Explanation** 
> 
> The command 'aws ec2 run-instances' allows a user to provision a virtual server directly from the CLI without any human interaction with AWS staff. This demonstrates self-service provisioning, a key attribute of cloud computing where users can obtain and configure resources on demand.
 
 
</details>

### 8. Which concept explains why AWS can offer lower prices for compute and storage compared to a single organization running its own data center?

- [ ] **A)** Reserved Instances
- [ ] **B)** Pay-as-you-go pricing
- [ ] **C)** Economies of scale
- [ ] **D)** Multi-region deployment

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: C**
 
> 💡  **Explanation** 
> 
> AWS aggregates usage from millions of customers, achieving massive economies of scale. This allows AWS to purchase hardware, bandwidth, and power at volume discounts, passing the savings to customers through lower prices. Reserved Instances and pay-as-you-go are pricing models, not the root cause of lower costs.
 
 
</details>

### 9. Which of the following are characteristics of the AWS Shared Responsibility Model? (Select TWO.)

- [ ] **A)** AWS is responsible for securing the physical infrastructure of data centers.
- [ ] **B)** Customers are responsible for patching the operating system on their Amazon RDS databases.
- [ ] **C)** AWS is responsible for all security aspects, including customer data.
- [ ] **D)** Customers are responsible for managing Identity and Access Management (IAM) policies.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, D**
 
> 💡  **Explanation** 
> 
> Under the shared responsibility model, AWS secures the cloud (physical data centers, hardware, hypervisor) while customers secure what they put in the cloud (data, IAM, OS patches on EC2, network configuration). RDS is a managed service where AWS handles OS patching; customers manage IAM and data encryption.
 
 
</details>

### 10. The following snippet is from an AWS CloudFormation template. What Well-Architected Framework design principle does this represent?

```yaml
Resources:
  MyEC2Instance:
    Type: 'AWS::EC2::Instance'
    Properties:
      InstanceType: t2.micro
      ImageId: ami-0abcdef1234567890
```

- [ ] **A)** Perform operations as code
- [ ] **B)** Stop guessing capacity
- [ ] **C)** Implement a strong identity foundation
- [ ] **D)** Enable traceability

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Using Infrastructure as Code (like CloudFormation) to define and provision infrastructure is a key design principle of the Operational Excellence pillar. It enables repeatable, version-controlled deployments and reduces manual error. The other options are valid principles but are not directly illustrated by the code snippet.
 
 
</details>

### 11. A company runs a web application on a single EC2 instance. Which AWS Cloud benefit would be most directly achieved by deploying the application across two Availability Zones?

- [ ] **A)** Elasticity
- [ ] **B)** Cost savings
- [ ] **C)** High availability
- [ ] **D)** Security

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: C**
 
> 💡  **Explanation** 
> 
> Deploying across multiple Availability Zones provides high availability by allowing the application to survive a failure in one AZ. Elasticity is about scaling based on demand, not geographic redundancy. Cost savings and security are not the direct benefits of multi-AZ deployment, though they may be secondary effects.
 
 
</details>


---

### **Cloud Technology and Services**

### 12. Which AWS deployment method provides a web-based graphical interface for manual resource creation?

- [ ] **A)** AWS Management Console
- [ ] **B)** AWS CLI
- [ ] **C)** AWS CloudFormation
- [ ] **D)** AWS Elastic Beanstalk

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The AWS Management Console is a GUI for manual resource creation, ideal for one-off tasks and learning.
 
 
</details>

### 13. Which two benefits does AWS CloudFormation provide over the AWS Management Console?

- [ ] **A)** Repeatable and consistent deployments
- [ ] **B)** Version-controlled infrastructure templates
- [ ] **C)** Lower total cost for small environments
- [ ] **D)** Faster learning curve for new users

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> CloudFormation templates enable repeatable, version-controlled deployments, while the console is manual and not scalable.
 
 
</details>

### 14. Review the AWS CloudFormation code below. Which AWS resource is being defined?

```yaml
Resources:
  MyEC2Instance:
    Type: AWS::EC2::Instance
    Properties:
      InstanceType: t2.micro
      ImageId: ami-0abcdef1234567890
```

- [ ] **A)** Amazon EC2 instance
- [ ] **B)** Amazon S3 bucket
- [ ] **C)** AWS IAM role
- [ ] **D)** Amazon VPC

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The template defines an AWS::EC2::Instance resource, creating a virtual machine.
 
 
</details>

### 15. Which AWS compute service is fully managed and runs code without provisioning servers?

- [ ] **A)** AWS Lambda
- [ ] **B)** Amazon EC2
- [ ] **C)** AWS Elastic Beanstalk
- [ ] **D)** Amazon ECS

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> AWS Lambda is a serverless compute service that runs code in response to events without provisioning servers.
 
 
</details>

### 16. Which two AWS storage services are designed for object storage?

- [ ] **A)** Amazon S3
- [ ] **B)** Amazon EBS
- [ ] **C)** Amazon S3 Glacier
- [ ] **D)** Amazon EFS

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, C**
 
> 💡  **Explanation** 
> 
> Amazon S3 and Amazon S3 Glacier (S3's archival class) are object storage services. EBS and EFS are block and file storage respectively.
 
 
</details>

### 17. Examine the AWS CLI command below. Which service does it interact with?

```bash
aws s3 cp myfile.txt s3://my-bucket/
```

- [ ] **A)** Amazon S3
- [ ] **B)** Amazon EC2
- [ ] **C)** Amazon RDS
- [ ] **D)** AWS Lambda

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The 'aws s3 cp' command copies files to/from Amazon S3, indicating interaction with the S3 service.
 
 
</details>

### 18. Which AWS database service is a fully managed NoSQL key-value and document database?

- [ ] **A)** Amazon DynamoDB
- [ ] **B)** Amazon RDS
- [ ] **C)** Amazon Aurora
- [ ] **D)** Amazon Redshift

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Amazon DynamoDB is a fully managed NoSQL database delivering single-digit millisecond performance, ideal for key-value and document workloads.
 
 
</details>

### 19. Which two AWS networking services operate at the global level?

- [ ] **A)** Amazon Route 53
- [ ] **B)** Amazon CloudFront
- [ ] **C)** Amazon VPC
- [ ] **D)** AWS Direct Connect

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> Route 53 (DNS) and CloudFront (CDN) are global services. VPC and Direct Connect are regional or point-to-point.
 
 
</details>

### 20. Refer to the AWS SDK code snippet. Which AWS service is the code accessing?

```python
import boto3
s3 = boto3.client('s3')
s3.put_object(Bucket='my-bucket', Key='hello.txt', Body='Hello World')
```

- [ ] **A)** Amazon S3
- [ ] **B)** Amazon DynamoDB
- [ ] **C)** Amazon SQS
- [ ] **D)** Amazon EC2

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The 'put_object' method is part of the boto3 S3 client, indicating interaction with Amazon S3.
 
 
</details>

### 21. Which AWS service is used to decouple application components via message queuing?

- [ ] **A)** Amazon SQS
- [ ] **B)** Amazon SNS
- [ ] **C)** Amazon API Gateway
- [ ] **D)** AWS Step Functions

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Amazon SQS is a fully managed message queuing service that decouples application components.
 
 
</details>


---

### **Security and Compliance**

### 22. Under the AWS Shared Responsibility Model, which of the following is a customer responsibility?

- [ ] **A)** Physical security of data centers
- [ ] **B)** Patching the guest operating system on EC2 instances
- [ ] **C)** Security of the hypervisor
- [ ] **D)** Global network infrastructure

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> The customer is responsible for security in the cloud, including patching the guest OS on EC2 instances. AWS handles physical security, hypervisor security, and global network infrastructure.
 
 
</details>

### 23. Which two AWS services help customers demonstrate compliance with regulatory requirements? (Choose two.)

- [ ] **A)** AWS Artifact
- [ ] **B)** Amazon GuardDuty
- [ ] **C)** Amazon Inspector
- [ ] **D)** AWS Config

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, D**
 
> 💡  **Explanation** 
> 
> AWS Artifact provides on-demand access to compliance reports and agreements. AWS Config evaluates resource configurations against desired rules to help maintain compliance. GuardDuty and Inspector focus on threat detection and vulnerability scanning, not compliance documentation or auditing.
 
 
</details>

### 24. Refer to the IAM policy below. What action does this policy allow on the specified S3 bucket?

```json
{
  "Version": "2012-10-17",
  "Statement": [
    {
      "Effect": "Allow",
      "Action": "s3:GetObject",
      "Resource": "arn:aws:s3:::my-bucket/*"
    }
  ]
}
```

- [ ] **A)** s3:ListBucket
- [ ] **B)** s3:PutObject
- [ ] **C)** s3:GetObject
- [ ] **D)** s3:DeleteObject

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: C**
 
> 💡  **Explanation** 
> 
> The policy allows the s3:GetObject action on the bucket named 'my-bucket'. The Resource specifies the bucket and all objects within it, and the Action lists s3:GetObject.
 
 
</details>

### 25. Which AWS service provides temporary, rotating credentials for accessing AWS resources?

- [ ] **A)** IAM user with access keys
- [ ] **B)** IAM role attached to an instance profile
- [ ] **C)** AWS Organizations service control policy
- [ ] **D)** AWS CloudTrail log

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> An IAM role attached to an instance profile provides temporary credentials via AWS STS. IAM users have long-term keys, SCPs set boundaries, and CloudTrail logs are not for credentials.
 
 
</details>

### 26. Which two statements about the AWS Shared Responsibility Model are accurate? (Choose two.)

- [ ] **A)** AWS is responsible for physical security of data centers.
- [ ] **B)** The customer is responsible for patching the hypervisor on EC2 hosts.
- [ ] **C)** The customer is always responsible for managing their data.
- [ ] **D)** AWS is responsible for configuring customer IAM policies.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, C**
 
> 💡  **Explanation** 
> 
> AWS handles physical security, and the customer is always responsible for their data. AWS does not patch hypervisors (that is AWS's job) nor configure customer IAM policies.
 
 
</details>

### 27. Review the sample GuardDuty finding JSON. What type of activity is being reported?

```json
{
  "version": "0",
  "id": "abc123",
  "detail-type": "GuardDuty Finding",
  "source": "aws.guardduty",
  "detail": {
    "type": "UnauthorizedAccess:EC2/PortScan",
    "service": {
      "action": {
        "networkConnectionAction": {
          "connectionDirection": "OUTBOUND",
          "remoteIpDetails": {
            "ipAddressV4": "198.51.100.1"
          }
        }
      }
    }
  }
}
```

- [ ] **A)** A vulnerability in an EC2 instance
- [ ] **B)** A port scan from a known malicious IP
- [ ] **C)** An unauthorized IAM user creation
- [ ] **D)** An S3 bucket policy change

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> The GuardDuty finding indicates a port scan activity from an IP address associated with malicious activity. GuardDuty detects threats like port scans, not vulnerabilities (Inspector) or IAM changes (CloudTrail).
 
 
</details>

### 28. Which AWS service can be used to automatically evaluate whether EC2 instances are configured with a specific security group?

- [ ] **A)** Amazon Inspector
- [ ] **B)** AWS CloudTrail
- [ ] **C)** AWS Config
- [ ] **D)** AWS Artifact

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: C**
 
> 💡  **Explanation** 
> 
> AWS Config records configuration changes and evaluates resources against rules (e.g., required security group). Inspector scans for vulnerabilities, CloudTrail logs API calls, and Artifact provides compliance reports.
 
 
</details>

### 29. Which two statements are true about IAM roles? (Choose two.)

- [ ] **A)** Roles provide long-term access keys.
- [ ] **B)** Roles use temporary credentials from AWS STS.
- [ ] **C)** Roles can be assumed by trusted entities such as AWS services.
- [ ] **D)** Roles are attached directly to IAM users by default.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B, C**
 
> 💡  **Explanation** 
> 
> IAM roles provide temporary credentials via STS and can be assumed by services like EC2, or by users from other accounts. Roles do not have long-term keys and are not attached directly to users; users assume roles.
 
 
</details>

### 30. Examine the service control policy (SCP) JSON. What effect does this SCP have on member accounts?

```json
{
  "Version": "2012-10-17",
  "Statement": [
    {
      "Effect": "Deny",
      "Action": "ec2:RunInstances",
      "Resource": "*",
      "Condition": {
        "StringNotEquals": {
          "aws:RequestedRegion": ["us-east-1", "eu-west-1"]
        }
      }
    }
  ]
}
```

- [ ] **A)** Allows launching EC2 instances only in the specified regions.
- [ ] **B)** Denies the ability to launch EC2 instances outside of us-east-1 and eu-west-1.
- [ ] **C)** Grants permission to use any AWS service.
- [ ] **D)** Prevents creation of IAM roles.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> The SCP uses a Deny effect to block ec2:RunInstances unless the region is us-east-1 or eu-west-1. SCPs set maximum permissions boundaries and cannot grant permissions; they only allow or deny actions.
 
 
</details>
