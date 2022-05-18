# An Overview of Firewall Technologies
## Abstract
<p>We are living in the information age. We need to keep information about every aspect of our lives. In other words, information is an asset that has value like any other asset. As an asset, information needs to be secure from attacks. The search is on for mechanisms and techniques for the protection of internal networks from such attacks. One of the protective mechanisms under serious consideration is a firewall. The Firewall is one of the most effective techniques to improve the security of a computer network. A firewall protects a network by guarding at the points of entry to it. Firewalls are becoming more sophisticated by the day, and new features are constantly being added, inspite of having limited features with them, they are still a powerful protective mechanism. This article provides an overview of firewall technologies.</p>

### Keywords:
<p>Firewall technology, network security, access control, security policy, protective mechanisms.</p>

## 1. Introduction

<p>Firewall is a security defense tool applied in the field of computer network security. A Firewall is a device (usually a router or a computer) installed between the internal network of an organization and the rest of the Internet and possesses the following properties:

* All the traffic inside to outside, and vice-versa must pass through it.
* Only authorized traffic, as defined by local security policy, is allowed to pass through it.
* The firewall itself is immune to penetration.
 </p>

![Network Security Firewall](firewall.png) 

__figure 1. Firewall semantics__

<p>The firewall is an analyzer. Be able to analyze the information flow through. And a separator, you can filter the analyzed information flow. It's also a limiter, restricting the flow of information that is screened as unsafe. Denying access to the intranet, authorize secure information flow into the intranet. Therefore, it can effectively protect network security. Ensure the security of the intranet.</p>

## 2. How Firewall Works
<p>Firewall match the network traffic against the rule set defined in its table. Once the rule is matched, associate action is applied to the network traffic. Rules can be defined on the firewall based on the necessity and security policies of the organization. From the perspective of a server, network traffic can be either outgoing or incoming. Firewall maintains a distinct set of rules for both the cases. Mostly the outgoing traffic, originated from the server itself, allowed to pass. Still, setting a rule on outgoing traffic is always better in order to achieve more security and prevent unwanted communication. Incoming traffic is treated differently. Most traffic which reaches on the firewall is one of these three major Transport Layer protocols- TCP, UDP or ICMP. All these types have a source address and destination address. Also, TCP and UDP have port numbers. ICMP uses type code instead of port number which identifies purpose of that packet.

Default policy: It is very difficult to explicitly cover every possible rule on the firewall. For this reason, the firewall must always have a default policy. Default policy only consists of action (accept, reject or drop).Suppose no rule is defined about SSH connection to the server on the firewall. So, it will follow the default policy. If default policy on the firewall is set to accept, then any computer outside of your office can establish an SSH connection to the server. Therefore, setting default policy as drop (or reject) is always a good practice.</p>

## 3. Firewalls: Basic Approaches
<p>Firewall technology can be used to protect networks, by installing it strategically at a single security screen station where the private network or the Intranet connects to the public Internet, making it easier to ensure security, audit and monitor traffic, and trace break-in attempts. It can also be used to isolate sub-networks and to provide additional layers of security (defense-in-depth) within the organization. There are three basic approaches or services that a firewall uses to protect a network: packet filtering, circuit proxy, and application proxy [6, 11].</p>

### 3.1 Packet filtering:
<p>A firewall can be used as a pocket filter. It can forward or block packets based on the information in the network-layer and transport-layer headers: source and destination IP address, source and destination port address and type of protocol(TCP or UDP). A packet-filter firewall is a router that uses a filtering table to decide which packet must be discarded.It analyses traffic at the transport protocol layer (but mainly uses first 3 layers).Packet firewalls treat each packet in isolation. They have no ability to tell whether a packet is part of an existing stream of traffic. </p>

### 3.2 Circuit proxy
<p>The second approach is the use of what is called a circuit proxy. The main difference between the circuit proxy and the packet filtering firewall is that the former is the addressee to which all communicators must address their packets. Assuming access has been granted, the circuit proxy replaces the original address with the address of the intended destination. It has the disadvantage of laying claim to the processing resources required to make changes</p>

### 3.3 Application proxy
<p>An application proxy is more complicated in operation than a packet filtering firewall or a circuit proxy. The application proxy understands the application protocol, and data and intercepts any information intended for that application. Based on the amount of information available to make decisions, the application proxy can authenticate users and judge whether any of the data could pose a threat. The price to be paid for this more comprehensive function is that users or clients often have to be reconfigured to them, sometimes a complicated process, with a consequent loss of
transparency. Application proxies are referred to as proxy services, and the host machines running them as application gateways.</p>

### 3.4 Packet instruction approach
<p>This approach, in contrast to the technologies so far described, involves inspecting the contents of packets as well as their headers. An inspection firewall carries out its inspection by using an inspection module, which understands, and can therefore inspect, data destined for all layers (from the network layer to the application layer). It carries out its inspection by integrating all information gathered from all layers into a single inspection point, and then examining it. A state-full inspection firewall registers the state of any connection it is handling and acts on this information.</p>
<p>Inspection firewalls can provide address translation and hiding, virus scanning, Web
site filtering, screening for keywords(typically in e-mail), and context-sensitive
security for complex applications.</p>


## 4. Firewall: limitations
<p>When it comes to network security, firewalls are considered the first line of defense. But the question is whether these firewalls are strong enough to make our devices safe from cyber-attacks. The answer may be "no". The best practice is to use a firewall system when using the Internet. However, it is important to use other defense systems to help protect the network and data stored on the computer. Because cyber threats are continually evolving, a firewall should not be the only consideration for protecting the home network.</p>
<p>
The importance of using firewalls as a security system is obvious; however, firewalls have some limitations:</p>

* Firewalls cannot stop users from accessing malicious websites, making it vulnerable to internal threats or attacks.
* Firewalls cannot protect against the transfer of virus-infected files or software.
* Firewalls cannot prevent misuse of passwords.-led devices updated. This includes the latest operating systems, web browsers, applications, and other security software (such as anti-virus). Besides, the security of wireless routers should be 

## 5. Conclusion
<p>Notwithstanding the limitations of firewalls and the fact that they are neither the panacea of every security aspect of a network, nor the sole sufficient bulwark against network intrusion, and despite development trends that threaten them, they are still a powerful protective mechanism and will continue to play an important and central role in the maintenance of network security for some years yet, and any organization that ignores them does so at its peril.</p>
<p>They continue to change and develop, and new features are regularly added as the need arises. If developments follow the present trend, they will continue to combine
configurable access control and authentication mechanisms with their traditional functions, thus providing more powerful and flexible protection for networks to make them secure.</p>

## 6. References
1. https://en.wikipedia.org/wiki/Firewall_(computing)
2. https://www.javatpoint.com/firewall
3. https://www.techtarget.com/searchsecurity/feature/The-five-different-types-of-firewalls
4. https://www.geeksforgeeks.org/introduction-of-firewall-in-computer-network/