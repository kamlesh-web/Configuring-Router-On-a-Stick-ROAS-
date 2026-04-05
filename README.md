## ROAS Overview
<img width="1366" height="768" alt="configuring ROAS Overview" src="https://github.com/user-attachments/assets/df316cca-fc55-4f44-bc9d-4c45cc910fba" />

---
## ROAS Configurations
    
    Router>
    Router>
    Router>enable
    Router#
    Router#configure terminal
    Enter configuration commands, one per line.  End with CNTL/Z.
    Router(config)#
    Router(config)#hostname router0
    router0(config)#
    router0(config)#enable secret CCNA
    router0(config)#
    router0(config)#interface g0/0/1
    router0(config-if)#
    router0(config-if)#interface g0/0/1.60
    router0(config-subif)#
    router0(config-subif)#encapsulation dot1q 60
    router0(config-subif)#
    router0(config-subif)#ip address 192.168.1.6 255.255.255.248
    router0(config-subif)#
    router0(config-subif)#interface g0/0/1.90
    router0(config-subif)#
    router0(config-subif)#encapsulation dot1q 90
    router0(config-subif)#
    router0(config-subif)#ip address 192.168.1.14 255.255.255.248
    router0(config-subif)#
    router0(config-subif)#interface g0/0/1.120
    router0(config-subif)#
    router0(config-subif)#encapsulation dot1q 120
    router0(config-subif)#
    router0(config-subif)#ip address 192.168.1.22 255.255.255.248
    router0(config-subif)#
    router0(config-subif)#interface g0/0/1.150
    router0(config-subif)#
    router0(config-subif)#encapsulation dot1q 150
    router0(config-subif)#
    router0(config-subif)#ip address 192.168.1.30 255.255.255.248
    router0(config-subif)#
    router0(config-subif)#exit
    router0(config)#
    router0(config)#interface g0/0/1
    router0(config-if)#
    router0(config-if)#no shutdown
    
    router0(config-if)#
    %LINK-5-CHANGED: Interface GigabitEthernet0/0/1, changed state to up
    
    %LINEPROTO-5-UPDOWN: Line protocol on Interface GigabitEthernet0/0/1, changed state to up
    
    %LINK-3-UPDOWN: Interface GigabitEthernet0/0/1.60, changed state to down
    
    %LINEPROTO-5-UPDOWN: Line protocol on Interface GigabitEthernet0/0/1.60, changed state to up
    
    %LINK-3-UPDOWN: Interface GigabitEthernet0/0/1.90, changed state to down
    
    %LINEPROTO-5-UPDOWN: Line protocol on Interface GigabitEthernet0/0/1.90, changed state to up
    
    %LINK-3-UPDOWN: Interface GigabitEthernet0/0/1.120, changed state to down
    
    %LINEPROTO-5-UPDOWN: Line protocol on Interface GigabitEthernet0/0/1.120, changed state to up
    
    %LINK-3-UPDOWN: Interface GigabitEthernet0/0/1.150, changed state to down
    
    %LINEPROTO-5-UPDOWN: Line protocol on Interface GigabitEthernet0/0/1.150, changed state to up
    
    router0(config-if)#
    router0(config-if)#end
    router0#
    %SYS-5-CONFIG_I: Configured from console by console
    
    router0#
    router0#write
    Building configuration...
    [OK]
    router0#
    router0#show ip interface brief
    Interface              IP-Address      OK? Method Status                Protocol 
    GigabitEthernet0/0/0   unassigned      YES unset  administratively down down 
    GigabitEthernet0/0/1   unassigned      YES unset  up                    up 
    GigabitEthernet0/0/1.60192.168.1.6     YES manual up                    up 
    GigabitEthernet0/0/1.90192.168.1.14    YES manual up                    up 
    GigabitEthernet0/0/1.120192.168.1.22    YES manual up                    up 
    GigabitEthernet0/0/1.150192.168.1.30    YES manual up                    up 
    GigabitEthernet0/0/2   unassigned      YES unset  administratively down down 
    Vlan1                  unassigned      YES unset  administratively down down
    router0#
---
## Ping Test
<img width="1366" height="768" alt="configuring ROAS 3" src="https://github.com/user-attachments/assets/43c5cb3f-376d-416e-b6de-9270c758c7ea" />
