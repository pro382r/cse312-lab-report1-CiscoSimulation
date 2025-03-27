# DNS, SMTP, and FTP Server Configuration with Cisco

This project demonstrates the configuration of essential network services - DNS (Domain Name System), SMTP (Simple Mail Transfer Protocol), and FTP (File Transfer Protocol) - within a simulated network environment using Cisco networking devices.

## Overview

The goal of this project was to configure and verify the basic functionality of DNS, SMTP, and FTP servers within a network consisting of two local area networks (LANs) connected by a router. This setup simulates a common network architecture where different departments or sections might reside on separate subnets.

The key components configured include:

* **DNS Server:** Responsible for translating hostnames to IP addresses, enabling user-friendly access to services.
* **SMTP Server:** Facilitates the sending and receiving of emails within the network.
* **FTP Server:** Allows for the transfer of files between devices on the network.

This project utilizes Cisco networking concepts and commands, likely implemented using a network simulation tool like Cisco Packet Tracer or GNS3.

## Network Topology

The network topology consists of two distinct LANs (LAN 1 and LAN 2) interconnected via a Cisco router. Each LAN includes end devices (PCs and laptops) and dedicated servers for DNS, SMTP, and FTP.

* **LAN 1 (Network: 192.10.10.1/24):**
    * DNS Server: 192.10.10.6
    * SMTP Server: 192.10.10.5
    * FTP Server: 192.10.10.4
    * PCs: 192.10.10.3, 192.10.10.2

* **LAN 2 (Network: 192.10.11.1/24):**
    * DNS Server: 192.10.11.6
    * SMTP Server: 192.10.11.5
    * FTP Server: 192.10.11.4
    * PCs: 192.10.11.2
    * Laptop: 192.10.11.3
* **Router:** Connects LAN 1 and LAN 2, enabling inter-VLAN communication.

## Implementation Details

This section outlines the steps taken to configure the DNS, SMTP, and FTP servers within the simulated Cisco environment.

### DNS Server Configuration

* A dedicated server was configured as the primary DNS server for each LAN (DNS Server 1 on LAN 1 and DNS Server 2 on LAN 2).
* DNS services were enabled on the designated servers.
* End devices on each LAN were configured to use their respective local DNS server.
* DNS resolution was tested by pinging the configured hostnames from end devices.

### SMTP Server Configuration

* Dedicated servers were configured as SMTP servers for each LAN (SMTP Server on LAN 1 and SMTP Server on LAN 2).
* SMTP services were enabled on the designated servers.
* User accounts were created on each SMTP server to allow sending and receiving emails within their respective LANs.
* Email clients on end devices were configured to use the appropriate SMTP server for their LAN.
* Email sending and receiving were tested between clients within the same LAN and across different LANs.

### FTP Server Configuration

* Dedicated servers were configured as FTP servers for each LAN (FTP Server on LAN 1 and FTP Server on LAN 2).
* FTP services were enabled on the designated servers.
* User accounts were created on each FTP server with specific permissions for accessing files.
* FTP clients on end devices were used to connect to the FTP servers.
* File upload and download functionality were tested between clients and the FTP servers.

## Technologies Used

* Cisco Networking Devices (Router, Switches)
* Network Simulation Software (e.g., Cisco Packet Tracer, GNS3)
* DNS Server Software (Integrated within the simulation environment)
* SMTP Server Software (Integrated within the simulation environment)
* FTP Server Software (Integrated within the simulation environment)

## How to Use/Replicate

1.  **Set up the Network Topology:** Recreate the network topology in your chosen network simulation software (Cisco Packet Tracer or GNS3) based on the description above or the provided `network_diagram.png`.
2.  **Configure IP Addressing:** Assign IP addresses to all devices according to the specified network scheme.
3.  **Configure Routing:** Configure the router to enable communication between LAN 1 and LAN 2. This might involve setting up routing protocols or static routes.
4.  **Configure DNS Servers:** Follow the steps outlined in the "DNS Server Configuration" section to set up the DNS servers and create the necessary A records.
5.  **Configure SMTP Servers:** Follow the steps outlined in the "SMTP Server Configuration" section to set up the SMTP servers and create user accounts.
6.  **Configure FTP Servers:** Follow the steps outlined in the "FTP Server Configuration" section to set up the FTP servers and create user accounts.
7.  **Test Connectivity and Services:** Verify network connectivity using ping and test the functionality of the DNS, SMTP, and FTP services as described in the implementation details.

## Author

* MD. REAHOON ZANNAH
