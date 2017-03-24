# ansible-role-libvirtd
Ansible role for configuration of libvirtd

# TODO: Configure bridge (/etc/sysconfig/network-scripts/ifcfg-br0) from original interface eth0
DEVICE=br0
BOOTPROTO=static
IPADDR=188.165.238.61
NETMASK=255.255.255.0
ONBOOT=yes
GATEWAY=188.165.238.254
IPV6INIT=yes
IPV6_AUTOCONF=no
IPV6ADDR=2001:41d0:0002:b93d::/64
NM_CONTROLLED=no
TYPE=Bridge

# TODO: Reconfigure network eth0 (/etc/sysconfig/network-scripts/ifcfg-eth0)
DEVICE=eth0
BOOTPROTO=none
ONBOOT=yes
NM_CONTROLLED=no
BRIDGE=br0
TYPE=Ethernet

# TODO: Restart network and / or server
# TODO: Reconfigure dhcp range on virsh net-edit default (/etc/libvirtd/qemu/networks/default.xml)
# TODO: Additionally configure extra bridge (/etc/libvirtd/qemu/networks/public.xml)
# TODO: virsh net-define, autostart, start public
# TODO: Bring in ISO:  http://mirror.ox.ac.uk/sites/mirror.centos.org/7/isos/x86_64/CentOS-7-x86_64-Minimal-1611.iso


IN PROGRESS: http://www.smorgasbork.com/2014/07/16/building-a-custom-centos-7-kickstart-disc-part-3/
