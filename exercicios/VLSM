SWITCH 1

vlan 10
ip address 192.168.0.0 255.255.248.0
name Testes
exit
vlan 20
ip address 192.168.8.0 255.255.252.0
name Telemarketing
exit
vlan 30
ip address 192.168.16.0 255.255.255.0
name Consultores
exit
vlan 40
ip address 192.168.20.0 255.255.255.192
name RH
interface range f0/1-9
switchport mode access
switchport access vlan 10
exit
interface range f0/10-17
switchport mode access
switchport access vlan 20
exit
interface range f0/18, f0/22, f0/24
switchport mode access
switchport access vlan 30
exit
interface range f0/19, f0/20, f0/21, f0/23
switchport mode access
switchport access vlan 40
exit
interface g0/1
switchport mode trunk
switchport trunk native vlan 88
switchport trunk allowed vlan 10,20,30,40,88
exit
do wr




SWITCH 2


vlan 50
ip address 10.0.0.0 255.254.0.0
name Analistas
exit
vlan 60
ip address 10.2.0.0 255.255.224.0
name Operacao
exit
vlan 70
ip address 10.2.32.0 255.255.252.0
name TI
exit
vlan 80
ip address 10.2.36.0 255.255.255.0
name Administrativo
exit
interface range f0/1-20
switchport mode access
switchport access vlan 50
exit
interface f0/24
switchport mode access
switchport access vlan 60
exit
interface f0/21, f0/23
switchport mode access
switchport access vlan 70
exit
interface f0/22
switchport mode access
switchport access vlan 80
exit
interface g0/1
switchport mode trunk
switchport trunk native vlan 88
switchport trunk allowed vlan 50,60,70,80,88
exit
do wr


SWITCH 3

vlan 80
ip address 192.168.32.0 255.255.252.0
name Financas
exit
vlan 60
ip address 192.168.36.0 255.255.254.0
name Operacoes
exit
vlan 88
ip address 192.168.38.0 255.255.255.128
name Relogios
exit
vlan 32
ip address 192.168.38.128 255.255.255.224
name Livres
exit
interface f0/1-5
switchport mode access
switchport access vlan 80
exit
interface f0/6-9
switchport mode access
switchport access vlan 60
exit
interface f0/10-19
switchport mode access
switchport access vlan 88
exit
interface f0/20-24
switchport mode access
switchport access vlan 100
exit
interface g0/1
switchport mode trunk
switchport trunk native vlan 88
switchport trunk allowed vlan 60,88,100,88
exit
do wr


SWITCH 4


vlan 88
ip address 172.24.0.0 255.254.0.0
name Servidores
exit
vlan 200
ip address 172.26.0.0 255.255.192.0
name Voz
exit
vlan 90
ip address 172.26.64.0 255.255.255.0
name TACACS
exit
vlan 88
ip address 172.16.0.0 255.248.0.0
name Monitoramento
exit
interface f0/1-9
switchport mode access
switchport access vlan 88
exit
interface f0/10-12
switchport mode access
switchport access vlan 200
exit
interface f0/13-14
switchport mode access
switchport access vlan 90
exit
interface f0/15-24
switchport mode access
switchport access vlan 88
exit
interface g0/1
switchport mode trunk
switchport trunk native vlan 88
switchport trunk allowed vlan 88,200,90,88
exit
do wr
