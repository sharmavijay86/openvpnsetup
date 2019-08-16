# openvpnsetup
Note: this script works with centos 7 only..
Openvpn setup script. To install openvpn server in one click , use this bash script.
If you wants tun ip to be specific for each user session login then append bellow lines in file 
/etc/openvpn/server.conf 

client-to-client 
duplicate-cn 

-- if you wish to connect to home network also using this vpn server then uncomment bellow line 
#push "redirect-gateway def1 bypass-dhcp"

now add your home lan network route just bellow to above line.

push "route 192.168.1.1 255.255.255.0"

save and restart service.

Done!
