<table width="100%">
  <tr>
    <td align="center" valign="middle" width="50%">
      <p align="center"><img src="https://pub-6a9f8dede1194a7786cba69e7dcdad9f.r2.dev/certifications/Google%20Cloud/Professional%20Cloud%20Network%20Engineer.png" width="50%"></p>
    </td>
    <td align="center" valign="middle" width="50%">
      <h1>Professional Cloud Network Engineer</h1>
    </td>
  </tr>
</table>

## 📑 Table of Contents

- [Configuring network services](#configuring-network-services) (6 questions)
- [Designing and planning a VPC network](#designing-and-planning-a-vpc-network) (7 questions)
- [Hybrid connectivity](#hybrid-connectivity) (6 questions)
- [Implementing a VPC network](#implementing-a-vpc-network) (5 questions)
- [Managing network operations](#managing-network-operations) (6 questions)

## 📋 Exam Information

| Field | Value |
|-------|-------|
| Total Questions | 30 |
| Level | Foundation |
| Exported At | 2026-09-04T23:44:48.018Z |
| Domains | 5 |

## 📊 Domain Distribution

| Domain | Questions |
|--------|-----------|
| Configuring network services | 6 |
| Designing and planning a VPC network | 7 |
| Hybrid connectivity | 6 |
| Implementing a VPC network | 5 |
| Managing network operations | 6 |

---

### **Configuring network services**

### 1. Which Google Cloud connectivity solution requires physical presence in a colocation facility and supports 10 Gbps or 100 Gbps circuits?

- [ ] **A)** Dedicated Interconnect
- [ ] **B)** Partner Interconnect
- [ ] **C)** Cloud VPN
- [ ] **D)** DNS Peering

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Dedicated Interconnect requires a physical presence in a Google colocation facility and offers 10 Gbps or 100 Gbps circuits. Partner Interconnect uses a service provider and lower bandwidth increments.
 
 
</details>

### 2. Which components are mandatory for an Interconnect deployment? (Select all that apply.)

- [ ] **A)** Cloud Router for BGP sessions
- [ ] **B)** VLAN attachments
- [ ] **C)** Static routes without BGP
- [ ] **D)** Cloud VPN tunnel on the same link

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> Interconnect requires Cloud Router for BGP dynamic routing and VLAN attachments to connect VPCs to the physical link. Static routing is not supported, and Cloud VPN is a different connectivity option.
 
 
</details>

### 3. Refer to the gcloud command. What resource is being created?

```bash
gcloud compute interconnects attachments create prod-attachment \
    --region=us-central1 \
    --router=core-router \
    --interconnect=prod-interconnect \
    --vlan-tag=101
```

- [ ] **A)** VLAN attachment for Dedicated Interconnect
- [ ] **B)** Cloud Router BGP session
- [ ] **C)** Partner Interconnect connection
- [ ] **D)** Cloud VPN tunnel

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The command creates a VLAN attachment for a Dedicated Interconnect by specifying the interconnect resource, router, region, and VLAN tag.
 
 
</details>

### 4. To meet the 99.99% SLA for Dedicated Interconnect, what architecture is required?

- [ ] **A)** Two connections in one metro area
- [ ] **B)** Redundant connections across two distinct edge availability domains
- [ ] **C)** A single Dedicated Interconnect circuit with BGP
- [ ] **D)** One Dedicated Interconnect plus one Partner Interconnect in same metro

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> To achieve 99.99% SLA, Google requires redundant connections across two distinct edge availability domains, or metropolitan areas. 99.9% may be achieved within a single metro area.
 
 
</details>

### 5. Which statements about Cloud DNS inbound and outbound policies are true? (Select all that apply.)

- [ ] **A)** Inbound DNS policy allows on-premises clients to resolve Google Cloud private DNS zones.
- [ ] **B)** Outbound DNS policy forwards VPC queries for specific domains to external DNS servers.
- [ ] **C)** Inbound and outbound policies can operate without VPN or Interconnect connectivity.
- [ ] **D)** DNS Peering can replace a forwarding rule to reach on-premises servers.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> Inbound DNS policy lets on-premises clients resolve private zones, while outbound DNS policy forwards VPC queries to external DNS servers. Both require underlying VPN or Interconnect connectivity to reach the proxy IPs.
 
 
</details>

### 6. Refer to the gcloud command. What type of DNS zone is being created?

```bash
gcloud dns managed-zones create corp-private \
    --visibility=private \
    --dns-name=corp.internal. \
    --description=Private_DNS_zone \
    --networks=my-vpc
```

- [ ] **A)** Cloud DNS private zone visible only to authorized VPC networks.
- [ ] **B)** Public DNS zone
- [ ] **C)** DNS peering zone
- [ ] **D)** Outbound forwarding zone

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> A private DNS zone is created with --visibility=private and is only visible to authorized VPC networks. It is not a public zone, peering zone, or forwarding zone.
 
 
</details>


---

### **Designing and planning a VPC network**

### 7. Which Cloud Interconnect option requires a direct physical connection in a Google colocation facility?

- [ ] **A)** Dedicated Interconnect
- [ ] **B)** Partner Interconnect
- [ ] **C)** Cloud VPN
- [ ] **D)** Cloud NAT

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Dedicated Interconnect requires a physical presence in a Google colocation facility and provides a direct physical connection to Google's edge network.
 
 
</details>

### 8. Which two components are required for Cloud Interconnect and HA VPN to dynamically exchange routes with on-premises networks?

- [ ] **A)** Cloud Router
- [ ] **B)** BGP
- [ ] **C)** Static routing protocol
- [ ] **D)** Cloud DNS

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> Cloud Interconnect and HA VPN require Cloud Router and BGP for dynamic route exchange; static routes are not supported.
 
 
</details>

### 9. In the code block, what type of logical interface is being defined?

```hcl
resource "google_compute_interconnect_attachment" "prod" {
  name = "prod-attachment"
  router = google_compute_router.router.id
  type = "DEDICATED"
}
```

- [ ] **A)** VLAN Attachment
- [ ] **B)** Cloud Router
- [ ] **C)** Dedicated Interconnect circuit
- [ ] **D)** Cloud DNS private zone

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The code block creates a VLAN attachment, which is the logical interface used to connect a VPC to an interconnect.
 
 
</details>

### 10. According to Google Cloud HA guidance, what SLA is supported by two connections located within one metro area?

- [ ] **A)** 99.9%
- [ ] **B)** 99.99%
- [ ] **C)** 99.95%
- [ ] **D)** 100%

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Two connections in one metro area provide a 99.9% SLA; 99.99% requires redundancy across two distinct edge availability domains.
 
 
</details>

### 11. Which statements accurately describe Dedicated Interconnect? (Select all that apply.)

- [ ] **A)** Requires physical presence in a Google colocation facility
- [ ] **B)** Supports 10 Gbps or 100 Gbps circuits
- [ ] **C)** Uses Cloud Router and BGP for routing
- [ ] **D)** Offers bandwidth increments from 50 Mbps to 50 Gbps

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B, C**
 
> 💡  **Explanation** 
> 
> Dedicated Interconnect requires a colocation presence, supports 10/100 Gbps circuits, and uses Cloud Router/BGP. Lower bandwidth increments are a Partner Interconnect characteristic.
 
 
</details>

### 12. What type of DNS resource is being configured in the code block?

```hcl
resource "google_dns_managed_zone" "private_zone" {
  name     = "private-example"
  dns_name = "corp.internal."
  visibility = "private"

  private_visibility_config {
    networks {
      network_url = google_compute_network.vpc.id
    }
  }
}
```

- [ ] **A)** Cloud DNS Private Zone
- [ ] **B)** Inbound DNS policy
- [ ] **C)** Outbound DNS policy
- [ ] **D)** DNS Peering

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The snippet creates a Cloud DNS private zone, which is visible only to authorized VPC networks and used for internal service discovery.
 
 
</details>

### 13. What is the purpose of Cloud DNS forwarding zones?

- [ ] **A)** Redirect queries for a specific domain to an inbound or outbound IP address
- [ ] **B)** Replace Cloud Interconnect for hybrid connectivity
- [ ] **C)** Encrypt DNS traffic over the public internet
- [ ] **D)** Establish a BGP session between VPCs

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Cloud DNS forwarding zones redirect queries for a specified domain to an inbound or outbound IP address, enabling hybrid DNS resolution.
 
 
</details>


---

### **Hybrid connectivity**

### 14. Which type of Interconnect requires a physical presence in a Google colocation facility and provides 10 Gbps or 100 Gbps circuits?

- [ ] **A)** Dedicated Interconnect
- [ ] **B)** Partner Interconnect
- [ ] **C)** Cloud VPN
- [ ] **D)** Cloud DNS Peering

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Dedicated Interconnect is the direct physical connection housed in Google colocation facilities, supporting 10 Gbps or 100 Gbps circuits.
 
 
</details>

### 15. Which statements about Interconnect high-availability requirements are correct?

- [ ] **A)** Two connections within one metro area can support a 99.9% SLA.
- [ ] **B)** A single Dedicated Interconnect circuit is enough for a 99.99% SLA.
- [ ] **C)** 99.99% SLA requires redundant connections across two distinct edge availability domains.
- [ ] **D)** Cloud VPN over the internet provides the same predictable performance as Interconnect.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, C**
 
> 💡  **Explanation** 
> 
> For 99.9%, two links in one metro suffice; for 99.99%, redundancy must span two metropolitan areas. Single circuits are single points of failure.
 
 
</details>

### 16. Review the configuration snippet. What must be configured on the Cloud Router to enable dynamic route exchange for this VLAN attachment?

```hcl
resource "google_compute_interconnect_attachment" "example" {
  name         = "example-attachment"
  interconnect = "dedicated-interconnect"
  router       = "cloud-router-example"
  region       = "us-central1"
  type         = "DEDICATED"
}
```

- [ ] **A)** Configure a BGP session with the on-premises peer
- [ ] **B)** Deploy Cloud NAT
- [ ] **C)** Create a DNS peering zone
- [ ] **D)** Add a static default route to Google

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Cloud Router uses BGP to exchange routes. Without a BGP session, the VLAN attachment cannot dynamically route traffic between on-premises and VPC.
 
 
</details>

### 17. Which service is appropriate for an organization that cannot place equipment in a Google colocation facility and needs a 200 Mbps connection?

- [ ] **A)** Partner Interconnect
- [ ] **B)** Dedicated Interconnect
- [ ] **C)** Cloud VPN
- [ ] **D)** DNS Peering

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Partner Interconnect is delivered through supported providers and supports 50 Mbps to 50 Gbps, so it suits 200 Mbps requirements without colocation equipment.
 
 
</details>

### 18. Which statements about Cloud DNS inbound/outbound policies and DNS peering are correct?

- [ ] **A)** Inbound DNS policy lets on-premises clients resolve Google Cloud private DNS zones.
- [ ] **B)** Outbound DNS policy forwards queries for specified domains to external DNS servers.
- [ ] **C)** DNS policies will work even without VPN or Interconnect connectivity.
- [ ] **D)** DNS peering natively bridges a VPC to an on-premises network.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> Inbound answers on-premises queries for private zones; outbound forwards VPC queries to external servers. Both require underlying connectivity, and peering connects VPCs, not on-premises.
 
 
</details>

### 19. Review the outbound DNS forwarding configuration. Where will VPC resources send matching domain queries?

```yaml
name: "outbound-policy"
networks:
- network: "projects/proj/global/networks/vpc-a"
forwarding:
- targetNameServers:
  - address: "10.0.0.5"
    forwardingPath: "private"
  - address: "10.0.0.6"
    forwardingPath: "private"
```

- [ ] **A)** The on-premises DNS servers at 10.0.0.5 and 10.0.0.6
- [ ] **B)** Google Public DNS at 8.8.8.8
- [ ] **C)** Cloud DNS private zone records
- [ ] **D)** VPC peering networks

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> An outbound forwarding policy sends matching queries to the listed on-premises DNS server addresses, allowing VPC resources to resolve internal hostnames.
 
 
</details>


---

### **Implementing a VPC network**

### 20. In hybrid cloud networking, which statement correctly defines Dedicated Interconnect and its primary characteristics?

- [ ] **A)** Direct physical connection at a Google colocation facility
- [ ] **B)** Encrypted tunnel over the public internet
- [ ] **C)** Service provider bridges on-premises to Google Cloud
- [ ] **D)** Logical interface connecting VPC to an interconnect

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Dedicated Interconnect is a direct physical link in a Google colocation facility, designed for high-bandwidth, predictable hybrid connectivity.
 
 
</details>

### 21. Which elements are required to achieve a 99.99% availability SLA for an Interconnect deployment? Choose all that apply.

- [ ] **A)** Cloud VPN as primary transport for high throughput
- [ ] **B)** Redundant connections in two distinct metro areas
- [ ] **C)** One Dedicated Interconnect circuit in one metro
- [ ] **D)** BGP sessions managed by Cloud Router

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B, D**
 
> 💡  **Explanation** 
> 
> A 99.99% SLA requires redundant connections across two distinct edge availability domains; Cloud Router/BGP is required for dynamic routing. A single circuit or VPN does not meet this SLA.
 
 
</details>

### 22. In the gcloud command shown, what is the function of the flag that references the Cloud Router resource?

```bash
gcloud compute interconnects attachments dedicated create my-attachment --region=us-central1 --router=my-router --interconnect=my-interconnect --vlan-tag=100
```

- [ ] **A)** Specifies the on-premises router
- [ ] **B)** Selects the VPC network
- [ ] **C)** Identifies the Cloud Router managing BGP sessions
- [ ] **D)** Enables static routing instead of BGP

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: C**
 
> 💡  **Explanation** 
> 
> The router flag names the Cloud Router that manages BGP sessions for the VLAN attachment, enabling route exchange between on-premises and VPC.
 
 
</details>

### 23. A company has no presence in a Google colocation facility and needs 200 Mbps of interconnect bandwidth. Which connection type should it choose?

- [ ] **A)** Dedicated Interconnect
- [ ] **B)** Partner Interconnect
- [ ] **C)** Cloud VPN
- [ ] **D)** DNS Peering

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> Partner Interconnect uses a service provider and supports lower bandwidth increments, making it ideal for organizations without a colocation location.
 
 
</details>

### 24. Which statements correctly describe Cloud DNS inbound and outbound policies in a hybrid cloud? Select all that apply.

- [ ] **A)** Inbound forwards VPC queries to on-prem DNS servers
- [ ] **B)** Outbound forwards VPC queries to on-prem DNS servers
- [ ] **C)** Both policies require VPN or Interconnect connectivity
- [ ] **D)** Inbound lets on-prem clients resolve private zones

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B, C, D**
 
> 💡  **Explanation** 
> 
> Inbound policies allow on-premises clients to query private zones; outbound policies forward VPC domain queries to on-prem DNS. Both depend on VPN or Interconnect connectivity.
 
 
</details>


---

### **Managing network operations**

### 25. What is a fundamental requirement for establishing a Dedicated Interconnect connection?

- [ ] **A)** A supported service provider
- [ ] **B)** A physical presence in a Google colocation facility
- [ ] **C)** A public internet connection
- [ ] **D)** A Cloud VPN tunnel

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> Dedicated Interconnect provides a direct physical connection and requires a physical presence in a Google colocation facility, unlike Partner Interconnect which uses a service provider.
 
 
</details>

### 26. Which statements about Interconnect high availability architectures are correct? (Choose all that apply.)

- [ ] **A)** Two connections in one metro area are enough for a 99.9% SLA.
- [ ] **B)** A 99.99% SLA requires redundant connections across two distinct edge availability domains.
- [ ] **C)** A single Dedicated Interconnect circuit provides high availability.
- [ ] **D)** A 99.9% SLA is always achieved with a single connection.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> For 99.9% SLA, two connections in one metro area are required; for 99.99%, redundant connections must span two distinct edge availability domains. A single circuit is a single point of failure.
 
 
</details>

### 27. The configuration snippet defines a Cloud Router resource. What routing protocol does it enable for Interconnect?

```hcl
resource "google_compute_router" "router" {
  name    = "cloud-router"
  network = "vpc-network"
  bgp {
    asn            = 65001
    advertise_mode = "CUSTOM"
  }
}
```

- [ ] **A)** BGP
- [ ] **B)** OSPF
- [ ] **C)** IS-IS
- [ ] **D)** EIGRP

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Interconnect relies on Border Gateway Protocol (BGP) for dynamic routing; Cloud Router manages BGP sessions.
 
 
</details>

### 28. What is a VLAN attachment in the context of Cloud Interconnect?

- [ ] **A)** A logical interface that maps a VPC to the Interconnect
- [ ] **B)** A physical cable in the colocation facility
- [ ] **C)** A VPN gateway in Google Cloud
- [ ] **D)** A DNS forwarding rule

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> A VLAN attachment is the logical interface used to connect your VPC to the Interconnect; for Dedicated Interconnect, it maps to a VLAN ID on the physical link.
 
 
</details>

### 29. Which statements about Partner Interconnect are accurate? (Choose all that apply.)

- [ ] **A)** It uses a supported service provider to connect to Google Cloud.
- [ ] **B)** It is ideal for organizations without a presence in a Google colocation facility.
- [ ] **C)** It requires a physical presence in a Google colocation facility.
- [ ] **D)** It supports bandwidth increments from 50 Mbps to 50 Gbps.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B, D**
 
> 💡  **Explanation** 
> 
> Partner Interconnect uses a supported service provider, is suited for environments without a Google colocation presence, and supports lower bandwidth increments; Dedicated Interconnect requires colocation presence.
 
 
</details>

### 30. Review the DNS zone configuration in the code block. What type of zone is being created?

```hcl
resource "google_dns_managed_zone" "private_zone" {
  name        = "private-zone"
  dns_name    = "corp.internal."
  visibility  = "private"
  private_visibility_config {
    networks {
      network_url = "vpc-network"
    }
  }
}
```

- [ ] **A)** Cloud DNS Private Zone
- [ ] **B)** Public DNS zone
- [ ] **C)** DNS peering zone
- [ ] **D)** Forwarding zone

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The configuration creates a private DNS zone visible only to authorized VPC networks, used for internal service discovery.
 
 
</details>
