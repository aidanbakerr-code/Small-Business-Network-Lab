## Company Overview

|Company Name	| Baker Digital Solutions (BDS)		|
|Industry	| IT Consulting & Digital Marketing	|
|Office Size	| 7 Employees				|		
|Location 	| One office with a single floor	|


## Employees

| Name            | Job Title             | Department     | Device           |
| --------------- | --------------------- | -------------- | ---------------- |
| Sarah Thompson  | Managing Director     | Management     | Laptop + Dock    |
| James Patel     | IT Administrator      | IT             | Desktop + Laptop |
| Emma Wilson     | Accounts Manager      | Finance        | Desktop          |
| Daniel Smith    | Sales Executive       | Sales          | Laptop           |
| Olivia Brown    | Marketing Coordinator | Marketing      | Desktop          |
| Michael Johnson | Customer Support      | Support        | Desktop          |
| Sophia Davis    | Receptionist          | Administration | Desktop          |


## Devices

| Device                | Cisco Model                   | Hostname |
| --------------------- | ----------------------------- | -------- |
| ISP Router            | Cisco ISR 4321                | ISP-RTR  |
| Business Router       | Cisco ISR 1941 (Packet Tracer)| BDS-R1   |
| Managed Switch        | Cisco Catalyst 2960-24TT 	| BDS-SW1  |
| Wireless Access Point | Cisco Aironet 1832i           | BDS-AP1  |
| Network Printer       | HP LaserJet Pro M404dn.       | BDS-PRN1 |
| NAS / File Server     | Synology DS923+               | BDS-FS1  |


## PCs

| Employee          |Hostname | Device Type  |
| --------------- | ---------| ---------------- |
| Sarah Thompson  | BDS-MGMT-PC01 | Laptop + Dock    |
| James Patel     |    BDS-IT-PC01       | Desktop + Laptop |
| Emma Wilson     |  BDS-FIN-PC01 | Desktop          |
| Daniel Smith    |   BDS-SALES-PC01 | Laptop           |
| Olivia Brown    |   BDS-MKT-PC01   | Desktop          |
| Michael Johnson | BDS-SUP-PC01 | Desktop          |
| Sophia Davis    | BDS-ADMIN-PC01 | Desktop          |

## Laptops 


| Employee       | Hostname       |
| -------------- | -------------- |
| Sarah Thompson | BDS-MGMT-LT01  |
| James Patel    | BDS-IT-LT01    |
| Daniel Smith   | BDS-SALES-LT01 |


## Business Requirements

## Functional Requirements
- Provide reliable internet connectivity to all employees.
- Enable secure communication between departments while restricting unnecessary access.
- Provide shared access to a central file server (NAS) for storing and accessing company documents.
- Allow all employees to print to a centrally managed network printer.
- Provide secure wireless connectivity for staff members.
- Provide a separate guest Wi-Fi network with internet-only access.
- Automatically assign IP addresses to employee devices using DHCP.
- Ensure all network devices can communicate with required services while maintaining appropriate network segmentation.

## Security Requirements
- Separate departments using VLANs to improve security and network management.
- Restrict guest users from accessing internal company resources.
- Secure network devices using encrypted SSH remote management.
- Configure strong passwords and encrypted credentials on all Cisco devices.
- Disable all unused switch ports to reduce security risks.
- Implement port security to prevent unauthorized devices from connecting to the network.
- Assign static IP addresses to critical infrastructure devices such as the router, switch, printer, access point, and file server.

## Availability Requirements
- Ensure employees have continuous access to network resources during business hours.
- Maintain reliable connectivity to shared services including the file server and printer.
- Create configuration backups for all Cisco networking devices to support disaster recovery.

## Scalability Requirements
- Support future growth from the current seven employees to approximately twenty employees without requiring a complete network redesign.
- Reserve additional IP address space for future users, printers, servers, and network devices.
- Allow additional VLANs to be added as new departments or business requirements emerge.

## Documentation Requirements
- Produce a complete logical network diagram.
- Maintain an IP addressing plan for all devices.
- Document VLAN assignments and network segmentation.
- Save and document router and switch configurations.
- Record testing procedures and connectivity verification.
- Create troubleshooting documentation for common network faults and their resolutions.

