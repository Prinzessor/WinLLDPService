# My modification notes

- Forked from: https://github.com/raspi/WinLLDPService
- Forked from: https://github.com/jftuga/WinLLDPService

- Example output
```
   net# sho lldp info remote-device B5
    
     LLDP Remote Device Information Detail
    
      Local Port   : B5
      ChassisType  : mac-address
      ChassisId    : c4 31 2b 7a 0a 11
      PortType     : mac-address
      PortId       : c4 31 2b 7a 0a 11
------------------------------------------------------------------------------
    Local Port   : B5
    ChassisType  : mac-address
    ChassisId    : c4 31 2b 7a 0a 11
    PortType     : local
    PortId       : Ethernet
    SysName      : FQDN
    System Descr : OS:'Win 10 Ent',Up:'27.04:08'
    PortDescr    : GW:'192.168.25.1',NM:'24',DHCP:'192.168.25.2',Spd:'1Gbps'

     Remote Management Address
     Type    : ipv4
     Address : 192.168.25.67
     
```
- Removed Usr from Description
- Changed SysName from NETBIOS Hostname to FQDN


# Download

- You can use the *WinLLDPService-installer.msi* package listed above in WinLLDPService/build/


--------------------------------------------------------------------------

# Original README.md

--------------------------------------------------------------------------

# WinLLDPService

Small LLDP Windows Service. 

Used by network switches to list network devices - https://en.wikipedia.org/wiki/Link_Layer_Discovery_Protocol

Sends LLDP packets to switch. Switch must have LLDP capability. It **doesn't** query switches' internal LLDP data. Errors are logged to Windows Event Log.

See homepage for more information and download `.msi` installer.

# Developing

See `WinLLDPService` directory.

# License
MIT

