
## Introduction
This document outlines the steps taken to set up network security measures for the VeryEasyIT client. The goal was to ensure secure access for two users, Alice and Bob, while configuring firewall settings and detecting Windows operating systems on the network.

## User Setup
- **Alice**: Configured as the system administrator with full access privileges.
- **Bob**: Created as a standard user with restricted access limited to reading, writing, and executing files within the /Users/Bob folder.

![add user](https://github.com/malsaleh88/BXL-k4MK4r-2/assets/141853984/6b12994d-ac0b-4e00-8975-a3a77d0a99f2)

![alice create](https://github.com/malsaleh88/BXL-k4MK4r-2/assets/141853984/0ed6fb04-3dd6-42ba-bd3f-eb2a07abbc4f)


![properiteis](https://github.com/malsaleh88/BXL-k4MK4r-2/assets/141853984/a50e6111-a7de-473c-853f-d7d8444e85c9)

![find admin](https://github.com/malsaleh88/BXL-k4MK4r-2/assets/141853984/e6f5ea96-1ec7-48dc-8e17-0d60130c6775)

![amdinnn2](https://github.com/malsaleh88/BXL-k4MK4r-2/assets/141853984/d69f0de1-8133-4263-9f17-426272cca4c3)

![alicesigin](https://github.com/malsaleh88/BXL-k4MK4r-2/assets/141853984/cbd989a4-5da1-4dc8-a5cb-2363ede30643)

![bob secrurity](https://github.com/malsaleh88/BXL-k4MK4r-2/assets/141853984/87c26596-1ee4-4000-a9ad-b95bec1bde94)

![rzex](https://github.com/malsaleh88/BXL-k4MK4r-2/assets/141853984/03e89ac8-a352-48b1-bdf2-781c5446c2e7)




## Firewall Configuration
- Utilized the built-in Windows Firewall for network protection.
- Configured firewall settings to control inbound and outbound traffic.
- Created custom rules to allow specific programs and ports while blocking unauthorized access.

![firewall](https://github.com/malsaleh88/BXL-k4MK4r-2/assets/141853984/f9fef3fb-bf4b-4e6b-81a5-dbcabe12b51a)


## Windows Detection
- Employed Nmap for network scanning and detection of Windows operating systems.
- Conducted scans to identify active hosts and discover open ports and services.
- Utilized Nmap's scripting engine for advanced scanning and analysis.
![windows security](https://github.com/malsaleh88/BXL-k4MK4r-2/assets/141853984/e16d5b7f-796a-42ec-a364-394f38d04b91)

![real-time](https://github.com/malsaleh88/BXL-k4MK4r-2/assets/141853984/c84647a5-8937-4367-aa58-98cb010a834e)

![quick](https://github.com/malsaleh88/BXL-k4MK4r-2/assets/141853984/a3ae718c-ea9d-4f92-9cbb-3a9077b14f3a)




## Conclusion
By implementing user-specific access controls, configuring firewall settings, and utilizing network scanning tools, the network security setup for the VeryEasyIT client has been enhanced. Alice and Bob have appropriate access privileges, and the firewall provides protection against unauthorized access. Continuous monitoring and updates will ensure ongoing network security.

For further details and documentation, refer to the corresponding configuration files and scripts in the repository.


