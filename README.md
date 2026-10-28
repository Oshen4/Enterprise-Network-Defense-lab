# Enterprise-Network-Defense-lab

Enterprise Network Defense & VLAN Segmentation Lab
Project Overview

A hands-on enterprise network security lab developed in Cisco Packet Tracer to practice network segmentation, inter-VLAN routing, and traffic access control using Cisco IOS.
Objectives

    Design an enterprise network with separate departmental VLANs.
    Configure 802.1Q trunking and router-on-a-stick routing.
    Implement extended Access Control Lists (ACLs).
    Test network reachability and intended traffic restrictions.
    Document configuration and verification evidence.

Network Design
VLAN	Department	Subnet	Gateway
10	Finance	192.168.10.0/24	192.168.10.1
20	IT	192.168.20.0/24	192.168.20.1
30	Servers	192.168.30.0/24	192.168.30.1
99	Management	192.168.99.0/24	192.168.99.1
Security Implementation

    Created separate VLANs for Finance, IT, Servers, and Management.
    Configured an 802.1Q trunk between the switch and router.
    Implemented router subinterfaces for inter-VLAN routing.
    Applied an extended ACL to block Finance-to-IT and Finance-to-Management IP traffic.
    Used Cisco IOS verification commands to inspect VLANs, trunk status, interfaces, and ACL counters.

Testing and Validation

Record the actual outcome of each test.
Test	Expected outcome	Actual outcome
Finance to Server	Permitted by the configured ACL	Add observed result
Finance to IT	Denied	Add observed result
Finance to Management	Denied	Add observed result
IT to Finance	Permitted by the Finance-side ACL policy	Add observed result
Tools and Technologies

Cisco Packet Tracer, Cisco IOS CLI, IPv4 subnetting, VLANs, IEEE 802.1Q, router-on-a-stick routing, extended ACLs, and network troubleshooting.
Key Learning Outcomes

Practiced implementing network segmentation, translating a security policy into router ACL rules, verifying network configuration, and documenting observed results.
Limitations and Future Improvements

This is a simulated lab, not a production deployment. The initial ACL allows other Finance IP traffic not explicitly denied. Future improvements include least-privilege server rules, stronger management-plane restrictions, and additional security monitoring.
