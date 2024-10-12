# AzureSoluationForNextcloud-
In this Guided Project, we will create a Virtual Machine in Azure to deploy a web server, specifically a Nextcloud server. Instead of using just the presets, we will explore how the basic architecture of Azure works, by creating a Virtual Machine, connecting it to a subnet,
In this Guided Project, we will create a Virtual Machine in Azure to deploy a web server, specifically a Nextcloud server. Instead of using just the presets, we will explore how the basic architecture of Azure works, by creating a Virtual Machine, connecting it to a subnet, protected by inbound and outbound rules thanks to Network Security Groups, in a Virtual Network. We'll use Bastion to connect to the machine via SSH, without exposing an external port to the Internet, and then installing a simple Nextcloud server and make the Virtual Machine available by opening a public IP and a DNS label.

Steps We Followed to Build the Solution:
1️⃣ Virtual Machines (VMs):
Deployed multiple VMs (VM1 and VM2) to simulate workloads and applications.
Connected the VMs to public and private IPs for internal and external access.

2️⃣ Application Gateway (AG):
Set up Azure Application Gateway (DEPI-AG) to load balance traffic and secure HTTP/HTTPS communication.
Configured WAF policies to protect against common web attacks like SQL injection.

3️⃣ Network Security Groups (NSG):
Applied NSG (DEPI-NSG) to control inbound and outbound traffic at the network level.
Ensured only authorized traffic could access the VMs and gateway.

4️⃣ Monitoring & Alerts:
Configured metric alerts to track key performance metrics like the total number of requests.
Added activity log alerts to monitor VM restarts and network changes.
Created action groups to notify the operations team in case of incidents.

5️⃣ Azure Bastion:
Deployed Azure Bastion for secure remote access to VMs without exposing RDP/SSH to the internet.

6️⃣ Virtual Network (VNet):
Built a DEPI-VNet to connect all resources securely and provide seamless communication between services.![WhatsApp Image 2024-10-12 at 19 20 52_f14b044f](https://github.com/user-attachments/assets/73ac685e-d12c-4ea1-968f-512ee843b768)
![Uploading WhatsApp Image 2024-10-12 at 19.20.52_f14b044f.jpg…]()
