<table width="100%">
  <tr>
    <td align="center" valign="middle" width="50%">
      <p align="center"><img src="https://pub-6a9f8dede1194a7786cba69e7dcdad9f.r2.dev/certifications/Amazon%20Web%20Services%20Training%20and%20Certification/AWS%20Certified%20DevOps%20Engineer%20–%20Professional" width="50%"></p>
    </td>
    <td align="center" valign="middle" width="50%">
      <h1>AWS Certified DevOps Engineer – Professional</h1>
    </td>
  </tr>
</table>

## 📑 Table of Contents

- [Configuration Management and Infrastructure as Code](#configuration-management-and-infrastructure-as-code) (6 questions)
- [High Availability, Fault Tolerance, and Disaster Recovery](#high-availability-fault-tolerance-and-disaster-recovery) (3 questions)
- [Incident and Event Response](#incident-and-event-response) (5 questions)
- [Monitoring and Logging](#monitoring-and-logging) (5 questions)
- [Policies and Standards Automation](#policies-and-standards-automation) (4 questions)
- [SDLC Automation](#sdlc-automation) (7 questions)

## 📋 Exam Information

| Field | Value |
|-------|-------|
| Total Questions | 30 |
| Level | Foundation |
| Exported At | 2026-08-04T06:25:28.692Z |
| Domains | 6 |

## 📊 Domain Distribution

| Domain | Questions |
|--------|-----------|
| Configuration Management and Infrastructure as Code | 6 |
| High Availability, Fault Tolerance, and Disaster Recovery | 3 |
| Incident and Event Response | 5 |
| Monitoring and Logging | 5 |
| Policies and Standards Automation | 4 |
| SDLC Automation | 7 |

---

### **Configuration Management and Infrastructure as Code**

### 1. What is the primary function of AWS Systems Manager State Manager?

- [ ] **A)** Enforce desired configuration on managed instances on a schedule
- [ ] **B)** Provide a continuous audit trail of resource configurations
- [ ] **C)** Scan for security vulnerabilities in EC2 instances
- [ ] **D)** Ad-hoc command execution on EC2 instances

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> State Manager is a Systems Manager capability that enforces a desired state configuration on instances using associations. It runs on a schedule to proactively prevent drift. AWS Config provides continuous audit trail, not State Manager.
 
 
</details>

### 2. Which of the following are valid features of AWS Config? (Select TWO.)

- [ ] **A)** Continuous evaluation of resource configurations against rules
- [ ] **B)** Automatic remediation of non-compliant resources by default
- [ ] **C)** Recording a configuration timeline for each supported resource
- [ ] **D)** Proactive enforcement of desired state on EC2 instances

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, C**
 
> 💡  **Explanation** 
> 
> AWS Config performs continuous evaluation of resource configurations against rules and maintains a configuration timeline. It does not automatically remediate by default; remediation requires additional automation. Proactive enforcement is done by State Manager.
 
 
</details>

### 3. Review the following CloudFormation snippet. Which resource property is used to prevent accidental updates to the stack?

```yaml
Resources:
  MyEC2Instance:
    Type: AWS::EC2::Instance
    Properties:
      InstanceType: t2.micro
      ImageId: ami-0abcdef1234567890
    DeletionPolicy: Retain

```

- [ ] **A)** DisableRollback
- [ ] **B)** StackPolicy
- [ ] **C)** EnableTerminationProtection
- [ ] **D)** DeletionPolicy

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: C**
 
> 💡  **Explanation** 
> 
> EnableTerminationProtection is a stack-level attribute that prevents accidental stack deletion. DisableRollback only prevents rollback on failure. StackPolicy controls update permissions to resources, not deletion. DeletionPolicy defines what happens when a resource is deleted.
 
 
</details>

### 4. What is the purpose of a conformance pack in AWS Config?

- [ ] **A)** Deploy a collection of Config rules and remediation actions as a single entity
- [ ] **B)** Store template definitions for EC2 Image Builder pipelines
- [ ] **C)** Manage state file locking for Terraform deployments
- [ ] **D)** Automatically rotate database credentials

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> A conformance pack is a collection of AWS Config rules and remediation actions that can be deployed as a single entity across accounts or OUs. It helps enforce compliance frameworks like CIS AWS Foundations Benchmark.
 
 
</details>

### 5. Which of the following are capabilities of AWS Systems Manager Patch Manager? (Select TWO.)

- [ ] **A)** Automating the process of patching managed nodes
- [ ] **B)** Providing continuous compliance evaluation of running instances
- [ ] **C)** Using patch baselines to define approved and rejected patches
- [ ] **D)** Enforcing a desired state configuration on instances

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, C**
 
> 💡  **Explanation** 
> 
> Patch Manager automates patching using patch baselines. Continuous compliance evaluation is done by AWS Config, not Patch Manager. Enforcing desired state is the role of State Manager.
 
 
</details>

### 6. Examine the following Terraform configuration snippet. What is the purpose of the 'backend' block?

```hcl
terraform {
  backend "s3" {
    bucket = "my-company-terraform-state"
    key    = "prod/network/terraform.tfstate"
    region = "us-east-1"
    dynamodb_table = "terraform-state-lock"
  }
}

```

- [ ] **A)** Define the provider used to create resources
- [ ] **B)** Specify where Terraform stores its state data
- [ ] **C)** Configure authentication with cloud providers
- [ ] **D)** Set variable values for the infrastructure

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> The backend block configures where Terraform stores its state file, including optional state locking. In this example, it uses an S3 bucket with DynamoDB for locking.
 
 
</details>


---

### **High Availability, Fault Tolerance, and Disaster Recovery**

### 7. What is the primary purpose of a multi-AZ architecture in AWS?

- [ ] **A)** Failure of a single data center within a region
- [ ] **B)** Failure of an entire AWS region
- [ ] **C)** Failure of an individual EC2 instance
- [ ] **D)** Failure of a single load balancer

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Multi-AZ protects against the failure of a single Availability Zone, not a full region.
 
 
</details>

### 8. Which two of the following are Route 53 routing policies that can be used for high availability?

- [ ] **A)** Failover routing
- [ ] **B)** Simple routing
- [ ] **C)** Weighted routing
- [ ] **D)** Latency-based routing

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, C**
 
> 💡  **Explanation** 
> 
> Failover and Weighted routing policies support health checks to exclude unhealthy endpoints.
 
 
</details>

### 9. Based on the CloudFormation snippet below, what is the consequence of setting the FailureThreshold to 3?

```json
{
  "Type": "AWS::Route53::HealthCheck",
  "Properties": {
    "HealthCheckConfig": {
      "FullyQualifiedDomainName": "example.com",
      "Port": 443,
      "Type": "HTTPS",
      "RequestInterval": 10,
      "FailureThreshold": 3
    }
  }
}
```

- [ ] **A)** 3 consecutive failures
- [ ] **B)** 10 consecutive failures
- [ ] **C)** The number of failures required is not specified
- [ ] **D)** The health check will never be marked unhealthy

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The FailureThreshold parameter defines the number of consecutive failures before marking unhealthy.
 
 
</details>


---

### **Incident and Event Response**

### 10. Which AWS service acts as the central event bus for handling operational events and routing them to Lambda functions?

- [ ] **A)** Amazon EventBridge
- [ ] **B)** Amazon SNS
- [ ] **C)** Amazon CloudWatch
- [ ] **D)** AWS Config

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Amazon EventBridge is the central event bus that ingests events from AWS services and routes them to targets like Lambda functions.
 
 
</details>

### 11. Which features of Amazon EventBridge are critical for incident response automation? (Select two.)

- [ ] **A)** Built-in retry policy and dead-letter queue
- [ ] **B)** Supports complex JSON event pattern matching
- [ ] **C)** Provides manual approval workflows
- [ ] **D)** Automatically deduplicates all events

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> EventBridge offers built-in retry/DLQ and advanced JSON pattern matching, essential for robust incident automation.
 
 
</details>

### 12. Review the EventBridge rule pattern below. Choose the option that correctly matches an EC2 instance stop event.

```json
{
  "source": ["aws.ec2"],
  "detail-type": ["EC2 Instance State-change Notification"],
  "detail": {
    "state": ["stopped"]
  }
}
```

- [ ] **A)** Source: aws.ec2, DetailType: EC2 Instance State-change Notification, Detail: state = stopped
- [ ] **B)** Source: aws.ec2, DetailType: EC2 Instance State-change Notification, Detail: state = running
- [ ] **C)** Source: aws.ec2, DetailType: EC2 Instance Stop, Detail: state = stopped
- [ ] **D)** Source: aws.ec2, DetailType: AWS API Call via CloudTrail, Detail: eventName = StopInstances

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The correct pattern targets the EC2 instance state-change detail-type with state equal to stopped.
 
 
</details>

### 13. What is the main function of an Auto Scaling lifecycle hook?

- [ ] **A)** Run custom actions before instance transitions
- [ ] **B)** Terminate unhealthy instances immediately
- [ ] **C)** Define scaling policies based on metrics
- [ ] **D)** Monitor CPU utilization of instances

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Lifecycle hooks pause instance launch or termination to run custom actions like software installation or deregistration.
 
 
</details>

### 14. Which two AWS services can be combined to create self-healing mechanisms?

- [ ] **A)** AWS Config Auto-Remediation
- [ ] **B)** AWS Systems Manager Automation
- [ ] **C)** Amazon Route 53
- [ ] **D)** AWS Shield

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> AWS Config Auto-Remediation and Systems Manager Automation are core services for implementing automated self-healing.
 
 
</details>


---

### **Monitoring and Logging**

### 15. What is the primary purpose of a CloudWatch Logs subscription filter?

- [ ] **A)** Transform log data before storage
- [ ] **B)** Filter logs for retention policy enforcement
- [ ] **C)** Route log events in real-time to destinations like Kinesis or Lambda
- [ ] **D)** Encrypt log data at rest

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: C**
 
> 💡  **Explanation** 
> 
> Subscription filters are used to stream log data from CloudWatch Logs to other AWS services in near real-time, enabling centralized processing and analysis.
 
 
</details>

### 16. Which of the following are valid destinations for a CloudWatch Logs subscription filter? (Select two.)

- [ ] **A)** Amazon S3
- [ ] **B)** AWS Lambda
- [ ] **C)** Amazon DynamoDB
- [ ] **D)** Amazon Kinesis Data Streams

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B, D**
 
> 💡  **Explanation** 
> 
> CloudWatch Logs subscription filters can deliver logs to Lambda, Kinesis Data Streams, Kinesis Data Firehose, and Amazon OpenSearch Service. S3 and DynamoDB are not direct destinations.
 
 
</details>

### 17. Examine the provided ECS task definition snippet. Which component is being deployed as a sidecar container to forward trace data to AWS X-Ray?

```json
{
  "containerDefinitions": [
    {
      "name": "xray-daemon",
      "image": "amazon/aws-xray-daemon",
      "portMappings": [{"containerPort": 2000, "protocol": "udp"}]
    },
    {
      "name": "my-app",
      "image": "my-app:latest"
    }
  ]
}
```

- [ ] **A)** X-Ray Daemon
- [ ] **B)** X-Ray SDK
- [ ] **C)** X-Ray Sampling Rule
- [ ] **D)** X-Ray API

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The X-Ray Daemon must run as a sidecar on ECS (or on EC2) to receive segment data from the application and send it to the X-Ray service.
 
 
</details>

### 18. What is the default buffer size for Amazon Kinesis Data Firehose before delivering data to its destination?

- [ ] **A)** 1 MB or 10 seconds
- [ ] **B)** 5 MB or 60 seconds
- [ ] **C)** 128 MB or 900 seconds
- [ ] **D)** 256 MB or 300 seconds

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> The default buffering hint for Kinesis Data Firehose is 5 MB or 60 seconds. The larger limits (128 MB or 900 seconds) are configurable maximums.
 
 
</details>

### 19. Which of the following are true about AWS X-Ray annotations? (Select two.)

- [ ] **A)** Annotations are key-value pairs that are indexed for search.
- [ ] **B)** Annotations are non-indexed and can be arbitrary JSON.
- [ ] **C)** Annotations can be used to filter traces in the X-Ray console.
- [ ] **D)** Annotations are automatically added by AWS services without code changes.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, C**
 
> 💡  **Explanation** 
> 
> Annotations are indexed and searchable, allowing you to filter traces. Metadata is non-indexed. Annotations require explicit code instrumentation.
 
 
</details>


---

### **Policies and Standards Automation**

### 20. What is the primary purpose of AWS Config managed rules?

- [ ] **A)** Replace IAM policies
- [ ] **B)** Evaluate resource configurations for compliance
- [ ] **C)** Automatically create AWS resources
- [ ] **D)** Monitor network traffic patterns

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> Managed rules are pre-built templates that continuously evaluate AWS resources against compliance standards like CIS or HIPAA.
 
 
</details>

### 21. Which two AWS services can automatically remediate non-compliant IAM resources?

- [ ] **A)** AWS Systems Manager Automation
- [ ] **B)** AWS Lambda
- [ ] **C)** Amazon Simple Notification Service
- [ ] **D)** AWS CloudTrail

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> SSM Automation documents and custom Lambda functions are common patterns to automatically remediate non-compliant resources.
 
 
</details>

### 22. Which condition key in an IAM policy enforces a required tag at resource creation?

```json
{
  "Effect": "Deny",
  "Action": "ec2:RunInstances",
  "Condition": {
    "Null": {
      "aws:RequestTag/Environment": "true"
    }
  }
}
```

- [ ] **A)** aws:RequestTag
- [ ] **B)** aws:ResourceTag
- [ ] **C)** aws:TagKeys
- [ ] **D)** ec2:TagSpecification

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The aws:RequestTag condition key checks for tags in the API request to enforce tagging at creation.
 
 
</details>

### 23. What is the effect of a Service Control Policy with an explicit Deny on an action?

- [ ] **A)** Action is allowed if IAM policy allows
- [ ] **B)** Action is denied regardless of IAM permissions
- [ ] **C)** Action is allowed only for the root user
- [ ] **D)** Action is denied but resource-based policies can override

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> An explicit Deny in an SCP always overrides any Allow in IAM policies, making the action unavailable.
 
 
</details>


---

### **SDLC Automation**

### 24. Which AWS service is primarily used for automated deployment of application code to EC2 instances?

- [ ] **A)** AWS CodeBuild
- [ ] **B)** AWS CodeDeploy
- [ ] **C)** AWS CodePipeline
- [ ] **D)** AWS CodeCommit

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> AWS CodeDeploy is the managed service that automates code deployments to EC2, Lambda, and ECS. CodeBuild handles building and testing, CodePipeline orchestrates the pipeline, and CodeCommit is a source control service.
 
 
</details>

### 25. Which of the following are valid artifact repository services on AWS? (Choose two.)

- [ ] **A)** Amazon S3
- [ ] **B)** Amazon DynamoDB
- [ ] **C)** AWS CodeArtifact
- [ ] **D)** Amazon RDS

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, C**
 
> 💡  **Explanation** 
> 
> S3 is widely used for storing generic build artifacts, and CodeArtifact is a managed service for package dependencies. DynamoDB and RDS are databases, not artifact stores.
 
 
</details>

### 26. Examine the following CloudFormation template snippet. Which intrinsic function should replace the placeholder to retrieve the VPC ID from another stack?

```yaml
Resources:
  MyInstance:
    Type: AWS::EC2::Instance
    Properties:
      SubnetId: !Ref Subnet
      VpcId: !ImportValue SharedVpcId
```

- [ ] **A)** Fn::GetAtt
- [ ] **B)** Fn::ImportValue
- [ ] **C)** Ref
- [ ] **D)** Fn::Select

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> Fn::ImportValue is used to import values exported from other stacks using the Export field. Fn::GetAtt gets attributes of resources in the same stack, Ref returns the physical ID, and Fn::Select selects from a list.
 
 
</details>

### 27. What does the 'CodeGuru Reviewer' service primarily analyze?

- [ ] **A)** Runtime performance
- [ ] **B)** Static code quality and security vulnerabilities
- [ ] **C)** Infrastructure configuration
- [ ] **D)** Network traffic patterns

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> CodeGuru Reviewer is a static analysis tool that identifies code defects, security vulnerabilities, and best practice violations. CodeGuru Profiler handles runtime performance.
 
 
</details>

### 28. Which of the following are valid trigger mechanisms for AWS CodePipeline? (Choose two.)

- [ ] **A)** Amazon CloudWatch Events (EventBridge)
- [ ] **B)** AWS Lambda function invocation
- [ ] **C)** GitHub webhooks via CodeStar Connections
- [ ] **D)** Amazon SQS queue messages

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, C**
 
> 💡  **Explanation** 
> 
> CodePipeline can be triggered by CloudWatch Events (e.g., CodeCommit state changes) and by webhooks from GitHub, Bitbucket, or GitLab via CodeStar Connections. Lambda is a possible action within a pipeline, not a trigger. SQS is not a native trigger for CodePipeline.
 
 
</details>

### 29. Review the following CodeDeploy lifecycle hook configuration. Which hook is missing to run a validation script after traffic is shifted to the new environment?

```yaml
version: 0.0
os: linux
files:
  - source: /
    destination: /var/www/html
hooks:
  AfterInstall:
    - location: scripts/validate.sh
      timeout: 300
```

- [ ] **A)** BeforeInstall
- [ ] **B)** AfterInstall
- [ ] **C)** AfterAllowTraffic
- [ ] **D)** BeforeAllowTraffic

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: C**
 
> 💡  **Explanation** 
> 
> AfterAllowTraffic runs after the new environment receives traffic. BeforeInstall runs before installation, AfterInstall after installation, and BeforeAllowTraffic before shifting traffic.
 
 
</details>

### 30. Which AWS service is used to manage package dependencies (such as npm, Maven, PyPI) within a CI/CD pipeline?

- [ ] **A)** Amazon S3
- [ ] **B)** AWS CodeArtifact
- [ ] **C)** Amazon ECR
- [ ] **D)** AWS Systems Manager

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> AWS CodeArtifact is a fully managed artifact repository service that works with popular package managers (npm, Maven, PyPI, NuGet, etc.). S3 is for generic binary artifacts, ECR for container images, and Systems Manager for operational data.
 
 
</details>
