___

## **REMOTE ACCESS CONCEPTS**
___

- Consider MSPs & MSSPs, both industries are primarily dependent on managing their client's computer systems remotely. 

- This functionality allows them to;
    a). centralize management, 

    b). standardize what technologies are used,

    c). automate numerous tasks,

    d). enable remote work arrangements and allow for quick response time when issues surface, or potential security threats emerge. 
    
    Remote access is not just limited to MSPs & MSSPs. Organizations with IT, Software Development &/or Security teams use remote access methods daily to build applications, manage servers and administer employee workstations. Some of the most common remote access technologies include but aren't limited to:

___

## **MANAGED SERVICE PROVIDERS AND MANAGED SECURITY SERVICE PROVIDERS**
___

- MSPs (Managed Service Providers) and MSSPs (Managed Security Service Providers) are companies that provide managed IT services and security services to businesses and organizations. MSPs typically offer a range of IT services such as network management, data backup and recovery, and software updates, while MSSPs focus specifically on providing security services such as firewall management, intrusion detection, and compliance management. Both types of organizations can help businesses reduce costs and improve efficiency by outsourcing IT and security management tasks.

- Some of the most common remote access technologies include but aren't limited to:

1. Virtual Private Networks (VPN):
- A VPN is a private network that uses a public network (usually the internet) to connect remote sites or users together.
- It allows users to access a private network and share data remotely through public networks.
- It encrypts data to keep it secure and protect it from unauthorized access.


2. Secure Shell (SSH):
- SSH is a protocol used to securely log into a remote machine, execute commands and manage networks.
- It encrypts the session to protect against malicious attacks.
- It can be used to remotely connect to a machine and perform various tasks such as file transfers, and even run a virtual desktop session.


3. File Transfer Protocol (FTP):
- FTP is a standard protocol used for transferring files between computers on a network.
- It is used to upload and download files to and from a server.
- It can be used to transfer files of any type, including text, images, and binary files.


4. Virtual Network Computing (VNC):
- VNC is a remote desktop protocol that allows users to view and interact with a computer remotely.
- It captures the desktop of the remote machine and sends it to the user, allowing the user to remotely control the machine as if they were physically sitting in front of it.
- It works on any platform and supports multiple operating systems.


5. Windows Remote Management (or PowerShell Remoting) (WinRM):
- WinRM is a protocol that allows administrators to remotely manage Windows-based servers and clients.
- It uses the Windows Remote Management (WinRM) service to enable remote management of Windows-based computers.
- It can be used to remotely run PowerShell commands and scripts, or even access the remote desktop session.


6. Remote Desktop Protocol (RDP):
- RDP is a proprietary protocol developed by Microsoft that allows users to remotely connect to a Windows-based computer.
- It captures the desktop of the remote machine and sends it to the user, allowing the user to remotely control the machine as if they were physically sitting in front of it.
- It requires a Windows operating system on both the remote and local machines.


* These technologies are widely used in the IT industry to enable remote access, management and control of networked devices and systems.


___
___

## **REMOTE DESKTOP PROTOCAL**

___
___

- RDP uses a client/server architecture where a client-side application is used to specify a computer's target IP address or hostname over a network where RDP access is enabled. The target computer where RDP remote access is enabled is considered the server. It is important to note that RDP listens by default on logical port 3389. Keep in mind that an IP address is used as a logical identifier for a computer on a network, and a logical port is an identifier assigned to an application. In simpler terms, we could consider a network subnet a street in a town (the corporate network), an IP address in that subnet assigned to a host as a house on that street, and logical ports as windows/doors that can be used to access the house.

- Once a request (encapsulated inside a packet) has reached a destination computer via its IP address, the request will be directed to an application hosted on the computer based on the port specified in that request (included as a header inside a packet). IP addressing and protocol encapsulation are covered in greater detail in the module Introduction to Networking. From a networking perspective, in this module, we only need to understand that every computer has an IP address assigned to communicate over a network, and applications hosted on target computers listen on specific logical ports.

- We can use RDP to connect to a Windows target from an attack host running Linux or Windows. If we are connecting to a Windows target from a Windows host, we can use the built-in RDP client application called Remote Desktop Connection (mstsc.exe).

- For this to work, remote access must already be allowed on the target Windows system. By default, remote access is not allowed on Windows operating systems. The HTB Academy team has configured many of our Windows targets to permit RDP access once connected to the Academy labs via VPN.

- Remote Desktop Connection also allows us to save connection profiles. This is a common habit among IT admins because it makes connecting to remote systems more convenient.

___
___

## **xfreerdp**
___
___

- xfreerdp is a command line tool for remotely connecting to Windows systems using the Remote Desktop Protocol (RDP).

- It is an open-source implementation of the RDP client that is built on the FreeRDP library. 

- It can be used to connect to Windows desktops and servers, and it supports a wide range of features including RemoteFX, Network Level Authentication (NLA), and RemoteApp. 

- The tool is available for Linux, MacOS and Windows.

- From a Linux-based attack host we can use a tool called xfreerdp to remotely access Windows targets. You will notice that we use xfreerdp across multiple modules because of its ease of use, feature set, command line utility, and efficiency.

- Remember that we can also copy and paste in xfreerdp commands in the command line, so we do not need to enter options manually. There are several options available to us with xfreerdp, such as drive redirection to be able to tranfer files to/from the target host, which are worth practicing and we will cover in other modules within HTB Academy.

- Other RDP clients exist, such as Remmina and rdesktop, and we encourage you to experiment with others and see what works best for you.