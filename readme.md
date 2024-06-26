## Windows Server AD 


* Install and configure Windows Server 2022.
* Create and manage user accounts within Active Directory.
* Set up and configure Active Directory for centralized user management.
* Apply granular permissions for users like Alice and Bob based on security principles.
* Install and configure essential server roles (IIS, DNS, DHCP).
* Implement Sysmon for system activity monitoring.
* Analyze Sysmon data and present its security value to the client.

You can follow [this](https://openclassrooms.com/en/courses/7710301-manage-windows-server) tutorial to discover windows server.

## Environment:

**Resources:**

* Virtualization software: Microsoft Hyper-V, VMware Workstation, VirtualBox, QEMU.
* **Required:** <br>
[Windows Server 2022 evaluation](https://www.microsoft.com/evalcenter/evaluate-windows-server-2022)
* [Sysmon](https://learn.microsoft.com/en-us/sysinternals/downloads/sysmon) monitoring solution

## Steps:

**1. System Preparation:**

1. Set up your virtualization environment with multiple VMs:
    - Server VM (Windows Server 2022 installation)
    - Client VMs (for access and monitoring)
    - Domain Controller VM (Active Directory installation)

2. Download and install Windows Server 2022 evaluation on the Server VM and Domain Controller VM.


![1](https://github.com/malsaleh88/BXL-k4MK4r-2/assets/141853984/9ba7f506-7276-4bfc-997f-24946d8389e6)



**If you're short of resources, you can use just one server, which will be your domain controller, and one client.**

#### **Must have** : 


**2. Active Directory Setup:**

1. Promote the Domain Controller VM to a domain controller.
2. Create a new Active Directory forest and domain structure.
3. Configure DNS service on the Domain Controller VM.
4. Create organizational units (OUs) for user and group management.
5. Join the Server VM and Client VMs to the domain.


![2](https://github.com/malsaleh88/BXL-k4MK4r-2/assets/141853984/c8b8fa57-03b8-4762-9b6d-7031905816d9)


**3. User Management with Alice and Bob:**

1. Create user accounts within Active Directory:
    - Alice (Administrator, assigned to dedicated OU)
    - Bob (Standard User with access to `/Users/Bob` folder, assigned to specific OU)
2. Leverage Group Policy Objects (GPOs) to configure user settings based on OUs.
3. Implement granular permissions based on security principles for both Alice and Bob.

![2](https://github.com/malsaleh88/BXL-k4MK4r-2/assets/141853984/ec4647a3-9b33-4103-a269-17d1bcb66306)

![3](https://github.com/malsaleh88/BXL-k4MK4r-2/assets/141853984/0ef9fe22-1f02-4db3-9d53-fdceb76a8e2a)

**4. Server Roles:**

**4.1 IIS for Alice:**

1. Install and configure [IIS](https://www.iis.net/overview) on the Server VM for Alice's specific web application/service.

2. Apply robust security best practices (permissions, WAFs, considering Alice's admin role).
3. Test the web application and ensure accessibility for authorized users in the domain.




![iis](https://github.com/malsaleh88/BXL-k4MK4r-2/assets/141853984/ecb1ee1d-23d9-4630-86af-22a50e1e1d5a)


**4.2 DNS:**

1. Verify DNS functionality within the Active Directory domain environment.
2. Configure conditional forwarders or external DNS integration if needed.

![DNS](https://github.com/malsaleh88/BXL-k4MK4r-2/assets/141853984/a2122320-bc58-424e-b025-ca779522517b)


**4.3 DHCP:**

1. Install and configure DHCP on the Server VM for automatic IP assignment within the domain.

2. Integrate DHCP with Active Directory for dynamic DNS updates (optional).


![DHCP](https://github.com/malsaleh88/BXL-k4MK4r-2/assets/141853984/498494b0-ee46-4767-baf8-b5eb378397aa)

![dhsp-](https://github.com/malsaleh88/BXL-k4MK4r-2/assets/141853984/3601fae8-f83b-433f-aaba-b75b015e96c3)






