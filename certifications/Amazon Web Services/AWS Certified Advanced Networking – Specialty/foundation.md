<table width="100%">
  <tr>
    <td align="center" valign="middle" width="50%">
      <p align="center"><img src="https://pub-6a9f8dede1194a7786cba69e7dcdad9f.r2.dev/certifications/Amazon%20Web%20Services%20Training%20and%20Certification/AWS%20Certified%20Advanced%20Networking%20–%20Specialty" width="50%"></p>
    </td>
    <td align="center" valign="middle" width="50%">
      <h1>AWS Certified Advanced Networking – Specialty</h1>
    </td>
  </tr>
</table>

## 📑 Table of Contents

- [Network Automation and Optimization](#network-automation-and-optimization) (3 questions)
- [Network Design](#network-design) (9 questions)
- [Network Implementation](#network-implementation) (8 questions)
- [Network Management and Operations](#network-management-and-operations) (6 questions)
- [Network Security, Compliance, and Governance](#network-security-compliance-and-governance) (4 questions)

## 📋 Exam Information

| Field | Value |
|-------|-------|
| Total Questions | 30 |
| Level | Foundation |
| Exported At | 2026-08-04T06:25:17.992Z |
| Domains | 5 |

## 📊 Domain Distribution

| Domain | Questions |
|--------|-----------|
| Network Automation and Optimization | 3 |
| Network Design | 9 |
| Network Implementation | 8 |
| Network Management and Operations | 6 |
| Network Security, Compliance, and Governance | 4 |

---

### **Network Automation and Optimization**

### 1. Which AWS service provides declarative templates for defining network resources as code?

- [ ] **A)** AWS CloudFormation
- [ ] **B)** AWS Cloud Development Kit (CDK)
- [ ] **C)** AWS OpsWorks
- [ ] **D)** AWS Elastic Beanstalk

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> AWS CloudFormation allows you to model and provision AWS resources using declarative templates. CDK uses programming languages but still synthesizes CloudFormation templates.
 
 
</details>

### 2. Which of the following are benefits of using AWS CloudFormation StackSets for network automation? (Select two.)

- [ ] **A)** Deploy identical network stacks across multiple accounts and regions
- [ ] **B)** Automatically roll back failed deployments without manual intervention
- [ ] **C)** Enable cross-account resource sharing without IAM roles
- [ ] **D)** Provide a single administration account to manage stack instances in target accounts

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, D**
 
> 💡  **Explanation** 
> 
> StackSets allow deploying stacks across multiple accounts and regions from a single admin account. Automatic rollback is not a native feature; it requires custom logic. Cross-account sharing still requires proper IAM roles.
 
 
</details>

### 3. Examine the CloudFormation snippet. Which property change will cause the VPC resource to be replaced?

```yaml
Resources:
  MyVPC:
    Type: AWS::EC2::VPC
    Properties:
      CidrBlock: "10.0.0.0/16"
      EnableDnsSupport: true
      Tags:
        - Key: Name
          Value: ProductionVPC
```

- [ ] **A)** CidrBlock
- [ ] **B)** EnableDnsSupport
- [ ] **C)** Tags
- [ ] **D)** InstanceTenancy

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Changing the CIDR block of a VPC forces replacement. Other properties like EnableDnsSupport or Tags can be updated in-place.
 
 
</details>


---

### **Network Design**

### 4. What describes the statefulness of AWS security groups?

- [ ] **A)** Security groups are stateful, meaning if you allow inbound traffic, the outbound return traffic is automatically allowed.
- [ ] **B)** Security groups are stateless, requiring explicit rules for both inbound and outbound traffic.
- [ ] **C)** Security groups are stateful only for TCP traffic; UDP and ICMP require separate rules.
- [ ] **D)** Security groups are stateless at the subnet level but stateful at the instance level.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Security groups act as a stateful virtual firewall at the instance (ENI) level. When you allow inbound traffic, the outbound return traffic is automatically permitted, regardless of outbound rules. This is a key differentiator from network ACLs, which are stateless and require explicit rules in both directions.
 
 
</details>

### 5. Which two AWS services are managed services that can inspect network traffic for security purposes? (Select two.)

- [ ] **A)** AWS Network Firewall
- [ ] **B)** AWS WAF
- [ ] **C)** Network ACLs
- [ ] **D)** VPC Flow Logs

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> AWS Network Firewall provides stateful intrusion prevention, web filtering, and deep packet inspection across VPCs. AWS WAF is a managed web application firewall that protects against common exploits like SQL injection and XSS. Network ACLs are stateless and not a managed service; VPC Flow Logs capture metadata only, not packet payloads.
 
 
</details>

### 6. Refer to the following network ACL rule configuration. Based on the rules shown, which statement is correct?

```plaintext
Inbound Rules:
  Rule#100: Type: TCP, Port: 80, Source: 0.0.0.0/0, Allow
  Rule#*: Type: All, Source: 0.0.0.0/0, Deny
Outbound Rules:
  Rule#100: Type: TCP, Port: 32768-65535, Destination: 0.0.0.0/0, Allow
  Rule#*: Type: All, Destination: 0.0.0.0/0, Deny
```

- [ ] **A)** The NACL will allow inbound HTTP traffic from any source.
- [ ] **B)** The NACL blocks all inbound ICMP traffic.
- [ ] **C)** The NACL is stateful and automatically allows return traffic.
- [ ] **D)** The NACL evaluates rules in numeric order and denies all traffic by default.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The NACL has an inbound rule with rule number 100 that allows TCP traffic on port 80 from any source (0.0.0.0/0). Rules are evaluated in order; if a rule matches, it is applied. Since the default rule ( * ) denies all traffic, any traffic not explicitly allowed is denied. The NACL is stateless, so return traffic must be explicitly allowed. ICMP is not allowed by any rule, but the statement about blocking is not necessarily true because there is no explicit deny – it would be denied by the default rule. The question asks which statement is correct: only the first option is directly supported by the rule shown.
 
 
</details>

### 7. What is the primary purpose of a VPC Gateway Endpoint?

- [ ] **A)** To provide private connectivity to AWS services without traversing the public internet.
- [ ] **B)** To enable internet access for instances in a private subnet.
- [ ] **C)** To peer two VPCs together in the same region.
- [ ] **D)** To create a VPN connection to an on-premises network.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> A VPC Gateway Endpoint (e.g., for S3 or DynamoDB) allows instances in a VPC to communicate with the service over the AWS network without requiring a public IP, NAT device, or internet gateway. This improves security and reduces data transfer costs because traffic stays within the AWS backbone.
 
 
</details>

### 8. Which two PCI DSS requirements directly relate to network security controls in AWS? (Select two.)

- [ ] **A)** Requirement 1 – Install and maintain a firewall configuration.
- [ ] **B)** Requirement 4 – Encrypt cardholder data over public networks.
- [ ] **C)** Requirement 2 – Do not use default passwords.
- [ ] **D)** Requirement 8 – Identify and authenticate users.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> Requirement 1 mandates a firewall (e.g., AWS Network Firewall, security groups) to protect cardholder data. Requirement 4 requires encryption of cardholder data transmitted over open/public networks, which can be met using TLS, VPN, or Direct Connect with MACsec. Requirements 2 and 8 deal with password management and access control, not directly network security.
 
 
</details>

### 9. Examine this security group rule snippet. Based on the configuration, which incoming traffic is allowed?

```yaml
Security Group: sg-12345678
Inbound Rules:
  - Protocol: TCP, Port: 22, Source: 203.0.113.0/24
  - Protocol: TCP, Port: 80, Source: 0.0.0.0/0
```

- [ ] **A)** Only inbound SSH (port 22) from any source.
- [ ] **B)** Inbound SSH (port 22) from 203.0.113.0/24 and inbound HTTP (port 80) from any source.
- [ ] **C)** Only inbound HTTP (port 80) from any source.
- [ ] **D)** Inbound SSH (port 22) from any source and inbound HTTP (port 80) from any source.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> The security group has two inbound rules: one allows TCP port 22 from the CIDR 203.0.113.0/24, and another allows TCP port 80 from 0.0.0.0/0. Therefore, SSH is restricted to the specific IP range, while HTTP is open to the internet. The other options improperly open SSH to all or omit one of the allowed ports.
 
 
</details>

### 10. Which AWS service provides centralized stateful inspection across VPCs using Suricata-compatible rules?

- [ ] **A)** AWS Network Firewall
- [ ] **B)** AWS WAF
- [ ] **C)** Security Groups
- [ ] **D)** AWS Shield Advanced

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> AWS Network Firewall is a managed service that provides stateful inspection, intrusion prevention, and web filtering using Suricata-compatible rules. It can be centrally managed and deployed across VPCs. AWS WAF works at the application layer on load balancers, not at the network layer. Security groups are stateful but applied per ENI, not centralized. AWS Shield Advanced is for DDoS protection.
 
 
</details>

### 11. Which two options can be used for hybrid connectivity between an on-premises data center and AWS? (Select two.)

- [ ] **A)** AWS Direct Connect
- [ ] **B)** Site-to-Site VPN
- [ ] **C)** VPC Peering
- [ ] **D)** AWS PrivateLink

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> AWS Direct Connect provides a dedicated, private network connection from on-premises to AWS. Site-to-Site VPN creates an encrypted tunnel over the public internet. VPC Peering connects VPCs, not on-premises networks. AWS PrivateLink exposes services within the same AWS network, not for hybrid connectivity.
 
 
</details>

### 12. Refer to the Route 53 health check configuration. What is the default evaluation interval for the health check?

```plaintext
Health Check ID: abc123
Type: HTTP
Interval: 30
Failure Threshold: 3
Resource: ALB endpoint
```

- [ ] **A)** 10 seconds
- [ ] **B)** 30 seconds
- [ ] **C)** 60 seconds
- [ ] **D)** 5 minutes

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> By default, Route 53 health checks run every 30 seconds. You can configure a fast interval of 10 seconds at an additional cost. The health check type shown is HTTP, and the default interval is 30 seconds.
 
 
</details>


---

### **Network Implementation**

### 13. Which AWS service provides a dedicated physical connection between on-premises and AWS?

- [ ] **A)** AWS Site-to-Site VPN
- [ ] **B)** AWS Direct Connect
- [ ] **C)** AWS Transit Gateway
- [ ] **D)** AWS Client VPN

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> Direct Connect provides a dedicated physical connection, bypassing the internet for consistent performance.
 
 
</details>

### 14. Which two features are characteristics of AWS Security Groups?

- [ ] **A)** Stateful filtering
- [ ] **B)** Stateless filtering
- [ ] **C)** Applied at subnet level
- [ ] **D)** Allow rules only

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, D**
 
> 💡  **Explanation** 
> 
> Security Groups are stateful and only support allow rules; they operate at the ENI level.
 
 
</details>

### 15. Examine the CloudFormation snippet. What does the 'SourceSecurityGroupId' reference achieve?

```yaml
WebSecurityGroup:
  Type: AWS::EC2::SecurityGroup
  Properties:
    GroupDescription: Allow HTTP from ALB
    SecurityGroupIngress:
      - IpProtocol: tcp
        FromPort: 80
        ToPort: 80
        SourceSecurityGroupId: !GetAtt ALBSecurityGroup.GroupId
```

- [ ] **A)** It allows traffic from any instance in the referenced security group
- [ ] **B)** It denies traffic from that security group
- [ ] **C)** It allows traffic from a specific IP range
- [ ] **D)** It sets the rule to apply only to the subnet

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Referencing a security group as a source decouples rules from IPs, simplifying management.
 
 
</details>

### 16. Which routing protocol is required for AWS Direct Connect private virtual interfaces?

- [ ] **A)** OSPF
- [ ] **B)** BGP
- [ ] **C)** EIGRP
- [ ] **D)** Static routing

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> AWS Direct Connect private virtual interfaces require BGP for dynamic routing.
 
 
</details>

### 17. Which two services can be used to automate AWS network resource deployment?

- [ ] **A)** AWS CloudFormation
- [ ] **B)** AWS CDK
- [ ] **C)** AWS OpsWorks
- [ ] **D)** AWS Elastic Beanstalk

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> CloudFormation and CDK are IaC services; OpsWorks and Elastic Beanstalk are not primarily for networking.
 
 
</details>

### 18. Examine the BGP configuration snippet. What does the 'neighbor 169.254.10.1 remote-as 64512' command do?

```cisco-ios
router bgp 65001
 neighbor 169.254.10.1 remote-as 64512
 neighbor 169.254.10.1 activate
 network 10.0.0.0 mask 255.255.0.0
```

- [ ] **A)** It establishes a BGP session with the AWS peer on that IP
- [ ] **B)** It defines the local router's AS number as 64512
- [ ] **C)** It creates a static route to the VPC
- [ ] **D)** It enables OSPF routing

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> This command establishes a BGP session with the AWS side using the assigned link-local address.
 
 
</details>

### 19. What is the default MTU for an AWS Site-to-Site VPN tunnel?

- [ ] **A)** 1500
- [ ] **B)** 9001
- [ ] **C)** 4470
- [ ] **D)** 1460

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> VPN tunnels use standard Ethernet MTU 1500 due to IPsec overhead; jumbo frames are not supported.
 
 
</details>

### 20. Which two AWS services provide DDoS protection?

- [ ] **A)** AWS Shield Standard
- [ ] **B)** AWS Shield Advanced
- [ ] **C)** AWS WAF
- [ ] **D)** AWS Network Firewall

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> Shield Standard and Advanced are DDoS protection services; WAF is a web application firewall.
 
 
</details>


---

### **Network Management and Operations**

### 21. Which of the following fields is captured by VPC Flow Logs?

- [ ] **A)** srcaddr
- [ ] **B)** packet payload
- [ ] **C)** HTTP method
- [ ] **D)** SSL certificate

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> VPC Flow Logs capture metadata fields such as source IP address (srcaddr), not payload or application-layer details.
 
 
</details>

### 22. Which two AWS services can be used to implement Infrastructure as Code for network resources?

- [ ] **A)** AWS CloudFormation
- [ ] **B)** Terraform with AWS provider
- [ ] **C)** AWS OpsWorks
- [ ] **D)** AWS CodeDeploy

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> CloudFormation and Terraform are IaC tools used to define and provision network resources in a repeatable manner.
 
 
</details>

### 23. Based on the CloudFormation template snippet, what resource type is being created?

```yaml
AWSTemplateFormatVersion: '2010-09-09'
Resources:
  MyVPC:
    Type: AWS::EC2::VPC
    Properties:
      CidrBlock: 10.0.0.0/16
```

- [ ] **A)** VPC
- [ ] **B)** Subnet
- [ ] **C)** Internet Gateway
- [ ] **D)** Route Table

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The snippet defines an AWS::EC2::VPC resource with a CIDR block, indicating a VPC creation.
 
 
</details>

### 24. What is the default quota for VPC peering connections per VPC?

- [ ] **A)** 50
- [ ] **B)** 125
- [ ] **C)** 100
- [ ] **D)** 250

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> Each VPC is limited to 125 peering connections by default, as noted in the AWS documentation.
 
 
</details>

### 25. Which two destinations can VPC Flow Logs be published to?

- [ ] **A)** Amazon CloudWatch Logs
- [ ] **B)** Amazon S3
- [ ] **C)** Amazon Kinesis Data Firehose
- [ ] **D)** Amazon DynamoDB

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> VPC Flow Logs can be sent to either CloudWatch Logs or S3; other destinations are not directly supported.
 
 
</details>

### 26. What is the AWS CLI command doing?

```bash
aws ec2 create-flow-logs --resource-type VPC --resource-id vpc-12345678 --traffic-type ALL --log-destination-type cloud-watch-logs --log-group-name my-flow-logs --iam-role-arn arn:aws:iam::123456789012:role/FlowLogsRole
```

- [ ] **A)** Enabling VPC Flow Logs
- [ ] **B)** Creating a new VPC
- [ ] **C)** Modifying a security group
- [ ] **D)** Deleting a flow log

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The 'create-flow-logs' command enables flow logs for a VPC, sending all traffic metadata to CloudWatch Logs.
 
 
</details>


---

### **Network Security, Compliance, and Governance**

### 27. Which statement best describes the statefulness of an AWS Security Group?

- [ ] **A)** Return traffic is automatically allowed for permitted inbound flows.
- [ ] **B)** Return traffic must be explicitly allowed in outbound rules.
- [ ] **C)** All traffic is allowed by default.
- [ ] **D)** Rules are evaluated in order until a match is found.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Security Groups are stateful: return traffic for allowed inbound flows is automatically permitted, regardless of outbound rules.
 
 
</details>

### 28. Which of the following are characteristics of an AWS Network ACL? (Select two)

- [ ] **A)** Stateless: return traffic must be explicitly allowed.
- [ ] **B)** Supports both allow and deny rules.
- [ ] **C)** Stateful: return traffic is automatically allowed.
- [ ] **D)** Rules are evaluated all together before decision.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> Network ACLs are stateless, support allow/deny rules, and are evaluated in ascending order until a match is found.
 
 
</details>

### 29. Refer to the VPC Flow Log entry below. What does the 'REJECT' field indicate?

```text
2 123456789010 eni-1235b8ca123456789 10.0.1.5 10.0.2.5 443 54864 6 10 5000 1620140761 1620140821 REJECT OK
```

- [ ] **A)** The traffic was allowed.
- [ ] **B)** The traffic was blocked.
- [ ] **C)** The traffic was inspected by Network Firewall.
- [ ] **D)** The traffic was encrypted.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> The REJECT action indicates that the traffic was denied by a security group or network ACL rule.
 
 
</details>

### 30. At which OSI layer does AWS WAF operate?

- [ ] **A)** Layer 7 (Application)
- [ ] **B)** Layer 4 (Transport)
- [ ] **C)** Layer 3 (Network)
- [ ] **D)** Layer 2 (Data Link)

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> AWS WAF is a web application firewall that operates at Layer 7 to protect against application-layer attacks.
 
 
</details>
