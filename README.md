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

Gotcha, baby. Here’s a more in-depth list of Fortinet CLI commands, especially useful for troubleshooting network, firewall, and VPN issues.  

---

## 🔹 **System & Performance Troubleshooting**  
| **Command**                               | **Purpose** |
|-------------------------------------------|-------------|
| `get system status`                       | Displays system info (firmware, uptime, etc.) |
| `get system performance status`           | Shows CPU & memory usage |
| `diagnose sys top`                        | Displays running processes & CPU usage |
| `diagnose sys process pidof <process>`    | Gets the PID of a specific process |
| `diagnose sys kill 11 <PID>`              | Kills a process (useful if something is stuck) |
| `diagnose hardware deviceinfo nic <int>`  | Shows details of an interface (speed, errors) |
| `get system interface physical`           | Displays all physical interfaces and their status |
| `execute ping-options repeat-count <num>` | Sets the number of pings before running `execute ping` |

---

## 🔹 **Network Connectivity & Packet Flow**  
| **Command**                                      | **Purpose** |
|--------------------------------------------------|-------------|
| `execute ping <IP>`                             | Tests connectivity to an IP |
| `execute traceroute <IP>`                       | Shows the path packets take to reach an IP |
| `diagnose ip address list`                      | Displays assigned IP addresses |
| `diagnose netlink interface list`               | Lists interfaces and their link status |
| `diagnose netlink neighbor list`                | Shows ARP table (connected devices) |
| `diagnose netlink route list`                   | Displays routing table |
| `diagnose firewall proute list`                 | Lists policy routes |
| `diagnose ip route get <IP>`                    | Shows the route used for a specific IP |
| `diagnose sniffer packet <interface> ‘host <IP>’` | Captures live traffic on an interface |
| `diagnose sniffer packet any ‘host <IP> and port 443’` | Captures HTTPS traffic from/to an IP |
| `execute tcpdump -i <interface> -nnn`           | Captures raw packets (alternative to `sniffer packet`) |

---

## 🔹 **Firewall & Security Troubleshooting**  
| **Command**                                      | **Purpose** |
|--------------------------------------------------|-------------|
| `diagnose debug enable`                         | Enables debugging mode |
| `diagnose debug console timestamp enable`       | Adds timestamps to debug logs |
| `diagnose debug application <process> <level>`  | Debugs a specific service (e.g., `ike`, `wad`, `dnsproxy`) |
| `diagnose firewall iprope show`                 | Displays firewall policy lookup results |
| `diagnose firewall iprope lookup <int> <src-IP> <dst-IP> <protocol> <port>` | Checks if a firewall policy allows a connection |
| `diagnose sys session list`                     | Displays current active sessions |
| `diagnose sys session filter clear`             | Clears filters for session monitoring |
| `diagnose sys session filter src <IP>`          | Filters session list by source IP |
| `diagnose sys session filter dst <IP>`          | Filters session list by destination IP |
| `diagnose sys session clear`                    | Clears all active sessions |
| `get router info routing-table all`             | Displays all routing information |
| `diagnose firewall policy list`                 | Displays all firewall rules |
| `diagnose firewall auth list`                   | Shows authenticated users |
| `diagnose user device list`                     | Lists devices connected to the network |
| `diagnose firewall fqdn list`                   | Displays cached FQDN entries used in policies |

---

## 🔹 **VPN Troubleshooting (IPsec & SSL VPN)**  
| **Command**                                      | **Purpose** |
|--------------------------------------------------|-------------|
| `diagnose vpn ike gateway list`                 | Displays active IKE gateways (phase 1) |
| `diagnose vpn ike log-filter dst-addr4 <IP>`    | Filters logs for a specific VPN peer |
| `diagnose vpn ike log-filter src-addr4 <IP>`    | Filters logs for a specific source |
| `diagnose vpn ike log-filter clear`             | Clears all VPN log filters |
| `diagnose debug application ike -1`             | Enables verbose IKE debugging |
| `diagnose debug application sslvpn -1`          | Enables SSL VPN debugging |
| `diagnose vpn tunnel list`                      | Shows active IPsec tunnels and their status |
| `diagnose vpn tunnel flush <name>`              | Resets an IPsec tunnel |
| `diagnose debug enable`                         | Enables debug mode |
| `diagnose debug console timestamp enable`       | Adds timestamps to debug logs |
| `diagnose debug disable`                        | Disables debugging |
| `diagnose debug reset`                          | Resets debug settings |

---

## 🔹 **Logs & Diagnostics**  
| **Command**                                      | **Purpose** |
|--------------------------------------------------|-------------|
| `execute log filter category <category>`        | Filters logs by category (e.g., `vpn`, `traffic`, `system`) |
| `execute log display`                           | Displays logs based on the filter set |
| `diagnose log test`                             | Tests log functionality |
| `execute log filter reset`                      | Clears log filters |
| `diagnose log config`                           | Shows logging configuration |
| `execute log disk read <number>`                | Reads the last X log entries from disk |
| `execute log delete`                            | Clears all logs |

---

## 🔹 **High Availability (HA) Troubleshooting**  
| **Command**                                      | **Purpose** |
|--------------------------------------------------|-------------|
| `get system ha status`                          | Shows HA status (primary/secondary) |
| `diagnose sys ha checksum`                      | Compares HA configs for mismatches |
| `diagnose sys ha dump-by vcluster`              | Displays HA synchronization status |
| `diagnose sys ha reset-stats`                   | Resets HA statistics |
| `diagnose sys ha show | grep <keyword>`         | Filters HA details for easier troubleshooting |

---
