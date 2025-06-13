# RELATÓRIO PROVA B2
**Professor:** João Gress  
**Curso:** Bacharelado em Sistemas de Informação – 5º Semestre  - IESGO

---
# Comandosdo swtich principal 3560
```bash

Switch>enable
Switch#configure terminal
Enter configuration commands, one per line.  End with CNTL/Z.
Switch(config)#vlan 10
Switch(config-vlan)#name Administracao
Switch(config-vlan)#interface vlan 10
Switch(config-if)#
%LINK-5-CHANGED: Interface Vlan10, changed state to up
ip address 192.168.10.1 255.255.255.0
Switch(config-if)#no shutdown
Switch(config-if)#exit
Switch(config)#vlan 20
Switch(config-vlan)#name Financeiro
Switch(config-vlan)#interface vlan 20
Switch(config-if)#
%LINK-5-CHANGED: Interface Vlan20, changed state to up
ip address 192.168.20.1 255.255.255.0
Switch(config-if)#no shutdown
Switch(config-if)#exit
Switch(config)#vlan 30
Switch(config-vlan)#name RH
Switch(config-vlan)#interface vlan 30
Switch(config-if)#
%LINK-5-CHANGED: Interface Vlan30, changed state to up
ip address 192.168.30.1 255.255.255.0
Switch(config-if)#no shutdown
Switch(config-if)#exit
Switch(config)#vlan 40
Switch(config-vlan)#name TI
Switch(config-vlan)#interface vlan 40
Switch(config-if)#
%LINK-5-CHANGED: Interface Vlan40, changed state to up
ip address 192.168.40.1 255.255.255.0
Switch(config-if)#no shutdown
Switch(config-if)#exit
Switch(config)#vlan 50
Switch(config-vlan)#name Suporte_Tecnico
Switch(config-vlan)#interface vlan 50
Switch(config-if)#
%LINK-5-CHANGED: Interface Vlan50, changed state to up
ip address 192.168.50.1 255.255.255.0
Switch(config-if)#no shutdown
Switch(config-if)#exit
Switch(config)#vlan 60
Switch(config-vlan)#name Gerencia
Switch(config-vlan)#interface vlan 60
Switch(config-if)#
%LINK-5-CHANGED: Interface Vlan60, changed state to up
ip address 192.168.60.1 255.255.255.0
Switch(config-if)#no shutdown
Switch(config-if)#exit
Switch(config)#vlan 70
Switch(config-vlan)#name Visitantes
Switch(config-vlan)#interface vlan 70
Switch(config-if)#
%LINK-5-CHANGED: Interface Vlan70, changed state to up
ip address 192.168.70.1 255.255.255.0
Switch(config-if)#no shutdown
Switch(config-if)#exit
Switch(config)#vlan 99
Switch(config-vlan)#name Servidores
Switch(config-vlan)#interface vlan 99
Switch(config-if)#
%LINK-5-CHANGED: Interface Vlan99, changed state to up
ip address 192.168.99.1 255.255.255.0
Switch(config-if)#no shutdown
Switch(config-if)#exit
Switch(config)#ip routing
Switch(config)#interface range fa0/1 - 3
Switch(config-if-range)#switchport mode access
Switch(config-if-range)#switchport access vlan 99
Switch(config-if-range)#
%LINEPROTO-5-UPDOWN: Line protocol on Interface Vlan99, changed state to up

Switch(config-if-range)#exit
Switch(config)#interface fa0/5
Switch(config-if)#switchport trunk encapsulation dot1q
Switch(config-if)#switchport mode trunk

Switch(config-if)#
%LINEPROTO-5-UPDOWN: Line protocol on Interface FastEthernet0/5, changed state to down

%LINEPROTO-5-UPDOWN: Line protocol on Interface FastEthernet0/5, changed state to up

%LINEPROTO-5-UPDOWN: Line protocol on Interface Vlan10, changed state to up

%LINEPROTO-5-UPDOWN: Line protocol on Interface Vlan20, changed state to up

%LINEPROTO-5-UPDOWN: Line protocol on Interface Vlan30, changed state to up

%LINEPROTO-5-UPDOWN: Line protocol on Interface Vlan40, changed state to up

%LINEPROTO-5-UPDOWN: Line protocol on Interface Vlan50, changed state to up

%LINEPROTO-5-UPDOWN: Line protocol on Interface Vlan60, changed state to up

%LINEPROTO-5-UPDOWN: Line protocol on Interface Vlan70, changed state to up
exit
Switch(config)#write memory
               ^
% Invalid input detected at '^' marker.
	
Switch(config)#exit
Switch#
%SYS-5-CONFIG_I: Configured from console by console
write memory
Building configuration...
[OK]
Switch#show vlan brief

VLAN Name                             Status    Ports
---- -------------------------------- --------- -------------------------------
1    default                          active    Fa0/4, Fa0/6, Fa0/7, Fa0/8
                                                Fa0/9, Fa0/10, Fa0/11, Fa0/12
                                                Fa0/13, Fa0/14, Fa0/15, Fa0/16
                                                Fa0/17, Fa0/18, Fa0/19, Fa0/20
                                                Fa0/21, Fa0/22, Fa0/23, Fa0/24
                                                Gig0/1, Gig0/2
10   Administracao                    active    
20   Financeiro                       active    
30   RH                               active    
40   TI                               active    
50   Suporte_Tecnico                  active    
60   Gerencia                         active    
70   Visitantes                       active    
99   Servidores                       active    Fa0/1, Fa0/2, Fa0/3
1002 fddi-default                     active    
1003 token-ring-default               active    
1004 fddinet-default                  active    
1005 trnet-default                    active    
Switch#show vlan

VLAN Name                             Status    Ports
---- -------------------------------- --------- -------------------------------
1    default                          active    Fa0/4, Fa0/6, Fa0/7, Fa0/8
                                                Fa0/9, Fa0/10, Fa0/11, Fa0/12
                                                Fa0/13, Fa0/14, Fa0/15, Fa0/16
                                                Fa0/17, Fa0/18, Fa0/19, Fa0/20
                                                Fa0/21, Fa0/22, Fa0/23, Fa0/24
                                                Gig0/1, Gig0/2
10   Administracao                    active    
20   Financeiro                       active    
30   RH                               active    
40   TI                               active    
50   Suporte_Tecnico                  active    
60   Gerencia                         active    
70   Visitantes                       active    
99   Servidores                       active    Fa0/1, Fa0/2, Fa0/3
1002 fddi-default                     active    
1003 token-ring-default               active    
1004 fddinet-default                  active    
1005 trnet-default                    active    

 --More-- 
```


# Comandos das vlans 10 a 70
---

## vlan ADMINITRAÇÃO

```bash 

Switch(config-if)#switchport mode trunk
Switch(config-if)#no shutdown
Switch(config-if)#exit
Switch(config)#interface range fa0/2 - 7
Switch(config-if-range)#switchport mode access
Switch(config-if-range)#switchport access vlan 10
% Access VLAN does not exist. Creating vlan 10
Switch(config-if-range)#no shutdown
Switch(config-if-range)#exit
Switch(config)#interface fa0/1
Switch(config-if)#switchport mode trunk
Switch(config-if)#no shutdown
Switch(config-if)#exit
Switch(config)#interface range fa0/2 - 7
Switch(config-if-range)#switchport mode access
Switch(config-if-range)#switchport access vlan 10
Switch(config-if-range)#no shutdown
Switch(config-if-range)#exit
Switch(config)#write memory
               ^
% Invalid input detected at '^' marker.
	
Switch(config)#exit
Switch#
%SYS-5-CONFIG_I: Configured from console by console
write memory
Building configuration...
[OK]
Switch#
Switch#configure terminal
Enter configuration commands, one per line.  End with CNTL/Z.
Switch(config)#vlan 10
Switch(config-vlan)#name Administracao
Switch(config-vlan)#exit
Switch(config)#exit
Switch#
%SYS-5-CONFIG_I: Configured from console by console
write memory
Building configuration...
[OK]
Switch#

```
---
## vlan FINANCEIRO
---
```bash

Switch>enable
Switch#configure terminal
Enter configuration commands, one per line.  End with CNTL/Z.
Switch(config)#interface fa0/1
Switch(config-if)#switchport mode trunk
Switch(config-if)#no shutdown
Switch(config-if)#exit
Switch(config)#interface range fa0/2 - 5
Switch(config-if-range)#switchport mode access
Switch(config-if-range)#switchport access vlan 20
% Access VLAN does not exist. Creating vlan 20
Switch(config-if-range)#no shutdown
Switch(config-if-range)#exit
Switch(config)#exit
Switch#
%SYS-5-CONFIG_I: Configured from console by console

Switch#configure terminal
Enter configuration commands, one per line.  End with CNTL/Z.
Switch(config)#vlan 20
Switch(config-vlan)#name Financeiro
Switch(config-vlan)#exit
Switch(config)#exit
Switch#
%SYS-5-CONFIG_I: Configured from console by console
write memory
Building configuration...
[OK]
Switch#

```
---
RH## vlan RH
---
```bash
Switch>enable
Switch#configure terminal
Enter configuration commands, one per line.  End with CNTL/Z.
Switch(config)#interface fa0/1
Switch(config-if)#switchport mode trunk
Switch(config-if)#no shutdown
Switch(config-if)#exit
Switch(config)#vlan 10
Switch(config-vlan)#name RH
Switch(config-vlan)#exit
Switch(config)#interface range fa0/2 - 4
Switch(config-if-range)#switchport mode access
Switch(config-if-range)#switchport access vlan 30
% Access VLAN does not exist. Creating vlan 30
Switch(config-if-range)#no shutdown
Switch(config-if-range)#exit
Switch(config)#exit
Switch#
%SYS-5-CONFIG_I: Configured from console by console
write memory
Building configuration...
[OK]
``` 
---
## vlan TI
---
```bash
Switch>enable 
Switch#configure terminal
Enter configuration commands, one per line.  End with CNTL/Z.
Switch(config)#enable
% Incomplete command.
Switch(config)#vlan 40
Switch(config-vlan)#name TI
Switch(config-vlan)#EXIT
Switch(config)#interface fa0/1
Switch(config-if)#switchport mode trunk
Switch(config-if)#
Switch(config-if)#no shutdown
Switch(config-if)#exit
Switch(config)#
Switch(config)#interface range fa0/2 - 9
Switch(config-if-range)#switchport mode access
Switch(config-if-range)#switchport mode access
Switch(config-if-range)#switchport access vlan 40
Switch(config-if-range)#no shutdown
Switch(config-if-range)#exit
Switch(config)#exit
Switch#
%SYS-5-CONFIG_I: Configured from console by console
write memory
Building configuration...
[OK]
```
---
## vlan SUPORTE_TECNICO
---
```bash 
Switch(config)#vlan 50
Switch(config-vlan)#name Suporte_Tecnico
Switch(config-vlan)#interface fa0/1
Switch(config-if)#switchport mode trunk
Switch(config-if)#no shutdown
Switch(config-if)#exit
Switch(config)#interface range fa0/2 - 4
Switch(config-if-range)#switchport mode access
Switch(config-if-range)#switchport access vlan 50
Switch(config-if-range)#no shutdown
Switch(config-if-range)#exit
Switch(config)#exit
Switch#
%SYS-5-CONFIG_I: Configured from console by console
write memory
Building configuration...
[OK]
Switch#
```
---
## vlan Gerencia
---
```bash
Switch>enable
Switch#configure terminal
Enter configuration commands, one per line.  End with CNTL/Z.
Switch(config)#vlan 60
Switch(config-vlan)#name Gerencia
Switch(config-vlan)#interface fa0/1
Switch(config-if)#switchport mode trunk
Switch(config-if)#no shutdown
Switch(config-if)#exit
Switch(config)#interface range fa0/2 - 3
Switch(config-if-range)#switchport mode access
Switch(config-if-range)#switchport access vlan 60
Switch(config-if-range)#no shutdown
Switch(config-if-range)#exit
Switch(config)#write memory
               ^
% Invalid input detected at '^' marker.
	
Switch(config)#exit
Switch#
%SYS-5-CONFIG_I: Configured from console by console
write memory
Building configuration...
[OK]
Switch#
```

------------------------
# Fazendo segurança da rede

## desabilitando portas e especificando MAC
---
## 2960 FIN
```bash
Switch>enable
Switch#configure terminal
Enter configuration commands, one per line.  End with CNTL/Z.
Switch(config)#interface range fa0/2 - 7
Switch(config-if-range)#switchport port-security
Switch(config-if-range)#switchport port-security maximum 1
Switch(config-if-range)#switchport port-security violation shutdown
Switch(config-if-range)#switchport port-security mac-address sticky
Switch(config-if-range)#exit
Switch(config)#interface range fa0/8 - 24
Switch(config-if-range)#shutdown

%LINK-5-CHANGED: Interface FastEthernet0/8, changed state to administratively down

%LINK-5-CHANGED: Interface FastEthernet0/9, changed state to administratively down

%LINK-5-CHANGED: Interface FastEthernet0/10, changed state to administratively down

%LINK-5-CHANGED: Interface FastEthernet0/11, changed state to administratively down

%LINK-5-CHANGED: Interface FastEthernet0/12, changed state to administratively down

%LINK-5-CHANGED: Interface FastEthernet0/13, changed state to administratively down

%LINK-5-CHANGED: Interface FastEthernet0/14, changed state to administratively down

%LINK-5-CHANGED: Interface FastEthernet0/15, changed state to administratively down

%LINK-5-CHANGED: Interface FastEthernet0/16, changed state to administratively down

%LINK-5-CHANGED: Interface FastEthernet0/17, changed state to administratively down

%LINK-5-CHANGED: Interface FastEthernet0/18, changed state to administratively down

%LINK-5-CHANGED: Interface FastEthernet0/19, changed state to administratively down

%LINK-5-CHANGED: Interface FastEthernet0/20, changed state to administratively down

%LINK-5-CHANGED: Interface FastEthernet0/21, changed state to administratively down

%LINK-5-CHANGED: Interface FastEthernet0/22, changed state to administratively down

%LINK-5-CHANGED: Interface FastEthernet0/23, changed state to administratively down

%LINK-5-CHANGED: Interface FastEthernet0/24, changed state to administratively down
Switch(config-if-range)#exit
Switch(config)#exit
Switch#
%SYS-5-CONFIG_I: Configured from console by console
write memory
Building configuration...
[OK]
```
---
## 2960 ADM
---
```bash

Switch>enable
Switch#enable
Switch#configure terminal
Enter configuration commands, one per line.  End with CNTL/Z.
Switch(config)#interface range fa0/2 - 5
Switch(config-if-range)#
Switch(config-if-range)# switchport port-security
Switch(config-if-range)#switchport port-security
Switch(config-if-range)#switchport port-security maximum 1
Switch(config-if-range)#switchport port-security violation shutdown
Switch(config-if-range)#switchport port-security mac-address sticky
Switch(config-if-range)#exit
Switch(config)#interface range fa0/6 - 24
Switch(config-if-range)#shutdown

%LINK-5-CHANGED: Interface FastEthernet0/6, changed state to administratively down

%LINK-5-CHANGED: Interface FastEthernet0/7, changed state to administratively down

%LINK-5-CHANGED: Interface FastEthernet0/8, changed state to administratively down

%LINK-5-CHANGED: Interface FastEthernet0/9, changed state to administratively down

%LINK-5-CHANGED: Interface FastEthernet0/10, changed state to administratively down

%LINK-5-CHANGED: Interface FastEthernet0/11, changed state to administratively down

%LINK-5-CHANGED: Interface FastEthernet0/12, changed state to administratively down

%LINK-5-CHANGED: Interface FastEthernet0/13, changed state to administratively down

%LINK-5-CHANGED: Interface FastEthernet0/14, changed state to administratively down

%LINK-5-CHANGED: Interface FastEthernet0/15, changed state to administratively down

%LINK-5-CHANGED: Interface FastEthernet0/16, changed state to administratively down

%LINK-5-CHANGED: Interface FastEthernet0/17, changed state to administratively down

%LINK-5-CHANGED: Interface FastEthernet0/18, changed state to administratively down

%LINK-5-CHANGED: Interface FastEthernet0/19, changed state to administratively down

%LINK-5-CHANGED: Interface FastEthernet0/20, changed state to administratively down

%LINK-5-CHANGED: Interface FastEthernet0/21, changed state to administratively down

%LINK-5-CHANGED: Interface FastEthernet0/22, changed state to administratively down

%LINK-5-CHANGED: Interface FastEthernet0/23, changed state to administratively down

%LINK-5-CHANGED: Interface FastEthernet0/24, changed state to administratively down
Switch(config-if-range)#exit
Switch(config)#exit
Switch#
%SYS-5-CONFIG_I: Configured from console by console
write memory
Building configuration...
[OK]
Switch#
```
---
## 2960 RH
---
```bash
Switch>enable
Switch#configure terminal
Enter configuration commands, one per line.  End with CNTL/Z.
Switch(config)#interface range fa0/2 - 4
Switch(config-if-range)#switchport port-security
Switch(config-if-range)#switchport port-security maximum 1
Switch(config-if-range)#switchport port-security violation shutdown
Switch(config-if-range)#switchport port-security mac-address sticky
Switch(config-if-range)#exit
Switch(config)#interface range fa0/5 - 24
Switch(config-if-range)#shutdown

%LINK-5-CHANGED: Interface FastEthernet0/5, changed state to administratively down

%LINK-5-CHANGED: Interface FastEthernet0/6, changed state to administratively down

%LINK-5-CHANGED: Interface FastEthernet0/7, changed state to administratively down

%LINK-5-CHANGED: Interface FastEthernet0/8, changed state to administratively down

%LINK-5-CHANGED: Interface FastEthernet0/9, changed state to administratively down

%LINK-5-CHANGED: Interface FastEthernet0/10, changed state to administratively down

%LINK-5-CHANGED: Interface FastEthernet0/11, changed state to administratively down

%LINK-5-CHANGED: Interface FastEthernet0/12, changed state to administratively down

%LINK-5-CHANGED: Interface FastEthernet0/13, changed state to administratively down

%LINK-5-CHANGED: Interface FastEthernet0/14, changed state to administratively down

%LINK-5-CHANGED: Interface FastEthernet0/15, changed state to administratively down

%LINK-5-CHANGED: Interface FastEthernet0/16, changed state to administratively down

%LINK-5-CHANGED: Interface FastEthernet0/17, changed state to administratively down

%LINK-5-CHANGED: Interface FastEthernet0/18, changed state to administratively down

%LINK-5-CHANGED: Interface FastEthernet0/19, changed state to administratively down

%LINK-5-CHANGED: Interface FastEthernet0/20, changed state to administratively down

%LINK-5-CHANGED: Interface FastEthernet0/21, changed state to administratively down

%LINK-5-CHANGED: Interface FastEthernet0/22, changed state to administratively down

%LINK-5-CHANGED: Interface FastEthernet0/23, changed state to administratively down

%LINK-5-CHANGED: Interface FastEthernet0/24, changed state to administratively down
Switch(config-if-range)#exit
Switch(config)#exit
Switch#
%SYS-5-CONFIG_I: Configured from console by console
write memory
Building configuration...
[OK]

```
---
## 2960 TI
---
```bash
Switch>enable
Switch#configure terminal
Enter configuration commands, one per line.  End with CNTL/Z.
Switch(config)#interface range fa0/2 - 9
Switch(config-if-range)#switchport port-security
Switch(config-if-range)#switchport port-security maximum 1
Switch(config-if-range)#switchport port-security violation shutdown
Switch(config-if-range)#switchport port-security mac-address sticky
Switch(config-if-range)#exit
Switch(config)#interface range fa0/10 - 24
Switch(config-if-range)#shutdown

%LINK-5-CHANGED: Interface FastEthernet0/10, changed state to administratively down

%LINK-5-CHANGED: Interface FastEthernet0/11, changed state to administratively down

%LINK-5-CHANGED: Interface FastEthernet0/12, changed state to administratively down

%LINK-5-CHANGED: Interface FastEthernet0/13, changed state to administratively down

%LINK-5-CHANGED: Interface FastEthernet0/14, changed state to administratively down

%LINK-5-CHANGED: Interface FastEthernet0/15, changed state to administratively down

%LINK-5-CHANGED: Interface FastEthernet0/16, changed state to administratively down

%LINK-5-CHANGED: Interface FastEthernet0/17, changed state to administratively down

%LINK-5-CHANGED: Interface FastEthernet0/18, changed state to administratively down

%LINK-5-CHANGED: Interface FastEthernet0/19, changed state to administratively down

%LINK-5-CHANGED: Interface FastEthernet0/20, changed state to administratively down

%LINK-5-CHANGED: Interface FastEthernet0/21, changed state to administratively down

%LINK-5-CHANGED: Interface FastEthernet0/22, changed state to administratively down

%LINK-5-CHANGED: Interface FastEthernet0/23, changed state to administratively down

%LINK-5-CHANGED: Interface FastEthernet0/24, changed state to administratively down
Switch(config-if-range)#exit
Switch(config)#exit
Switch#
%SYS-5-CONFIG_I: Configured from console by console
write memory
Building configuration...
[OK]
Switch#

```
---
## 2960 SUPORTE_TECNICO
---
```bash

Switch>enable
Switch#configure terminal
Enter configuration commands, one per line.  End with CNTL/Z.
Switch(config)#interface range fa0/2 - 4
Switch(config-if-range)#switchport port-security
Switch(config-if-range)#switchport port-security maximum 1
Switch(config-if-range)#switchport port-security violation shutdown
Switch(config-if-range)#switchport port-security mac-address sticky
Switch(config-if-range)#exit
Switch(config)#interface range fa0/5 - 24
Switch(config-if-range)#shutdown

%LINK-5-CHANGED: Interface FastEthernet0/5, changed state to administratively down

%LINK-5-CHANGED: Interface FastEthernet0/6, changed state to administratively down

%LINK-5-CHANGED: Interface FastEthernet0/7, changed state to administratively down

%LINK-5-CHANGED: Interface FastEthernet0/8, changed state to administratively down

%LINK-5-CHANGED: Interface FastEthernet0/9, changed state to administratively down

%LINK-5-CHANGED: Interface FastEthernet0/10, changed state to administratively down

%LINK-5-CHANGED: Interface FastEthernet0/11, changed state to administratively down

%LINK-5-CHANGED: Interface FastEthernet0/12, changed state to administratively down

%LINK-5-CHANGED: Interface FastEthernet0/13, changed state to administratively down

%LINK-5-CHANGED: Interface FastEthernet0/14, changed state to administratively down

%LINK-5-CHANGED: Interface FastEthernet0/15, changed state to administratively down

%LINK-5-CHANGED: Interface FastEthernet0/16, changed state to administratively down

%LINK-5-CHANGED: Interface FastEthernet0/17, changed state to administratively down

%LINK-5-CHANGED: Interface FastEthernet0/18, changed state to administratively down

%LINK-5-CHANGED: Interface FastEthernet0/19, changed state to administratively down

%LINK-5-CHANGED: Interface FastEthernet0/20, changed state to administratively down

%LINK-5-CHANGED: Interface FastEthernet0/21, changed state to administratively down

%LINK-5-CHANGED: Interface FastEthernet0/22, changed state to administratively down

%LINK-5-CHANGED: Interface FastEthernet0/23, changed state to administratively down

%LINK-5-CHANGED: Interface FastEthernet0/24, changed state to administratively down
Switch(config-if-range)#exit
Switch(config)#exit
Switch#
%SYS-5-CONFIG_I: Configured from console by console
write memory
Building configuration...
[OK]
Switch#
```
---
# 2960 GERENCIA
---
```bash 

Switch>enable
Switch#configure terminal
Enter configuration commands, one per line.  End with CNTL/Z.
Switch(config)#interface range fa0/2 - 3
Switch(config-if-range)#
Switch(config-if-range)# switchport port-security
Switch(config-if-range)#
Switch(config-if-range)#switchport port-security maximum 1
Switch(config-if-range)#switchport port-security violation shutdown
Switch(config-if-range)#switchport port-security mac-address sticky
Switch(config-if-range)#exit
Switch(config)#interface range fa0/4 - 24
Switch(config-if-range)#shutdown

%LINK-5-CHANGED: Interface FastEthernet0/4, changed state to administratively down

%LINK-5-CHANGED: Interface FastEthernet0/5, changed state to administratively down

%LINK-5-CHANGED: Interface FastEthernet0/6, changed state to administratively down

%LINK-5-CHANGED: Interface FastEthernet0/7, changed state to administratively down

%LINK-5-CHANGED: Interface FastEthernet0/8, changed state to administratively down

%LINK-5-CHANGED: Interface FastEthernet0/9, changed state to administratively down

%LINK-5-CHANGED: Interface FastEthernet0/10, changed state to administratively down

%LINK-5-CHANGED: Interface FastEthernet0/11, changed state to administratively down

%LINK-5-CHANGED: Interface FastEthernet0/12, changed state to administratively down

%LINK-5-CHANGED: Interface FastEthernet0/13, changed state to administratively down

%LINK-5-CHANGED: Interface FastEthernet0/14, changed state to administratively down

%LINK-5-CHANGED: Interface FastEthernet0/15, changed state to administratively down

%LINK-5-CHANGED: Interface FastEthernet0/16, changed state to administratively down

%LINK-5-CHANGED: Interface FastEthernet0/17, changed state to administratively down

%LINK-5-CHANGED: Interface FastEthernet0/18, changed state to administratively down

%LINK-5-CHANGED: Interface FastEthernet0/19, changed state to administratively down

%LINK-5-CHANGED: Interface FastEthernet0/20, changed state to administratively down

%LINK-5-CHANGED: Interface FastEthernet0/21, changed state to administratively down

%LINK-5-CHANGED: Interface FastEthernet0/22, changed state to administratively down

%LINK-5-CHANGED: Interface FastEthernet0/23, changed state to administratively down

%LINK-5-CHANGED: Interface FastEthernet0/24, changed state to administratively down
Switch(config-if-range)#exit
Switch(config)#exit
Switch#
%SYS-5-CONFIG_I: Configured from console by console
write memory
Building configuration...
[OK]
Switch#
```
---
# 2960 visitantes
---
```bash

Switch>enable
Switch#configure terminal
Enter configuration commands, one per line.  End with CNTL/Z.
Switch(config)#vlan 70
Switch(config-vlan)#name
% Incomplete command.
Switch(config-vlan)#Visitantes
                    ^
% Invalid input detected at '^' marker.
	
Switch(config-vlan)#name Visitantes
Switch(config-vlan)#exit
Switch(config)#enable
% Incomplete command.
Switch(config)#! Porta trunk (uplink)
Switch(config)#
Switch(config)#interface fa0/1
Switch(config-if)#switchport mode trunk
Switch(config-if)#no shutdown
Switch(config-if)#exit
Switch(config)#interface range fa0/2 - 6
Switch(config-if-range)#switchport mode access
Switch(config-if-range)#switchport access vlan 70
Switch(config-if-range)#switchport port-security
Switch(config-if-range)#switchport port-security maximum 1
Switch(config-if-range)#switchport port-security violation shutdown
Switch(config-if-range)#switchport port-security mac-address sticky
Switch(config-if-range)#no shutdown
Switch(config-if-range)#interface range fa0/7 - 24
Switch(config-if-range)#shutdown

%LINK-5-CHANGED: Interface FastEthernet0/7, changed state to administratively down

%LINK-5-CHANGED: Interface FastEthernet0/8, changed state to administratively down

%LINK-5-CHANGED: Interface FastEthernet0/9, changed state to administratively down

%LINK-5-CHANGED: Interface FastEthernet0/10, changed state to administratively down

%LINK-5-CHANGED: Interface FastEthernet0/11, changed state to administratively down

%LINK-5-CHANGED: Interface FastEthernet0/12, changed state to administratively down

%LINK-5-CHANGED: Interface FastEthernet0/13, changed state to administratively down

%LINK-5-CHANGED: Interface FastEthernet0/14, changed state to administratively down

%LINK-5-CHANGED: Interface FastEthernet0/15, changed state to administratively down

%LINK-5-CHANGED: Interface FastEthernet0/16, changed state to administratively down

%LINK-5-CHANGED: Interface FastEthernet0/17, changed state to administratively down

%LINK-5-CHANGED: Interface FastEthernet0/18, changed state to administratively down

%LINK-5-CHANGED: Interface FastEthernet0/19, changed state to administratively down

%LINK-5-CHANGED: Interface FastEthernet0/20, changed state to administratively down

%LINK-5-CHANGED: Interface FastEthernet0/21, changed state to administratively down

%LINK-5-CHANGED: Interface FastEthernet0/22, changed state to administratively down

%LINK-5-CHANGED: Interface FastEthernet0/23, changed state to administratively down

%LINK-5-CHANGED: Interface FastEthernet0/24, changed state to administratively down
Switch(config-if-range)#exit
Switch(config)#exit
Switch#
%SYS-5-CONFIG_I: Configured from console by console
write memory
Building configuration...
[OK]

```
----
# CONFIGURANDO SERVIDOR DHCP
### -- IMAGEM DO STATIC ENDEREÇO PEDIDO PELO PROFESSOR
![image](https://github.com/user-attachments/assets/89d9f6e3-71f2-427e-a684-67dcc2356b4f)
### -- SEPARAÇÃO DAS VLANS PARA O USO DO CLI
![image](https://github.com/user-attachments/assets/bb779b9d-bb15-45b9-bc61-623b9a168d91)
	

```bash
configure terminal
ip routing

interface vlan 10
 ip address 192.168.10.1 255.255.255.0
 ip helper-address 192.168.99.11
 no shutdown
exit

interface vlan 20
 ip address 192.168.20.1 255.255.255.0
 ip helper-address 192.168.99.11
 no shutdown
exit

interface vlan 30
 ip address 192.168.30.1 255.255.255.0
 ip helper-address 192.168.99.11
 no shutdown
exit

interface vlan 40
 ip address 192.168.40.1 255.255.255.0
 ip helper-address 192.168.99.11
 no shutdown
exit

interface vlan 50
 ip address 192.168.50.1 255.255.255.0
 ip helper-address 192.168.99.11
 no shutdown
exit

interface vlan 60
 ip address 192.168.60.1 255.255.255.0
 ip helper-address 192.168.99.11
 no shutdown
exit

interface vlan 70
 ip address 192.168.70.1 255.255.255.0
 ip helper-address 192.168.99.11
 no shutdown
exit


```
---
## CONFIGURANDO CLI
---
```bash
Switch>ENABLE
Switch#configure terminal
Enter configuration commands, one per line.  End with CNTL/Z.
Switch(config)#IPIip routing
Switch(config)#interface vlan 10
Switch(config-if)#ip address 192.168.10.1 255.255.255.0
Switch(config-if)#ipiEXIT
Switch(config)#interface vlan 10
Switch(config-if)#
Switch(config-if)#ip address 192.168.10.1 255.255.255.0
Switch(config-if)#ip helper-address 192.168.99.11
Switch(config-if)#no shutdown
Switch(config-if)#exit
Switch(config)#interface vlan 20
Switch(config-if)#ip address 192.168.20.1 255.255.255.0
Switch(config-if)#ip helper-address 192.168.99.11
Switch(config-if)#no shutdown
Switch(config-if)#exit
Switch(config)#interface vlan 30
Switch(config-if)#ip address 192.168.30.1 255.255.255.0
Switch(config-if)#ip helper-address 192.168.99.11
Switch(config-if)#no shutdown
Switch(config-if)#exit
Switch(config)#interface vlan 40
Switch(config-if)#ip address 192.168.40.1 255.255.255.0
Switch(config-if)#ip helper-address 192.168.99.11
Switch(config-if)#no shutdown
Switch(config-if)#exit
Switch(config)#interface vlan 50
Switch(config-if)#ip address 192.168.50.1 255.255.255.0
Switch(config-if)#ip helper-address 192.168.99.11
Switch(config-if)#no shutdown
Switch(config-if)#exit
Switch(config)#interface vlan 60
Switch(config-if)#ip address 192.168.60.1 255.255.255.0
Switch(config-if)#ip helper-address 192.168.99.11
Switch(config-if)#no shutdown
Switch(config-if)#exit
Switch(config)#interface vlan 70
Switch(config-if)#ip address 192.168.70.1 255.255.255.0
Switch(config-if)#ip helper-address 192.168.99.11
Switch(config-if)#no shutdown
Switch(config-if)#exit
Switch(config)#interface vlan 99
Switch(config-if)#ip address 192.168.99.1 255.255.255.0
Switch(config-if)#no shutdown
Switch(config-if)#exit
Switch(config)#
```
