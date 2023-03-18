1) Explain the subnet and use the NMAP Command to scan the services for the whole subnet.

Subnet is a segmented piece of a larger network. It falls within the class A, B or C range. Ip address are used for subnetting. Systems can communicate within subnetwork but not with other subnetworks. That's why it is more secured.
class A  has ip address ranging from 0.0.0.0 to 127.255.255.255 with subnet mask 255.0.0.0.
class B  has ip address ranging from 128.0.0.0 to 191.255.255.255 with subnet mask 255.255.0.0.
class C  has ip address ranging from 0.0.0.0 to 192.255.255.255 with subnet mask 255.255.255.0.

Nmap allows to scan network and discover everything connected to it. It also give information about what's connected, what services each host is operating, and so on. It gives detail of open ports , live host etc.

2) What is a firewall and mention its types. Use the NMAP command to detect that a firewall protects the host.

Firewalls monitor incoming and outgoing network traffic and allow/prohibit data packets based on a set of rules. Firewalls protect networks from external and malicious traffic and data packets while allowing legitimate traffic to pass through.

Types Of Firewalls

i)    packet-filtering Firewalls
ii)   Circuit-level Gateways
iii)  Application-level Gateways (Proxy Firewalls)
iv)   Stateful Multi-layer Inspection (SMLI) Firewalls
v)    Next-generation Firewalls (NGFW)
vi)   Threat-focused NGFW
vii)  Network Address Translation (NAT) Firewalls
viii) Cloud Firewalls
ix)   Unified Threat Management (UTM) Firewalls


3) bvhg

4)  What are vertical and horizontal scanning?

Horizontal scanning or network scanning sends requests to the same port on different hosts. Attackers use horizontal scanning to prepare for a mass attack. It is also scanning a group of IPs for a single ports.

Vertical scanning sends requests to different ports on the same host. Attackers use vertical scanning to look for vulnerabilities in a preselected target. It is also scanning single IP being scanned for multiple ports.



