# SYS-255-Spring-
github for labs 

LAB-01 Notes:
Addresses
DNS - 10..0.5.2 
Default Gateway - 10.0.5.2
IP wks-01 - 10.0.5.100
Subnet mask - 255.255.255.0

Command for Tracert - "tracert -h 3 champlain.edu"
Default gateway: A default gateway connects the host to the internet; it serves as an access point for outbound connections. Lets two different computers communicate on different networks. 

--------------

LAB-02 Notes 

ad01-hayden
HAYDEN/Administrator pw:Dun******
Uncheck update/ptr record can help troubleshoot 
fw01-hayden.blaisdell.local = 10.0.5.2
ad01-hayden.blaisdell.local = 10.0.5.5

LAB-03 Notes 

For powershell to get pass 10 record the command is "history | head -10"
IP for dhcp01-hayden - 10.0.5.3
On linux ping make sure to include -c 1 to be able to control amount of packets transmitted 
Note to self: always rember to hostame in powerhsell to rember what user you are logged in as. 


Linux HW: 

Process for setting a static IP:

1. First create a network script file for eth0 or use nmtui
2. Specify server IP Ex: IPADDR = 192.168.2.216
3. Set default gateway IP Ex: 192.168.2.254
4. Set DNS servers 
5. Make sure IPV6 is dissabled 
6. Restart network by the Command: systemctl restart network


New User Command: 

adduser newuser

passwd newuser 

Tree Command displays all users on machine 

The Command Whoami displays the user that is CURRENTLY logged into the machine.



LAB 0-4: 

on wks01 make sure to renew ip "ipconfig /renew

make sure to release after "ipconfig /release"

Set wks01 to dynamic istead of static:
1.control panel 
2.ethernet 
3.check circles to "obtian" 

after dhcp set up reload fire wall settings:
1. firewall-cmd --add-service=dhcp --permanent 
2. firewall-cmd --list-all

Note to self: systemctl reload, systemctl start dhcpd, systemctle enable dhcpd 




