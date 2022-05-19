# An Overview of Firewall Technologies
## Abstract
We are living in the information age. We need to keep information about every aspect of our lives. During the last three decades, computer networks created a revolution in the use of information.    Information is now distributed all over the world through a computer network. Information is an asset that has value like any other asset. As an asset, information needs to be secure from attacks. The search is going on for mechanisms and techniques for the protection of internal networks from attacks. One of the protective mechanisms under serious consideration is a firewall. It is one of the most effective techniques to improve the security of a computer network. It protects a network by guarding at the points of entry to it. These are becoming more sophisticated by the day, and new features are constantly being added, despite having limited features with them, they are still a powerful protective mechanism. This article provides an overview of firewall technologies.

### Keywords:
Firewall technology, network security, access control, security policy, and protective mechanisms.

## 1. Introduction
A firewall is a security defense tool applied in the field of computer network security. It is a device (usually a router or a computer) installed between the internal network of an organization and the rest of the Internet and possesses the following properties:

* All the traffic inside to outside, and vice-versa must pass through it.
* Only authorized traffic, as defined by local security policy, is allowed to pass through it.
* The firewall itself is immune to penetration.
 

![Network Security Firewall](firewall.png) 

figure 1. Firewall semantics

A firewall is an analyzer. It is can analyze the information flow through. And a separator can filter the analyzed information flow. It's also a limiter, restricting the flow of information that is screened as unsafe. Denying access to the intranet, authorize secure information flow into the intranet. Therefore, it can effectively protect network security. Ensure the security of the intranet.

## 2. How Firewall Works
A firewall matches the network traffic against the rule set defined in its table. Once the rule is matched, associate action is applied to the network traffic. Rules can be defined on the firewall based on the necessity and security policies of the organization. From the perspective of a server, network traffic can be either outgoing or incoming. The Firewall maintains a distinct set of rules for both cases. Mostly the outgoing traffic, which originated from the server itself and allowed to pass. Still, setting a rule on outgoing traffic is always better to achieve more security and prevent unwanted communication. Incoming traffic is treated differently. Most traffic that reaches the firewall is one of these three major Transport Layer protocols- TCP, UDP or ICMP. All these types have a source address and destination address. Also, TCP and UDP have port numbers. ICMP uses type code instead of port number which identifies the purpose of that packet.

It is very difficult to explicitly cover every possible rule on the firewall. For this reason, the firewall must always have a default policy. Default policy only consists of action (accept, reject or drop). Suppose no rule is defined about SSH connection to the server on the firewall. So, it will follow the default policy. If the default policy on the firewall is set to accept, then any computer outside of your office can establish an SSH connection to the server. Therefore, setting the default policy as a drop (or reject) is always a good practice.

## 3. Types of Firewalls

Firewalls are also categorized based on how they operate, and each type can be set up either as software or a physical device. Based on their method of operation, there are four different types of firewalls.

### 3.1 Packet filtering:
A firewall can be used as a pocket filter. It can forward or block packets based on the information in the network-layer and transport-layer headers: source and destination IP address, source and destination port address and type of protocol(TCP or UDP). A packet-filter firewall is a router that uses a filtering table to decide which packet must be discarded. It analyses traffic at the transport protocol layer. Packet firewalls treat each packet in isolation. They can't tell whether a packet is part of an existing stream of traffic.

### 3.2 Circuit-Level Gateways
The main difference between the circuit level gateways and the packet filtering firewall is that the former is the addressee to which all communicators must address their packets. Assuming access has been granted, the circuit proxy replaces the original address with the address of the intended destination. However, their inability to inspect the content of data packets makes them an incomplete security solution on their own. A data packet containing malware can bypass a circuit-level gateway easily if it has a legitimate TCP handshake. That is why another type of firewall is often configured on top of circuit-level gateways for added protection.

### 3.3 Application-Level gateways (Proxy Firewalls)
Proxy firewalls are implemented at the application layer via a proxy device. Instead of an outsider accessing your internal network directly, the connection is established through the proxy firewall. The external client sends a request to the proxy firewall. After verifying the authenticity of the request, the proxy firewall forwards it to one of the internal devices or servers on the client’s behalf. Alternatively, an internal device may request access to a webpage, and the proxy device will forward the request while hiding the identity and location of the internal devices and network. Unlike packet filtering firewalls, proxy firewalls perform stateful and deep packet inspection to analyze the context and content of data packets against a set of user-defined rules. Based on the outcome, they either permit or discard a packet. They protect the identity and location of your sensitive resources by preventing a direct connection between internal systems and external networks.

### 3.4 Packet instruction approach
A step ahead of circuit-level gateways, stateful inspection firewalls, and verifying and keeping track of established connections also perform packet inspection to provide better, more comprehensive security. They work by creating a state table with source IP, destination IP, source port, and destination port once a connection is established. They create their own rules dynamically to allow expected incoming network traffic instead of relying on a hardcoded set of rules based on this information. They conveniently drop data packets that do not belong to a verified active connection.


## 4. Firewall: limitations
When it comes to network security, firewalls are considered the first line of defense. But the question is whether these firewalls are strong enough to make our devices safe from cyber-attacks. The answer may be "no". The best practice is to use a firewall system when using the Internet. However, it is important to use other defense systems to help protect the network and data stored on the computer. Because cyber threats are continually evolving, a firewall should not be the only consideration for protecting the home network.

The importance of using firewalls as a security system is obvious; however, firewalls have some limitations:

*  Firewalls cannot stop users from accessing malicious websites, making them vulnerable to internal threats or attacks.
* Firewalls cannot protect against the transfer of virus-infected files or software.
* Firewalls cannot prevent misuse of passwords.-led devices updated. This includes the latest operating systems, web browsers, applications, and other security software (such as anti-virus). Besides, the security of wireless routers should be.

## 5. Conclusion
Notwithstanding the limitations of firewalls and the fact that they are neither the panacea of every security aspect of a network, nor the sole sufficient bulwark against network intrusion, and despite development trends that threaten them, they are still a powerful protective mechanism and will continue to play an important and central role in the maintenance of network security for some years yet, and any organization that ignores them does so at its peril.

They continue to change and develop, and new features are regularly added as the need arises. If developments follow the present trend, they will continue to combine
configurable access control and authentication mechanisms with their traditional functions, thus providing more powerful and flexible protection for networks to make them secure.

## 6. References

1. https://en.wikipedia.org/wiki/Firewall_(computing)
2. https://www.tunnelsup.com/what-is-a-firewall/
3. https://www.simplilearn.com/tutorials/cyber-security-tutorial/what-is-firewall
4. https://www.javatpoint.com/firewall
5. https://www.techtarget.com/searchsecurity/feature/The-five-different-types-of-firewalls
6. https://www.geeksforgeeks.org/introduction-of-firewall-in-computer-network/
7. https://www.parallels.com/blogs/ras/types-of-firewalls/