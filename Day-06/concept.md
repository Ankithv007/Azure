# Azure Networking Advanced

## Azure App Gateway & WAF

Azure Application Gateway is a web traffic load balancer that enables you to manage and route traffic to your web applications. Web Application Firewall (WAF) provides protection against web vulnerabilities. Key features include:

---
Azure Application Gateway is like a traffic officer for web applications. It manages and routes incoming web traffic to your backend servers based on predefined rules.


- Key Features:

- Load Balancing: Distributes incoming traffic across multiple servers to ensure no single server is overwhelmed, similar to how a traffic officer redirects vehicles to avoid congestion on a single road.
- SSL Termination: Offloads SSL decryption to enhance the efficiency of web servers, like how a toll booth collects tolls so drivers don’t need to stop again elsewhere.
- Web Application Firewall (WAF): Protects web applications from vulnerabilities and exploits, acting like a security checkpoint to block suspicious activity.

### Azure Load Balancer
Azure Load Balancer acts as a traffic director for network traffic. It ensures that your applications remain available by distributing traffic across multiple servers.

- Key Features:
- Load Balancing Algorithms: Uses strategies like round-robin or least connections to distribute traffic effectively, like assigning customers to the least busy cashier in a supermarket.
- Availability Sets: Works with Azure's availability sets to maintain high availability for your applications.
- Inbound and Outbound Traffic: Balances traffic coming into and going out of your servers, similar to how a bridge controls the flow of vehicles entering and exiting a city.

### Azure DNS
Azure DNS is like a phone directory for the Internet. It maps domain names (like www.example.com) to IP addresses, allowing users to find your services easily.

- Key Features:
- Domain Hosting: Hosts and resolves domain names within Azure's infrastructure, ensuring reliability.
- Integration with Azure Services: Seamlessly connects with services like App Service and Traffic Manager.
- Global Availability: Ensures low-latency responses worldwide, much like having multiple directory offices in different locations to serve local users faster.

### Azure Firewall
Azure Firewall is your digital security guard, monitoring and filtering traffic to protect your virtual network.

- Key Features:
- Stateful Firewall: Tracks traffic sessions to allow or deny based on defined rules, much like a building security system that tracks who enters and exits.
- Application FQDN Filtering: Filters traffic by fully qualified domain names, like blocking or allowing visitors based on specific ID cards.
- Threat Intelligence Integration: Enhances security by integrating with threat intelligence feeds, akin to a guard who is constantly updated on potential threats.

### Virtual Network Peering and VNet Gateway
- Virtual Network Peering
Virtual Network Peering is like building a private bridge between two islands (Virtual Networks). It enables resources in one network to communicate directly with resources in another, bypassing the need for public internet.

- Key Features:
- Global VNet Peering: Connects VNets across different regions, like international bridges between countries.
- Transitive Routing: Ensures traffic between peered VNets flows directly, improving performance, similar to a shortcut road connecting two locations.


### VNet Gateway
VNet Gateway acts as a secure entry and exit point for communication between Azure and on-premises networks or remote clients.

- Key Features:
- Site-to-Site VPN: Creates an encrypted VPN tunnel between your office network and Azure, similar to a private tunnel under a river connecting two offices.
- Point-to-Site VPN: Allows individual devices to connect securely to Azure resources, like providing employees with keycards to access the office remotely.


### VPN Gateway
Azure VPN Gateway is like a dedicated courier service that securely delivers packages (data) between locations (on-premises and Azure).

- Key Features:
- IPsec/IKE VPN Protocols: Uses secure communication protocols to protect data during transit, akin to sealed, tamper-proof containers.
- High Availability: Supports active-active and active-passive configurations, ensuring constant service, like having backup couriers ready if the main courier is unavailable.
- BGP Support: Enables dynamic routing between networks, like GPS systems that find the best route in real-time for efficient deliveries.







