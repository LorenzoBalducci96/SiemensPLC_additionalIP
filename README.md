# SiemensPLC_additionalIP
A set of plugins and doc for exposing a siemens PLC with a different IP address using a Windows based PC as IP forwarder

## USE CASE
You have a Siemens PLC without a CP (communication processor) which can have just 1 IP address.
You have an automation blocked-down network which does not allow changing of the IP address.
You want to expose the PLC to another network with a different IP address.

## REQUIREMENTS
The Network in which you want to expose the PLC with a different IP address is behind a windows based PC.

## NETWORK SETUP
![netowrk_architecture](https://user-images.githubusercontent.com/39745742/205751388-691a69a0-e2bd-4e86-b86e-c02bf9fbfffc.png)

## FUNCTIONS
1) MIM in the PROFINET DCP discovery packets, changing of the ip addresses in DCP packets (WinPcap application)
2) Port forwarding via netsh

(optional)
3) disabling icmp via windows firewall
4) reiplementation of ICMP (in winpcap application)
