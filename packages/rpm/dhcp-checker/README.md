FIND DHCP SERVER IN NETWORK
====================================

==Install vagrant==
wget http://files.vagrantup.com/packages/7ec0ee1d00a916f80b109a298bab08e391945243/vagrant_1.2.7_x86_64.deb

dpkg -i vagrant_1.2.7_x86_64.deb

==Start Vagrant==
vagrant up

==Usage==
dhcpcheck --help - Print general usage about tool
dhcpcheck help discover - Print sspecific usage for every command

==Use cli==
DEFAULT TIMEOUT 5 sec
dhcpcheck discover --ifaces eth0 eth1 eth2
dhcpcheck discover --ifaces eth0 --timeout=10

==Usefull stuff==
Also you could make dhcpchecks from your host
dhcpcheck discover --ifaces vboxnet4

I sugest to look at trafic with wireshark or tcpdump writing to .pcap file

