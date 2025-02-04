Everyday page for Cisco routers and switches commands

**Cisco Router CLI Commands:**

| Command | Purpose |
|---------|---------|
| `enable` | Enter privileged EXEC mode |
| `configure terminal` | Enter global configuration mode |
| `show running-config` | Display the current running configuration |
| `show startup-config` | Display the saved configuration in NVRAM |
| `show ip interface brief` | Display summary of all interfaces and their status |
| `interface <interface>` | Enter interface configuration mode |
| `ip address <IP> <Subnet>` | Assign IP address to an interface |
| `no shutdown` | Enable an interface |
| `shutdown` | Disable an interface |
| `router ospf <ID>` | Enable OSPF routing protocol |
| `network <IP> <Wildcard> area <ID>` | Define OSPF network |
| `router bgp <AS>` | Enable BGP routing protocol |
| `neighbor <IP> remote-as <AS>` | Establish BGP neighbor |
| `show ip route` | Display routing table |
| `show ip protocols` | Display routing protocol information |
| `ping <IP>` | Test network connectivity |
| `traceroute <IP>` | Trace packet route |
| `reload` | Restart the router |
| `copy running-config startup-config` | Save the current configuration |
| `erase startup-config` | Delete the startup configuration |
| `show version` | Display system information |
| `show interfaces` | Display detailed interface information |
| `debug ip ospf events` | Debug OSPF events |
| `debug ip bgp` | Debug BGP events |
| `access-list <ID> permit/deny <IP>` | Configure access control lists (ACLs) |
| `show access-lists` | Display ACLs |
| `service password-encryption` | Encrypt all passwords |
| `hostname <NAME>` | Set router hostname |

---

**Cisco Switch CLI Commands:**

| Command | Purpose |
|---------|---------|
| `enable` | Enter privileged EXEC mode |
| `configure terminal` | Enter global configuration mode |
| `show running-config` | Display the current running configuration |
| `show startup-config` | Display the saved configuration in NVRAM |
| `show vlan brief` | Display VLAN information |
| `vlan <ID>` | Create a VLAN |
| `name <VLAN_NAME>` | Assign a name to VLAN |
| `interface vlan <ID>` | Enter VLAN interface mode |
| `ip address <IP> <Subnet>` | Assign IP address to VLAN interface |
| `interface <interface>` | Enter interface configuration mode |
| `switchport mode access` | Set interface to access mode |
| `switchport access vlan <ID>` | Assign VLAN to an access port |
| `switchport mode trunk` | Set interface to trunk mode |
| `switchport trunk allowed vlan <IDs>` | Define allowed VLANs on trunk |
| `show mac address-table` | Display MAC address table |
| `show interfaces status` | Display interface statuses |
| `spanning-tree mode <type>` | Enable spanning-tree protocol |
| `show spanning-tree` | Display spanning-tree status |
| `show port-security` | Display port security settings |
| `show interfaces trunk` | Display trunk port information |
| `reload` | Restart the switch |
| `copy running-config startup-config` | Save the current configuration |
| `erase startup-config` | Delete the startup configuration |
| `show cdp neighbors` | Display connected Cisco devices |
| `show power inline` | Display power consumption details |
| `interface range <start>-<end>` | Configure multiple interfaces at once |
| `spanning-tree portfast` | Enable PortFast on an interface |
| `switchport voice vlan <ID>` | Configure Voice VLAN on a port |
| `show interfaces counters` | Display interface statistics |
| `debug spanning-tree events` | Debug Spanning Tree events |


----

# Fortinet 

Here's a sheet of common Fortinet firewall CLI commands and their purposes:

| **Command**                          | **Purpose**                                                                 |
|--------------------------------------|-----------------------------------------------------------------------------|
| `get system status`                  | Displays system information (firmware version, uptime, etc.)                |
| `get system performance top`         | Shows real-time system performance (CPU, memory, etc.)                      |
| `show`                               | Displays the current configuration settings for various sections            |
| `config system global`               | Enter global configuration mode                                             |
| `config firewall policy`             | Configure firewall policies                                                 |
| `show firewall policy`               | Displays the current firewall policy configuration                          |
| `config system interface`            | Configure network interfaces                                                |
| `show system interface`              | Display network interface settings                                          |
| `diagnose debug enable`              | Enables debugging for troubleshooting                                       |
| `diagnose debug console timestamp enable` | Adds timestamp to debug output                                            |
| `diagnose firewall iprope lookup`    | Displays the connection table and packet statistics                         |
| `execute reboot`                     | Reboots the Fortinet device                                                 |
| `execute ping <IP address>`          | Pings a given IP address                                                   |
| `execute traceroute <IP address>`    | Traces the path packets take to a destination IP address                    |
| `config system time`                 | Configure system time and NTP settings                                      |
| `show system time`                   | Displays the current system time                                            |
| `config log disk setting`            | Configure log settings for disk storage                                     |
| `execute log filter`                 | Filters logs based on various parameters                                    |
| `diagnose sys top`                   | Shows a detailed top-like process display                                   |
| `show firewall address`              | Displays all defined address objects                                        |
| `config firewall address`            | Add or modify address objects for firewall rules                            |
| `show vpn ipsec phase1`              | Displays phase 1 of an IPSec VPN configuration                              |
| `config vpn ipsec phase1`            | Configure Phase 1 settings for IPSec VPN                                    |
| `execute factoryreset`               | Resets the device to factory settings                                       |
| `config system dns`                  | Configure DNS settings for the device                                       |
| `show system dns`                    | Displays current DNS settings                                               |
| `show system performance firewall`   | Displays firewall-specific performance statistics                           |

These are just a few of the common commands. Let me know if you need more!