## OVERVIEW

This project concerns setting up Active Directory Domain Controller on Windows Server 2019. 

By building this, I want to learn more about creating/disabling user accounts, structuring the domain using Organization Units, 
and applying group policies. This server was built using Oracle VirtualBox

### Steps

I changed the VM’s network adapter from NAT to bridged mode to allow the machine to communicate directly on the local network.

![Network Setting](screenshots/1.png)

After the Windows Server Installation Process, install Active Directory Domain Services on Server Manager. 

Manage > Add Roles and Features > Server Roles > Active Directory Domain Services (Also added DNS and DHCP for later)

![Installing Active Directory](screenshots/3.PNG)

Once Domain Services have installed, deployment configuration must be set up.

This gives you the option to either add a domain controller to an existing domain, add a new domain to an existing forest, 

or create an entirely new forest. Since this is an entirely new domain environment, a new forest will be created

![Deployment Config](screenshots/6.PNG)

After the deployment config, it is important to promote the server as a domain controller because it elevates the server to

be able to manage domain authentication, user accounts, and network resources. 

### What I learned

I learned how to set up a Windows Server using virtualization, and the steps to set up Active Directory Domain Services. 

### What's Next?

Next, I will use AD to create users, groups, OUs, and GPOs in my domain. I will use Server to share network resources with users in the domain. 

