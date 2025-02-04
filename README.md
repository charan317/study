# study
Everyday Study page

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

This sheet covers the most essential Cisco CLI commands for routers and switches!

