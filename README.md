# DCCN_PacketTracer_Lab14
## Topology
![image](https://github.com/festerduck/DCCN_PacketTracer_Lab14/assets/117522051/45260bb2-c253-4b9d-ba99-c26649973c78)

## Creating New VLANS
~~~
enable
~~~
~~~
config terminal
~~~
~~~
vlan 10
~~~
~~~
name Voice
~~~
~~~
vlan 20
~~~
~~~
name Sales
~~~
## Now Setting Up the ports for each VLAN
For a single port in `switch(config`, select an interface to which the device is connected
~~~
interface fastEthernet 0/1
~~~
~~~
switchport mode access
~~~
~~~
switchport access vlan 10
~~~
For a multiple ports in `switch(config`, select ranges of interfaces to which the devices are connected
~~~
interface range fastEthernet 0/2 – 6
~~~
~~~
switchport mode access
~~~
~~~
switchport access vlan 20
~~~

Exit the VLAN config by `Ctrl + Z` 
To show the current VLANs
~~~
show VLAN
~~~
