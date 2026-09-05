<table width="100%">
  <tr>
    <td align="center" valign="middle" width="50%">
      <p align="center"><img src="https://pub-6a9f8dede1194a7786cba69e7dcdad9f.r2.dev/certifications/Microsoft/Microsoft%20Certified-%20Azure%20Network%20Engineer%20Associate.png" width="50%"></p>
    </td>
    <td align="center" valign="middle" width="50%">
      <h1>Microsoft Certified: Azure Network Engineer Associate</h1>
    </td>
  </tr>
</table>

## 📑 Table of Contents

- [Design and implement Azure network security services](#design-and-implement-azure-network-security-services) (6 questions)
- [Design and implement application delivery services](#design-and-implement-application-delivery-services) (5 questions)
- [Design and implement core networking infrastructure](#design-and-implement-core-networking-infrastructure) (7 questions)
- [Design and implement private access to Azure services](#design-and-implement-private-access-to-azure-services) (5 questions)
- [Design, implement, and manage connectivity services](#design-implement-and-manage-connectivity-services) (7 questions)

## 📋 Exam Information

| Field | Value |
|-------|-------|
| Total Questions | 30 |
| Level | Foundation |
| Exported At | 2026-09-04T23:45:11.080Z |
| Domains | 5 |

## 📊 Domain Distribution

| Domain | Questions |
|--------|-----------|
| Design and implement Azure network security services | 6 |
| Design and implement application delivery services | 5 |
| Design and implement core networking infrastructure | 7 |
| Design and implement private access to Azure services | 5 |
| Design, implement, and manage connectivity services | 7 |

---

### **Design and implement Azure network security services**

### 1. What is the function of an Azure CDN profile?

- [ ] **A)** Management container for endpoints
- [ ] **B)** Client-facing URL for content
- [ ] **C)** Caching rule for expiry
- [ ] **D)** Source of truth for content

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> An Azure CDN profile is a management container for one or more endpoints. Endpoints are the client-facing URLs, while the origin is the source of content.
 
 
</details>

### 2. Which options are valid origin types for an Azure CDN? Select all that apply.

- [ ] **A)** Azure Storage account
- [ ] **B)** A Web App
- [ ] **C)** Custom HTTP server
- [ ] **D)** Azure SQL Database

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B, C**
 
> 💡  **Explanation** 
> 
> Azure CDN origins can be an Azure Storage account, a Web App, or a custom HTTP server. A SQL database is not a valid origin for static or dynamic web content delivery.
 
 
</details>

### 3. Based on the Traffic Manager configuration shown, which statement about traffic distribution is correct?

```yaml
routing_method: Weighted
endpoints:
  Endpoint1: { weight: 1 }
  Endpoint2: { weight: 3 }
```

- [ ] **A)** Endpoint2 gets 75%, Endpoint1 gets 25%
- [ ] **B)** Both endpoints get 50% equally
- [ ] **C)** Endpoint1 gets 75%, Endpoint2 gets 25%
- [ ] **D)** Endpoint2 receives all traffic until it fails

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> With weighted routing and weights 1 and 3, Endpoint2 receives 75% of traffic and Endpoint1 receives 25%. Higher weight receives proportionally more traffic.
 
 
</details>

### 4. Which Azure service uses Anycast and the Microsoft global network to accomplish Layer 7 global load balancing?

- [ ] **A)** Azure Front Door
- [ ] **B)** Azure Traffic Manager
- [ ] **C)** Azure Application Gateway
- [ ] **D)** Azure Load Balancer

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Azure Front Door is a global Layer 7 service that uses Anycast and integrates with WAF. Traffic Manager is DNS-based, while Application Gateway and Load Balancer are regional.
 
 
</details>

### 5. Which statements accurately describe Azure Front Door? Select all that apply.

- [ ] **A)** Uses Anycast protocol
- [ ] **B)** Provides Layer 7 load balancing
- [ ] **C)** Integrates with Web Application Firewall
- [ ] **D)** Operates only at the DNS level

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B, C**
 
> 💡  **Explanation** 
> 
> Azure Front Door uses Anycast, performs Layer 7 load balancing, and includes WAF integration. DNS-level operation is a characteristic of Azure Traffic Manager.
 
 
</details>

### 6. A load balancer health probe is configured as shown. What occurs after two consecutive probe failures?

```yaml
probe:
  protocol: HTTP
  path: /health
  interval: 30s
  unhealthy_threshold: 2
```

- [ ] **A)** Backend instance is removed from rotation
- [ ] **B)** Backend virtual machine is restarted
- [ ] **C)** DNS record is switched to another region
- [ ] **D)** Client session cookie is reset

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Health probes determine backend availability. After the unhealthy threshold is reached, the load balancer removes the instance from rotation until it responds successfully again.
 
 
</details>


---

### **Design and implement application delivery services**

### 7. In the Azure CDN resource hierarchy, what is the primary purpose of a CDN profile?

- [ ] **A)** A management container for one or more endpoints.
- [ ] **B)** A URL that serves cached content to clients.
- [ ] **C)** The origin server storing the original content.
- [ ] **D)** A DNS-based routing service for global traffic.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> A profile is a management container for one or more endpoints. Endpoints are the actual URLs clients use to access content.
 
 
</details>

### 8. Which of the following can be configured as an origin type for an Azure CDN endpoint? Select all that apply.

- [ ] **A)** Azure Storage account
- [ ] **B)** Azure Web App
- [ ] **C)** Custom HTTP server
- [ ] **D)** Azure SQL Database

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B, C**
 
> 💡  **Explanation** 
> 
> Azure CDN supports Azure Storage, Web Apps, and custom HTTP servers as origins. SQL Database is not a valid origin for CDN content.
 
 
</details>

### 9. Review the JSON configuration below. What type of origin is defined for this Azure CDN endpoint?

```json
{
  "origin": {
    "host": "myapp.azurewebsites.net",
    "protocol": "HTTPS"
  }
}
```

- [ ] **A)** Azure Storage account
- [ ] **B)** Azure Web App
- [ ] **C)** Custom HTTP server
- [ ] **D)** Apache web server

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> The host myapp.azurewebsites.net indicates an Azure Web App origin because it uses the azurewebsites.net domain.
 
 
</details>

### 10. Which Azure service uses the Anycast protocol and the Microsoft global network to provide Layer 7 load balancing with integrated WAF?

- [ ] **A)** Azure Traffic Manager
- [ ] **B)** Azure Front Door
- [ ] **C)** Azure Load Balancer
- [ ] **D)** Azure Application Gateway

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> Azure Front Door uses Anycast and Microsoft's global network to provide Layer 7 load balancing, SSL offloading, and WAF integration.
 
 
</details>

### 11. Which of the following are valid routing methods for Azure Traffic Manager? Select all that apply.

- [ ] **A)** Performance
- [ ] **B)** Priority
- [ ] **C)** Weighted
- [ ] **D)** Latency

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B, C**
 
> 💡  **Explanation** 
> 
> Traffic Manager supports Performance, Priority, Weighted, and Geographic routing methods. Latency is not a distinct routing method.
 
 
</details>


---

### **Design and implement core networking infrastructure**

### 12. In Azure CDN, what is the main purpose of a CDN profile in the resource hierarchy?

- [ ] **A)** It acts as a management container for endpoints
- [ ] **B)** It stores cached content at edge locations
- [ ] **C)** It is the client-facing URL used to access content
- [ ] **D)** It defines the origin server authentication method

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> A profile is a management container for one or more endpoints, while endpoints are the client-facing URLs.
 
 
</details>

### 13. Which of the following can be configured as an Azure CDN origin? Select all that apply.

- [ ] **A)** Azure Storage account
- [ ] **B)** Azure SQL Database
- [ ] **C)** Azure Web App
- [ ] **D)** Custom HTTP server

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, C, D**
 
> 💡  **Explanation** 
> 
> Azure CDN origins include storage accounts, web apps, and custom HTTP servers; SQL Database is not a CDN origin.
 
 
</details>

### 14. Review the Azure CLI command shown in the code block. What Azure resource does it create?

```bash
az cdn profile create --name prod-cdn-profile --resource-group rg-app --sku Standard_Microsoft
```

- [ ] **A)** CDN endpoint
- [ ] **B)** CDN profile
- [ ] **C)** Front Door profile
- [ ] **D)** Storage account

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> The az cdn profile create command creates an Azure CDN profile, the management container for endpoints.
 
 
</details>

### 15. In Azure CDN caching, what does the TTL setting determine?

- [ ] **A)** The maximum size of files cached at the edge
- [ ] **B)** How long cached content remains valid before being refreshed
- [ ] **C)** The number of purge requests allowed per day
- [ ] **D)** The number of edge nodes that store the content

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> TTL defines how long edge nodes keep cached content before considering it stale, balancing cache hits and freshness.
 
 
</details>

### 16. Which Azure services perform Layer 7 load balancing? Select all that apply.

- [ ] **A)** Azure Application Gateway
- [ ] **B)** Azure Load Balancer
- [ ] **C)** Azure Front Door
- [ ] **D)** Azure Traffic Manager

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, C**
 
> 💡  **Explanation** 
> 
> Application Gateway and Front Door inspect HTTP/HTTPS data; Load Balancer is Layer 4 and Traffic Manager is DNS-based.
 
 
</details>

### 17. A load balancer is configured with the probe shown in the code block. What is the purpose of this probe?

```json
{
  "name": "httpProbe",
  "protocol": "HTTP",
  "port": 8080,
  "intervalInSeconds": 15,
  "numberOfProbes": 2,
  "probeThreshold": 1,
  "requestPath": "/health"
}
```

- [ ] **A)** To assign traffic weights to backend instances
- [ ] **B)** To check whether backend instances are healthy
- [ ] **C)** To cache static content for faster delivery
- [ ] **D)** To terminate TLS connections at the load balancer

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> Health probes send periodic requests to a specified port and path; if the probe fails, the instance is removed from rotation.
 
 
</details>

### 18. Which Azure Traffic Manager routing method selects the endpoint with the lowest latency?

- [ ] **A)** Priority
- [ ] **B)** Weighted
- [ ] **C)** Performance
- [ ] **D)** Geographic

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: C**
 
> 💡  **Explanation** 
> 
> Performance routing sends traffic to the endpoint with the lowest measured latency. Priority focuses on failover, Weighted on capacity.
 
 
</details>


---

### **Design and implement private access to Azure services**

### 19. In Azure Content Delivery Network (CDN), what is the primary role of a CDN profile?

- [ ] **A)** A management container for one or more endpoints
- [ ] **B)** A DNS record used to resolve custom domains
- [ ] **C)** A firewall policy protecting origin servers
- [ ] **D)** A storage solution for static content

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> An Azure CDN profile is a management container that groups one or more endpoints. It provides configuration, billing, and policy settings for all endpoints within it.
 
 
</details>

### 20. Which of the following are valid Azure CDN origin types? (Choose all that apply.)

- [ ] **A)** Azure Storage account
- [ ] **B)** Azure Web App
- [ ] **C)** Custom HTTP server
- [ ] **D)** Azure SQL Database

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B, C**
 
> 💡  **Explanation** 
> 
> Azure CDN supports Azure Storage, Azure Web Apps, and custom HTTP servers as origins. Azure SQL Database is a relational database platform, not a content origin.
 
 
</details>

### 21. A network engineer is reviewing a configuration file for an Azure traffic distribution service. The settings in the code block include HTTP protocol, regional deployment, URL path routing, WAF enablement, and cookie-based affinity. Which Azure service does this configuration represent?

```text
service = 'frontend'
deployment_scope = 'regional'
protocol = 'HTTP'
port = 443
url_path_routing = true
waf_enabled = true
cookie_based_affinity = true
```

- [ ] **A)** Azure Application Gateway
- [ ] **B)** Azure Load Balancer
- [ ] **C)** Azure Traffic Manager
- [ ] **D)** Azure Front Door

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The regional scope, URL path-based routing, WAF protection, and cookie-based affinity are all characteristics of Azure Application Gateway.
 
 
</details>

### 22. What is the purpose of health probes in Azure load balancing?

- [ ] **A)** They check the availability and health of backend instances
- [ ] **B)** They cache static content at edge locations
- [ ] **C)** They select the backend based on client IP address
- [ ] **D)** They encrypt traffic between clients and the backend

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Health probes monitor specific endpoints on backend instances to determine whether they are healthy and should continue receiving traffic.
 
 
</details>

### 23. Which routing methods are available with Azure Traffic Manager? (Select all that apply.)

- [ ] **A)** Performance
- [ ] **B)** Priority
- [ ] **C)** Weighted
- [ ] **D)** Geographic

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B, C, D**
 
> 💡  **Explanation** 
> 
> Azure Traffic Manager supports Performance, Priority, Weighted, and Geographic routing methods for controlling traffic distribution.
 
 
</details>


---

### **Design, implement, and manage connectivity services**

### 24. In Azure CDN, which component serves as the management container for one or more endpoints?

- [ ] **A)** CDN profile
- [ ] **B)** CDN endpoint
- [ ] **C)** Origin server
- [ ] **D)** Point of presence

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> A CDN profile is the management container that groups endpoints. Endpoints are client-facing URLs, and origins provide the actual content.
 
 
</details>

### 25. Which of the following can be configured as an origin in Azure CDN? Select all that apply.

- [ ] **A)** Azure Storage account
- [ ] **B)** Azure Web App
- [ ] **C)** Custom HTTP server
- [ ] **D)** Azure SQL Database

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B, C**
 
> 💡  **Explanation** 
> 
> Azure CDN origins can be Azure Storage accounts, Azure Web Apps, or custom HTTP servers. Azure SQL Database is not a supported content origin.
 
 
</details>

### 26. Review the Azure CLI command in the code block. What does the origin option define for the CDN endpoint?

```bash
az cdn endpoint create
  --profile-name myprofile
  --resource-group myrg
  --name myendpoint
  --origin www.example.com
```

- [ ] **A)** The source server that provides the content
- [ ] **B)** The client-facing CDN endpoint URL
- [ ] **C)** The CDN profile management container
- [ ] **D)** The point-of-presence cache location

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The origin parameter specifies the origin server, which is the source of truth for content that the CDN will cache and deliver.
 
 
</details>

### 27. When a client requests content that is valid and stored at an Azure CDN point of presence, what does the CDN do?

- [ ] **A)** Serves the cached copy directly from the point of presence
- [ ] **B)** Forwards the request to the origin server
- [ ] **C)** Purges the cached content and refetches it
- [ ] **D)** Returns an error to the client

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The CDN serves content from the edge cache when a valid copy exists, avoiding a round-trip to the origin and reducing latency.
 
 
</details>

### 28. From the options listed, which Azure services are designed for global traffic distribution? Select all that apply.

- [ ] **A)** Azure Front Door
- [ ] **B)** Azure Traffic Manager
- [ ] **C)** Azure Application Gateway
- [ ] **D)** Azure Load Balancer

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> Azure Front Door and Traffic Manager are global services. Application Gateway and Load Balancer handle traffic within a single region.
 
 
</details>

### 29. Review the Azure CLI command in the code block. Which Traffic Manager routing method is being configured?

```bash
az network traffic-manager profile create
  --name myprofile
  --resource-group myrg
  --routing-method Performance
```

- [ ] **A)** Performance
- [ ] **B)** Priority
- [ ] **C)** Weighted
- [ ] **D)** Geographic

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The command sets the routing method to Performance, which directs traffic to the endpoint with the lowest latency.
 
 
</details>

### 30. At which layer of the network stack does Azure Traffic Manager make traffic routing decisions?

- [ ] **A)** DNS
- [ ] **B)** Transport (Layer 4)
- [ ] **C)** Application (Layer 7)
- [ ] **D)** Data link (Layer 2)

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Traffic Manager is a DNS-based balancer that returns a healthy endpoint IP address and cannot inspect packets or application headers.
 
 
</details>
