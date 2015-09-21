# difference_bridge-NAT

### Bridge Network

* Used in environments where virtual machines provide services or participate in a real network.
* Connects virtual machines to the Local Area Network (LAN) of their host machine, whether wired or wireless.
* Allows them to connect to any other host or virtual machines (if they are also bridged) on the network.
* Connects the virtual network adapter in a virtual machine to the physical Ethernet adapter in its host machine.
* You can establish additional virtual bridges to use in custom configurations that require connections to more than one physical Ethernet adapter on the host computer.
* The default network adapter interface is vmnet0

### NAT (Network Address Translation) Network

* Used in environments where virtual machines do not provide services but still need to access a network.
* Connects virtual machines to an external network, using the host machines IP address for external communication.
* Connects virtual machines to the Internet through their host machines dial-up connection, Ethernet adapter or wireless Ethernet adapter.
* Connects virtual machines to a non-Ethernet network, such as Token Ring or ATM.
* Establishes a private LAN shared only by your host machine and any other virtual machines also using NAT networking
* .Other host machines on the host LAN can communicate with the virtual machines, however external host machines cannot initiate communication with virtual machines unless NAT port forwarding is also in use.
* NAT port forwarding causes network traffic destined for a port on a host machine to be forwarded to a specific port on a virtual machine.
* The default network adapter interface is vmnet8.
