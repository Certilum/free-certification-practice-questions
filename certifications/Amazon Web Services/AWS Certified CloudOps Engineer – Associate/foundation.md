<table width="100%">
  <tr>
    <td align="center" valign="middle" width="50%">
      <p align="center"><img src="https://pub-6a9f8dede1194a7786cba69e7dcdad9f.r2.dev/certifications/Amazon%20Web%20Services%20Training%20and%20Certification/AWS%20Certified%20DevOps%20Engineer%20%E2%80%93%20Professional" width="50%"></p>
    </td>
    <td align="center" valign="middle" width="50%">
      <h1>AWS Certified CloudOps Engineer – Associate</h1>
    </td>
  </tr>
</table>

## 📑 Table of Contents

- [Cost and Performance Optimization](#cost-and-performance-optimization) (4 questions)
- [Deployment, Provisioning, and Automation](#deployment-provisioning-and-automation) (5 questions)
- [Monitoring, Logging, and Remediation](#monitoring-logging-and-remediation) (6 questions)
- [Networking and Content Delivery](#networking-and-content-delivery) (5 questions)
- [Reliability and Business Continuity](#reliability-and-business-continuity) (5 questions)
- [Security and Compliance](#security-and-compliance) (5 questions)

## 📋 Exam Information

| Field | Value |
|-------|-------|
| Total Questions | 30 |
| Level | Foundation |
| Exported At | 2026-08-04T06:25:23.263Z |
| Domains | 6 |

## 📊 Domain Distribution

| Domain | Questions |
|--------|-----------|
| Cost and Performance Optimization | 4 |
| Deployment, Provisioning, and Automation | 5 |
| Monitoring, Logging, and Remediation | 6 |
| Networking and Content Delivery | 5 |
| Reliability and Business Continuity | 5 |
| Security and Compliance | 5 |

---

### **Cost and Performance Optimization**

### 1. What is the typical data latency for AWS Cost Explorer when viewing current day costs?

- [ ] **A)** Up to 1 hour
- [ ] **B)** Up to 12 hours
- [ ] **C)** Up to 24 hours
- [ ] **D)** Near real-time (under 5 minutes)

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: C**
 
> 💡  **Explanation** 
> 
> Cost Explorer data is collected and reported with a latency of up to 24 hours for the current day. Real-time billing data is available via CloudWatch billing metrics.
 
 
</details>

### 2. Which two of the following are valid AWS Budgets types? (Choose two.)

- [ ] **A)** Cost Budget
- [ ] **B)** Reservation Budget
- [ ] **C)** Security Budget
- [ ] **D)** Performance Budget

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> AWS Budgets supports three types: Cost budgets (against total cost), Usage budgets (against resource usage), and Reservation budgets (for RI/Savings Plans utilization or coverage). Security and Performance are not budget types.
 
 
</details>

### 3. The following Python code is part of a Lambda function that runs periodically. What is the primary purpose of this code?

```python
import boto3
ec2 = boto3.client('ec2')
def lambda_handler(event, context):
    instances = ec2.describe_instances(Filters=[{'Name':'tag-key','Values':['AutoStop']}])
    stop_ids = []
    for reservation in instances['Reservations']:
        for instance in reservation['Instances']:
            tags = {t['Key']: t['Value'] for t in instance.get('Tags', [])}
            if tags.get('AutoStop') != 'No':
                stop_ids.append(instance['InstanceId'])
    if stop_ids:
        ec2.stop_instances(InstanceIds=stop_ids)
```

- [ ] **A)** It stops EC2 instances that are not tagged with 'AutoStop:No'.
- [ ] **B)** It terminates EC2 instances that are older than 7 days.
- [ ] **C)** It creates a backup of EC2 instances.
- [ ] **D)** It restarts EC2 instances that have low CPU utilization.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The code filters EC2 instances by tag 'AutoStop:No' (inverted check) and then calls the stop_instances API. It is a simple stop operation for instances that are not excluded.
 
 
</details>

### 4. Before AWS Budgets can filter costs by a cost allocation tag, where must the tag be activated?

- [ ] **A)** AWS Config
- [ ] **B)** Billing and Cost Management console
- [ ] **C)** AWS Organizations console
- [ ] **D)** Amazon EC2 console

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> Cost allocation tags must be activated in the Billing and Cost Management console. Simply tagging resources is not enough; activation is required for cost tracking tools like Budgets and Cost Explorer.
 
 
</details>


---

### **Deployment, Provisioning, and Automation**

### 5. What is the primary purpose of AWS CloudFormation?

- [ ] **A)** Deploy applications as a PaaS
- [ ] **B)** Declaratively provision AWS resources
- [ ] **C)** Monitor EC2 instance health
- [ ] **D)** Automate code building and testing

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> CloudFormation is a declarative infrastructure-as-code service to provision AWS resources in an orderly, repeatable manner.
 
 
</details>

### 6. Which two features are components of an AWS CloudFormation template?

- [ ] **A)** Resources
- [ ] **B)** Outputs
- [ ] **C)** Parameters
- [ ] **D)** AWSTemplateFormatVersion

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, D**
 
> 💡  **Explanation** 
> 
> Every CloudFormation template must include AWSTemplateFormatVersion and Resources. Outputs and Parameters are optional.
 
 
</details>

### 7. Based on the code snippet, what is the CloudFormation resource type?

```yaml
Resources:
  MyEC2Instance:
    Type: 'AWS::EC2::Instance'
    Properties:
      ImageId: ami-0abcdef123
      InstanceType: t3.micro
```

- [ ] **A)** AWS::EC2::SecurityGroup
- [ ] **B)** AWS::EC2::Instance
- [ ] **C)** AWS::IAM::Role
- [ ] **D)** AWS::S3::Bucket

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> The snippet defines an EC2 instance with specified properties like ImageId and InstanceType.
 
 
</details>

### 8. What is the function of a change set in CloudFormation?

- [ ] **A)** Execute stack updates immediately
- [ ] **B)** Preview modifications before applying them
- [ ] **C)** Roll back a failed stack update
- [ ] **D)** Delete a stack and its resources

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> A change set provides a preview of the changes CloudFormation will make, allowing review before execution.
 
 
</details>

### 9. Which two deployment policies are supported by AWS Elastic Beanstalk?

- [ ] **A)** Rolling
- [ ] **B)** Blue/Green
- [ ] **C)** All at Once
- [ ] **D)** Canary

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> Elastic Beanstalk supports Rolling, Immutable, Blue/Green, Rolling with Additional Batch, and All at Once.
 
 
</details>


---

### **Monitoring, Logging, and Remediation**

### 10. Which AWS service records API activity in an AWS account for auditing?

- [ ] **A)** Amazon CloudWatch
- [ ] **B)** AWS CloudTrail
- [ ] **C)** AWS Config
- [ ] **D)** AWS Systems Manager

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> AWS CloudTrail records API activity in your account, providing auditing and security analysis. CloudWatch monitors metrics, Config evaluates configurations, and Systems Manager manages operations.
 
 
</details>

### 11. Which two actions can a CloudWatch alarm trigger directly? (Choose two.)

- [ ] **A)** Send a message to an SNS topic
- [ ] **B)** Invoke a Lambda function directly
- [ ] **C)** Execute an SSM Automation document
- [ ] **D)** Trigger an Auto Scaling policy

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, D**
 
> 💡  **Explanation** 
> 
> CloudWatch alarms can directly trigger SNS notifications and Auto Scaling policies. Lambda invocation requires SNS as intermediary; SSM Automation is not a direct alarm action.
 
 
</details>

### 12. Examine the following CloudWatch alarm configuration snippet. What action will this alarm perform when it transitions to ALARM state?

```json
{
  "AlarmName": "HighCPUAlarm",
  "AlarmActions": ["arn:aws:sns:us-east-1:123456789012:MyTopic"],
  "MetricName": "CPUUtilization",
  "Threshold": 80.0
}
```

- [ ] **A)** It sends a notification to an SNS topic.
- [ ] **B)** It terminates the EC2 instance.
- [ ] **C)** It starts an SSM Automation document.
- [ ] **D)** It triggers a Lambda function.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The alarm configuration includes an AlarmActions array with an SNS topic ARN, meaning it sends a notification when the alarm is in ALARM state.
 
 
</details>

### 13. Which component does AWS Config use to automatically fix non-compliant resources?

- [ ] **A)** CloudWatch Alarm
- [ ] **B)** SSM Automation document
- [ ] **C)** SNS Topic
- [ ] **D)** Lambda function directly

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> AWS Config automatic remediation uses SSM Automation documents (or Lambda) to fix non‑compliant resources. CloudWatch alarms detect metric breaches; SNS is for notifications.
 
 
</details>

### 14. Which three tools can a CloudOps engineer use to analyze performance bottlenecks? (Choose three.)

- [ ] **A)** CloudWatch Logs Insights
- [ ] **B)** AWS X-Ray
- [ ] **C)** AWS CloudTrail
- [ ] **D)** VPC Flow Logs

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B, D**
 
> 💡  **Explanation** 
> 
> CloudWatch Logs Insights queries logs, X-Ray traces requests across services, and VPC Flow Logs analyze network performance. CloudTrail records API calls, not performance.
 
 
</details>

### 15. The following CloudWatch Logs Insights query processes application log data. What does it calculate?

```sql
fields @timestamp, @duration
| filter @message like /ERROR/
| stats pct(@duration, 99) by @timestamp
```

- [ ] **A)** Average request latency
- [ ] **B)** 99th percentile request latency
- [ ] **C)** Total number of requests
- [ ] **D)** Maximum request size

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> The query uses `stats pct(@duration, 99)` which calculates the 99th percentile of the duration field, indicating the latency experienced by the slowest 1% of requests.
 
 
</details>


---

### **Networking and Content Delivery**

### 16. What characteristic of a VPC CIDR block cannot be modified after creation?

- [ ] **A)** Size
- [ ] **B)** Range
- [ ] **C)** Subnet mask
- [ ] **D)** IP version

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> The CIDR block range (e.g., 10.0.0.0/16) cannot be changed after VPC creation; only the range is immutable.
 
 
</details>

### 17. Which two statements correctly describe differences between security groups and network ACLs?

- [ ] **A)** Security groups are stateful
- [ ] **B)** NACLs are stateful
- [ ] **C)** NACLs support deny rules
- [ ] **D)** Security groups support deny rules

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, C**
 
> 💡  **Explanation** 
> 
> Security groups are stateful and only allow rules; NACLs are stateless and support both allow and deny rules.
 
 
</details>

### 18. Review the NACL configuration. Why are inbound HTTP responses being dropped?

```plaintext
Inbound NACL rules:
  100 ALLOW TCP 80 0.0.0.0/0
  200 ALLOW TCP 443 0.0.0.0/0
Outbound NACL rules:
  100 ALLOW TCP 80 0.0.0.0/0
  200 ALLOW TCP 443 0.0.0.0/0
```

- [ ] **A)** Missing outbound rule for ephemeral ports
- [ ] **B)** Inbound rule for HTTPS is missing
- [ ] **C)** Security group blocks outbound traffic
- [ ] **D)** NACL inbound rule priority is too low

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> NACLs are stateless; return traffic uses ephemeral ports, which must be explicitly allowed in outbound rules.
 
 
</details>

### 19. Which Virtual Interface type is used to access S3 over Direct Connect without traversing the internet?

- [ ] **A)** Private VIF
- [ ] **B)** Public VIF
- [ ] **C)** Transit VIF
- [ ] **D)** BGP VIF

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> A public VIF provides access to AWS public services (S3, DynamoDB) over Direct Connect without internet.
 
 
</details>

### 20. Which two are benefits of using Amazon CloudFront for content delivery?

- [ ] **A)** Reduced latency for global users
- [ ] **B)** Automatic encryption of data at rest
- [ ] **C)** Lower origin load through caching
- [ ] **D)** Eliminates need for security groups

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, C**
 
> 💡  **Explanation** 
> 
> CloudFront caches content at edge locations, reducing latency and offloading origin infrastructure.
 
 
</details>


---

### **Reliability and Business Continuity**

### 21. Which AWS service automatically distributes incoming application traffic across multiple targets to improve fault tolerance?

- [ ] **A)** Auto Scaling
- [ ] **B)** Elastic Load Balancing
- [ ] **C)** AWS Global Accelerator
- [ ] **D)** Route 53

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> Elastic Load Balancing distributes traffic and performs health checks, improving fault tolerance.
 
 
</details>

### 22. Which of the following are characteristics of Amazon RDS Multi-AZ deployments? (Select two.)

- [ ] **A)** The standby can serve read traffic.
- [ ] **B)** Synchronous replication to a standby in a different Availability Zone.
- [ ] **C)** Automatic failover in the event of a failure.
- [ ] **D)** Standby is in a different region.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B, C**
 
> 💡  **Explanation** 
> 
> Multi-AZ provides synchronous replication and automatic failover; the standby does not serve reads and is in the same region.
 
 
</details>

### 23. Consider the Auto Scaling group configuration in the code block. When an EC2 instance fails its ELB health check, what action does the Auto Scaling group take?

```yaml
AutoScalingGroup:
  HealthCheckType: ELB
  HealthCheckGracePeriod: 300
  TargetGroupARNs: arn:aws:elasticloadbalancing:us-east-1:123456789012:targetgroup/my-tg/1234567890abcdef
```

- [ ] **A)** The instance is immediately terminated by ELB.
- [ ] **B)** The ASG will consider the instance unhealthy and replace it.
- [ ] **C)** The instance remains running unless EC2 status check fails.
- [ ] **D)** The ELB automatically adds a new instance.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> If the ASG has ELB health checks enabled, it will mark the instance unhealthy and launch a replacement.
 
 
</details>

### 24. What is the primary purpose of enabling cross-zone load balancing on an Application Load Balancer?

- [ ] **A)** To distribute traffic across all registered targets in all enabled Availability Zones
- [ ] **B)** To keep traffic within a single Availability Zone
- [ ] **C)** To enable sticky sessions
- [ ] **D)** To reduce latency by using the nearest zone

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Cross-zone load balancing distributes traffic evenly across all targets in all enabled AZs.
 
 
</details>

### 25. Which of the following are valid scaling policy types for Auto Scaling groups? (Select two.)

- [ ] **A)** Target Tracking
- [ ] **B)** Scheduled Scaling
- [ ] **C)** Step Scaling
- [ ] **D)** Simple Scaling

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, C**
 
> 💡  **Explanation** 
> 
> Target Tracking and Step Scaling are dynamic scaling policies; Simple and Scheduled are also types but the question asks for two of the dynamic ones.
 
 
</details>


---

### **Security and Compliance**

### 26. What is the principle of least privilege in AWS IAM?

- [ ] **A)** Give every user full administrative access to all services.
- [ ] **B)** Grant only the minimum permissions necessary for a task.
- [ ] **C)** Grant permissions based on the user's job title.
- [ ] **D)** Allow all actions but deny specific risky actions.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> Least privilege means granting only the minimum permissions needed to perform a function, reducing risk.
 
 
</details>

### 27. Which of the following are capabilities of IAM Access Analyzer? (Select two.)

- [ ] **A)** Identifies resources shared with external principals
- [ ] **B)** Generates policy suggestions based on actual usage
- [ ] **C)** Automatically rotates IAM user access keys
- [ ] **D)** Blocks all public access to S3 buckets

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> IAM Access Analyzer finds externally shared resources and can generate refined policies from CloudTrail logs.
 
 
</details>

### 28. Review the diagram showing encryption options for S3. Which option uses customer-provided keys?

```markdown
| Feature | SSE-S3 | SSE-KMS | SSE-C |
|---------|--------|---------|-------|
| Key management | AWS managed | Customer managed | Customer provides key each request |
| Key rotation | Automatic | Automatic or manual | Customer rotates externally |
| Audit trail | Limited | Full | None |
```

- [ ] **A)** SSE-S3
- [ ] **B)** SSE-KMS
- [ ] **C)** SSE-C
- [ ] **D)** Client-Side Encryption

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: C**
 
> 💡  **Explanation** 
> 
> SSE-C requires the customer to provide the encryption key with each request; S3 does not store the key.
 
 
</details>

### 29. What data sources does Amazon GuardDuty analyze for threat detection?

- [ ] **A)** VPC Flow Logs, CloudTrail, and DNS logs
- [ ] **B)** Only CloudTrail management events
- [ ] **C)** Only VPC Flow Logs
- [ ] **D)** AWS Config configuration history

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> GuardDuty analyzes VPC Flow Logs, CloudTrail events, and DNS logs for malicious activity.
 
 
</details>

### 30. Which services can send findings to AWS Security Hub? (Select two.)

- [ ] **A)** Amazon GuardDuty
- [ ] **B)** AWS Config
- [ ] **C)** Amazon Route 53
- [ ] **D)** AWS CloudFormation

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> Security Hub ingests findings from GuardDuty and AWS Config, among other services.
 
 
</details>
