# VLAN-Configuration-for-Cisco-Switch-with-IP-Routing
This configuration sets up four VLANs (AA, BB, CC, DD) on a Cisco switch, assigns them specific IP addresses, and enables inter-VLAN routing. It includes the configuration of access ports and routing protocols to ensure smooth communication between different VLANs.
# Cisco Switch VLAN Configuration

This project demonstrates the configuration of VLANs and IP addresses on a Cisco switch. The switch is divided into four VLANs (AA, BB, CC, DD), with each VLAN assigned to specific interfaces. Additionally, the switch has IP addresses configured for each VLAN interface.

## VLANs and IP Configuration
- **VLAN 10 (AA)**: 192.168.1.62/26
- **VLAN 20 (BB)**: 192.168.1.126/26
- **VLAN 30 (CC)**: 192.168.1.190/26
- **VLAN 40 (DD)**: 192.168.1.254/26

### Interfaces and VLAN Assignment:
- **Fa0/1-2**: Assigned to VLAN 10
- **Fa0/3-4**: Assigned to VLAN 20
- **Fa0/5-6**: Assigned to VLAN 30
- **Fa0/7-8**: Assigned to VLAN 40

### Configuration Steps:
1. **Define VLANs**: Four VLANs (10, 20, 30, 40) are created and named as AA, BB, CC, and DD respectively.
2. **Assign Interfaces**: Access ports on FastEthernet ports (Fa0/1 to Fa0/8) are assigned to the respective VLANs.
3. **Assign IP Addresses**: Each VLAN interface (SVI) is configured with an IP address within the subnet.
4. **Enable Routing**: IP routing is enabled for inter-VLAN communication.

### Commands Used:
- `vlan`: Creates and names VLANs.
- `interface range`: Configures multiple interfaces at once.
- `switchport mode access`: Sets the port as an access port.
- `ip address`: Assigns an IP address to the VLAN interface.
- `ip routing`: Enables routing between VLANs.

## Requirements:
- Cisco Switch with IOS that supports VLANs and routing.

## How to Use:
1. Connect to the Cisco switch via console cable.
2. Enter global configuration mode by typing `conf t`.
3. Copy and paste the provided configuration commands.
4. Save the configuration with `write memory`.

