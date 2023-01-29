#  **NETWORKING**
___

## **LAN**

__
-   LAN stands for Local Area Network
-   It is a network of devices (such as computers, servers, and printers) that are connected in a limited geographical area (such as a home, office, or building)
-   The devices on a LAN can communicate and share resources (such as files, internet access, and printers)
-   LANs can be connected to other LANs or to the internet using devices such as routers or modems
-   LANs can be wired (using Ethernet cables) or wireless (using Wi-Fi)

___

## **IP ADDRESS**
___

-   IP stands for Internet Protocol
-   An IP address is a numerical label assigned to each device connected to a computer network that uses the Internet Protocol for communication.
-   IP addresses are used to identify and locate devices on a network
-   An IP address is a unique identifier for a device and it is usually written in the form of four sets of numbers separated by dots, like “192.168.0.1”
- Two types of IP addresses are IPv4 and IPv6, the main difference is the number of bits used to represent an IP address. IPv4 uses 32 bits, while IPv6 uses 128 bits.
-   IP addresses can be divided into two types: static and dynamic. A static IP address is a fixed address assigned to a device, while a dynamic IP address is one that can change over time.
- IP addresses are used to route data to specific devices on a network, allowing them to communicate with other devices or networks.
___

## **SUBNET**
___

- A subnet, short for "subnetwork", is a way to divide a larger network into smaller, more manageable parts.
- Each subnet has its own unique range of IP addresses.
- This allows for better organization and security of a network, as well as the ability to control the flow of data between different parts of the network.
- Subnetting is done by borrowing bits from the host portion of the IP address and using them for the subnet portion.
- This allows for a larger number of subnets and smaller number of hosts per subnet.
- Dividing a network into subnets can also help reduce network congestion and improve network performance.
- It also allows for the creation of VLANs (Virtual Local Area Network) that can be used to segment a network for security, management or other reasons.

## **SWITCH**
___

-   A switch is a networking device that connects multiple devices together on a network.
-   It forwards data packets between devices on a LAN (Local Area Network)
        -A data packet is a small unit of digital information that is sent over a network. It contains the data being transmitted, as well as information about where the data came from and where it's going. Data packets are created by the sender's device and are then sent over the network to the intended recipient. Along the way, data packets may pass through multiple devices such as routers and switches, which help direct the packets to their final destination. The data packets are reassembled at the destination to form the original message. In summary, data packets are a way for digital information to be broken down into smaller chunks for efficient transmission over a network.
-   A switch operates at the data link layer (layer 2) of the OSI model
        - Data Link Layer (layer 2): It is one of the seven layers in the OSI (Open Systems Interconnection) model. It is responsible for creating a reliable link between two devices on a network by providing a means for error-free data transfer. It is responsible for the physical addressing and logical addressing, also known as MAC and LLC respectively.

        - OSI Model: OSI (Open Systems Interconnection) is a reference model for how communication should occur between two devices on a network. It is divided into seven layers, each with a specific purpose. The layers are:

            1. Physical Layer: It deals with the physical connection between devices.
            2. Data Link Layer: It deals with creating a reliable link between two devices and error-free data transfer.
            3. Network Layer: It deals with routing data packets between devices.
            4. Transport Layer: It deals with ensuring that data is delivered reliably and in order.
            5. Session Layer: It deals with establishing, maintaining, and terminating connections between devices.
            6. Presentation Layer: It deals with the format of the data being transmitted.
           7. Application Layer: It deals with the applications and users that interact with the network.

        # MEMONIC TO REMEMBER THE OSI MODEL
                -All           => Application
                -People        => Presentation
                -Seem          => Session
                -To            => Transport
                -Need          => Network
                -Data          => Data Link
                -Processing    => Processing
        - Each layer communicates with the layer above and below it to ensure that data is transmitted correctly and efficiently.
-   It uses MAC addresses to forward the data packets to the correct destination
-   A switch can also provide security by isolating different parts of the network, and it can improve network performance by reducing network congestion.
-   A switch can be managed or unmanaged. Managed switch have more advanced features like VLAN, Quality of Service (QoS), and Remote management.
-   A switch can have multiple ports, which allows multiple devices to be connected to the switch.
-   Some switches can also provide Power over Ethernet (PoE) to devices, which allows them to receive power over the Ethernet cable, eliminating the need for a separate power source.

___

## **Router**
___

- A router is a networking device that connects multiple networks together and routes data packets between them. It operates at the network layer (layer 3) of the OSI (Open Systems Interconnection) model. 
- A router uses routing tables and protocols to determine the best path for data packets to travel from one network to another. 
- It can also provide network services such as DHCP, NAT, and VPN. A router can have multiple WAN (Wide Area Network) and LAN (Local Area Network) ports, allowing it to connect to different networks such as the internet, and multiple devices such as computers and servers to the same network. It can also provide network security by using firewalls and other security features.
___

## **DMZ**
___

- DMZ stands for Demilitarized Zone
- It is a network segment that is isolated from the rest of the internal network
- It is usually used to host public-facing servers such as web servers, email servers, and DNS servers
- The purpose of a DMZ is to provide an additional layer of security for the internal network by isolating it from the public-facing servers
- A DMZ is typically created by using a firewall to control access to the internal network from the DMZ, and another firewall to control access from the DMZ to the internet
- Only necessary ports are opened on the firewall to the DMZ, while all other ports are closed, this makes it more difficult for attackers to access the internal network
- DMZ can also reduce the attack surface of the internal network by keeping all public-facing servers and services in one location
- DMZ also allows to maintain compliance and security standards required by various regulatory bodies.

___

## **PORT FOWARDING**
___

-   Port forwarding is a technique used to allow external devices to access services on a private network.
-   It is typically used to allow access to services such as web servers, game servers, and other applications that run on a private network.
-   The process involves forwarding a specific port on the router to a specific IP address and port on the internal network.
-   This allows external devices to connect to the service on the internal network using the router's public IP address and the forwarded port.
-   Port forwarding can be set up manually through the router's web interface or automatically using software.
-   It is important to note that port forwarding can also be a security risk as it opens up a port on the router to the internet. It is important to only forward the ports that are necessary and to keep the software and firmware on the router up to date.

___
## **PORT**
___

-   A port in networking is a virtual pathway on a computer or network device that allows different types of data to flow in and out.
-   Each port is identified by a unique number, called the "port number", that ranges from 0 to 65535.
-   Different types of data and services use specific port numbers. For example, web traffic uses port 80, while email uses port 25.
-   An IP address is a unique numerical label assigned to each device connected to a computer network that uses the Internet Protocol for communication.
-   An IP address identifies the device and its location on the network, while a port number identifies a specific process or service running on that device.
-   Together, an IP address and a port number create a unique endpoint for data to be sent to or received from.

-   For example, if you want to access a website on your computer, your computer sends a request to the website's IP address, and then the website sends the data back to your computer via the port number.


___


## **FIREWALL**

___

- A firewall is a network security system that monitors and controls incoming and outgoing network traffic based on predetermined security rules and policies.
- Its main function is to prevent unauthorized access to or from a private network.
- Firewalls can be implemented in hardware, software or a combination of both.
- Firewalls use a set of rules to allow or block traffic based on IP addresses, ports, and other parameters.
- They can be used to protect a single computer, or a network of computers.
- Firewalls can also include other security features such as intrusion detection and prevention, and VPN support.
- Firewalls are typically the first line of defense in protecting a network from external threats.






