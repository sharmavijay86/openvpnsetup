# openvpnsetup
Openvpn setup script. To install openvpn server in one click , use this bash script.
If you wants tun ip to be specific for each user session login then append bellow lines in file 
/etc/openvpn/server.conf 

client-to-client 
duplicate-cn 
