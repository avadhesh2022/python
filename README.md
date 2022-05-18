# An Overview of Firewall Technologies
## Abstract
<p>We are living in the information age. We need to keep information about every aspect of our lives. In other words, information is an asset that has value like any other asset. As an asset, information needs to be secure from attacks. The search is for mechanisms and techniques for the protection of internal networks from such attacks. One of the protective mechanisms under serious consideration is the firewall. A Firewall is one of the most effective techniques to improve the security of a computer network. A firewall protects a network by guarding at the points of entry to it. Firewalls are becoming more sophisticated by the day, and new features are constantly being added, so that, despite the criticisms made of them and developmental trends threatening them, they are still a powerful protective mechanism. This article provides an overview of firewall technologies.</p>

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

## 2. Firewalls: Basic Approaches
<p>Firewall technology can be used to protect networks, by installing it strategically at a single security screen station where the private network or the Intranet connects to the public Internet, making it easier to ensure security, audit and monitor traffic, and trace break-in attempts. It can also be used to isolate sub-networks and to provide additional layers of security (defense-in-depth) within the organization. There are three basic approaches or services that a firewall uses to protect a network: packet filtering, circuit proxy, and application proxy [6, 11].</p>

### 2.1 Packet filtering:
<p>A firewall can be used as a pocket filter. It can forward or block packets based on the information in the network-layer and transport-layer headers: source and destination IP address, source and destination port address and type of protocol(TCP or UDP). A packet-filter firewall is a router that uses a filtering table to decide which packet must be discarded.</p>

### 2.2 Circuit proxy
<p>The second approach is the use of what is called a circuit proxy. The main difference between the circuit proxy and the packet filtering firewall is that the former is the addressee to which all communicators must address their packets. Assuming access has been granted, the circuit proxy replaces the original address with the address of the intended destination. It has the disadvantage of laying claim to the processing resources required to make changes</p>

### 2.3 Application proxy
<p>An application proxy is more complicated in operation than a packet filtering firewall or a circuit proxy. The application proxy understands the application protocol, and data and intercepts any information intended for that application. Based on the amount of information available to make decisions, the application proxy can authenticate users and judge whether any of the data could pose a threat. The price to be paid for this more comprehensive function is that users or clients often have to be reconfigured to them, sometimes a complicated process, with a consequent loss of
transparency. Application proxies are referred to as proxy services, and the host machines running them as application gateways.</p>

### 2.4 Packet instruction approach
<p>This approach, in contrast to the technologies so far described, involves inspecting the contents of packets as well as their headers. An inspection firewall carries out its inspection by using an inspection module, which understands, and can therefore inspect, data destined for all layers (from the network layer to the application layer). It carries out its inspection by integrating all information gathered from all layers into a single inspection point, and then examining it. A state-full inspection firewall registers the state of any connection it is handling and acts on this information.</p>
<p>Inspection firewalls can provide address translation and hiding, virus scanning, Web
site filtering, screening for keywords(typically in e-mail), and context-sensitive
security for complex applications.</p>


## 3. Firewall: limitations
<p>When it comes to network security, firewalls are considered the first line of defense. But the question is whether these firewalls are strong enough to make our devices safe from cyber-attacks. The answer may be "no". The best practice is to use a firewall system when using the Internet. However, it is important to use other defense systems to help protect the network and data stored on the computer. Because cyber threats are continually evolving, a firewall should not be the only consideration for protecting the home network.</p>
<p>
The importance of using firewalls as a security system is obvious; however, firewalls have some limitations:</p>

* Firewalls cannot stop users from accessing malicious websites, making it vulnerable to internal threats or attacks.
* Firewalls cannot protect against the transfer of virus-infected files or software.
* Firewalls cannot prevent misuse of passwords.<!--led devices updated. This includes the latest operating systems, web browsers, applications, and other security software (such as anti-virus). Besides, the security of wireless routers should be another practice. The process of protecting a router may include options such as repeatedly changing the router's name and password, reviewing security settings, and creating a guest network for visitors.</p>
<!--
## 4. Trends Threatening Firewalls - and Counter Trends
<!--
### 4.1 Trends Threatening Firewalls
<!--
<p>The traditional assumption that all inside the firewall are friendly and all outside it
potentially hostile, is now becoming somewhat outdated. Internet connectivity has
expanded, Extranets can allow outsiders access to areas protected by firewalls, and
some machines require greater access to the outside than others, which often involves
a change in the internal IP address. Another threat is the use of end-to-end encryption
since the firewall is unable to peer through the encryption.</p>
<p>In the literature [3], some people have gone so far as to suggest that a more adaptive
approach would be to drop firewalls altogether on the basis that they are obsolete, or
that the use of cryptography obviates the need for them. </p>
<!--
### 4.2 Counter trends and Arguments 
<p>Firewalls are still powerful protective mechanisms for the following reasons:</p>
<!--
* Firewalls are  useful for protecting legacy systems. While applications that require strong authentication should provide their own, there are too many older
protocols and implementations that do not. Saying that strong cryptography should be used is true but irrelevant. In the context of such applications, it is
simply unavailable.
<!--
* More subtly, firewalls are a mechanism for policy control. That is, they permit a
site's administrator to set a policy on external access. Just as file permissions
enforce an internal security policy, a firewall can enforce an external security
policy.
<p>As already stated, we concur with the above, and cite the following additional
arguments.</p>
<p>Cryptography notwithstanding, the use of firewalls is deeply entrenched in several organizations and is part and parcel of their security setup, and will continue to be so for some years yet. While it is true that cryptography is the heir apparent to the firewall, the number of as yet unresolved issues prevents the assembling of a comprehensive solution for securing distributed computing resources around the Public Key Infrastructure (PKI) and encryption. In addition, the process of standardization within the area of PKI is not proceeding particularly rapidly. Thus, even those organizations favoring technologies other than firewalls will just have to bite the bullet and live with them for the moment.</p>
<p>Another factor is the ongoing development of new features and services at present being continually added to firewalls. These reduce the number of the limitations listed above and increase the firewall's flexibility while allowing it to retain its original function unimpaired. Examples, to mention but a few, that illustrate this point are:</p>
 <!--
* The proposal of a distributed firewall [3], using IPSEC (IP Security), a policy
language, and system management tools, that preserves central control of access
policy while reducing or eliminating any dependency on topology.
* Phoenix's Adaptive Firewall Technology [17], as noted above, provides self-adapting control of network access, thus establishing an effective network
security policy by examining every packet and adapting rules on the fly based on information in the packet passing through the network interface.
<!--
* FORE Systems' Firewall Switching Agent [8], in combination with Check Point's Firewall-1 [5], provides 20 Gbps of firewall switching bandwidth while delivering wire-speed routing, switching, and class-of-service delivery.
* OMG's [15] CORBA Firewall Security [13], which brings firewalls to distributed object technology and provides a standard approach by which a firewall identifies and controls the flow of IIOP (Internet Inter-ORB Protocol), which has become
the defacto standard interoperability protocol for the Internet, providing "out-of-the-box" interoperation with ORBs (Object Request Brokers), thereby increasing the security of CORBA-based applications [1].
<p>These trends in the development of firewalls make them important mechanisms to ease the transition to flexible and truly distributed security solutions, such as CORBA Security Services [14], thus sparing traditionally-minded network/firewall
administrators much discomfort. After all, the laboratory test results described in "Super firewalls" [12] show that today's high-end firewalls are tougher, faster, and easier to use.</p>
-->

## 5. Conclusion
<p>Notwithstanding the limitations of firewalls and the fact that they are neither the panacea of every security aspect of a network, nor the sole sufficient bulwark against network intrusion, and despite development trends that threaten them, they are still a powerful protective mechanism and will continue to play an important and central role in the maintenance of network security for some years yet, and any organization that ignores them does so at its peril.</p>
<p>They continue to change and develop, and new features are regularly added as the need arises. If developments follow the present trend, they will continue to combine
configurable access control and authentication mechanisms with their traditional functions, thus providing more powerful and flexible protection for networks to make them secure.</p>

## 6. References
1. https://www.javatpoint.com/firewall
2. https://www.techtarget.com/searchsecurity/feature/The-five-different-types-of-firewalls