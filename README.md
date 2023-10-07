# Modern-Hotel-Network
To design and implement the Vic Modern Hotel network as per your requirements, you'll need to consider various aspects including physical layout, IP addressing, VLANs, routing, DHCP, and SSH configuration. Here's a project summary to guide you through the process:

1. **Physical Layout**:
   - Three floors in the hotel.
   - Each floor has a server room where routers will be placed.
   - Each floor has a switch for local connectivity.
   - Wi-Fi networks are required on each floor.
   - Each department has a printer.

2. **Router Configuration**:
   - Install three routers in the server room on the third floor (IT and Admin).
   - Connect these routers using serial DCE cables with the following subnets:
     - Router 1: 10.10.10.1/30
     - Router 2: 10.10.10.5/30
     - Router 3: 10.10.10.9/30
   - Use OSPF as the routing protocol to advertise routes between routers.

3. **Switch Configuration**:
   - Place one switch on each floor (connected to the respective router).
   - Configure VLANs for each department (Reception, Store, Logistics, Finance, HR, Sales/Marketing, IT, and Admin).
   - Associate VLANs with their respective IP subnets.

4. **VLAN and IP Addressing**:
   - Define VLANs and IP subnets for each department as specified in your requirements.

5. **Wi-Fi Network**:
   - Set up Wi-Fi networks on each floor for laptops and phones.
   - Assign appropriate VLANs to these wireless networks.

6. **Printer Setup**:
   - Each department should have its own printer.
   - Configure the printers on their respective VLANs.

7. **DHCP Configuration**:
   - Configure each router as a DHCP server for its VLAN.
   - Ensure that devices within each VLAN obtain IP addresses dynamically from their respective routers.

8. **Interdepartmental Communication**:
   - Ensure that all devices in the network can communicate with each other.
   - This can be achieved by configuring the routers to route traffic between VLANs and using OSPF for routing.

9. **SSH Configuration**:
   - Secure remote access by configuring SSH on all routers.
   - Create secure login credentials for SSH access.

10. **Testing and Documentation**:
    - Thoroughly test the network to ensure proper functionality.
    - Document the network design, configurations, IP addresses, and any security settings.
    - Provide instructions for future maintenance and troubleshooting.

11. **Security**:
    - Implement access control lists (ACLs) or firewall rules to restrict unauthorized access between departments or to critical network resources.

12. **Monitoring and Management**:
    - Consider implementing network monitoring tools to ensure the network's health and security.
    - Plan for ongoing network management and maintenance.

13. **Backup and Redundancy**:
    - Implement regular backup and redundancy measures to ensure network uptime and data integrity.

14. **User Training**:
    - Provide training to hotel staff on how to connect to and use the network, especially for Wi-Fi access.

15. **Compliance and Regulations**:
    - Ensure that the network design complies with any relevant regulations and data privacy requirements.

16. **Documentation and Handover**:
    - Create detailed network documentation, diagrams, and handover materials for future support and maintenance.

This project summary outlines the key steps and considerations for designing and implementing the Vic Modern Hotel network. Ensure proper planning, testing, and documentation to achieve a reliable and efficient network infrastructure.
