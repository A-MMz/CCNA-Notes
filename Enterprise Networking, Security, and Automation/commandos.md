tratar de hacer ping
192.168.30.10


r1
```
en 
show ip protocol
conf t
interface loopback0
ip address 1.1.1.1 255.255.255.255
router ospf 10
network 1.1.1.1 0.0.0.0 area 0
network 10.1.1.0 0.0.0.3 area 0
network 10.1.1.4 0.0.0.3 area 0
netowor 192.168.10.0 0.0.0.255 area 0
do show ip ospf int brief
do show ip ospf neighbor
```

r2
```
en
conf t
int l0
ip address 2.2.2.2 255.255.255.255
do show ip protocol
router ospf 10
do show ip protocol
do show ip ospf int brief
network 2.2.2.2 0.0.0.0 area 0
network 0.0.0.0 255.255.255.255 area 0
do show ip ospf int brief
do show ip ospf neighbor

```

r3
```
en
conf t
int l0
ip address 3.3.3.3 255.255.255.255
router ospf 10
do show ip protocol
router-id 33.3.3.3
do show ip protocol
router-id 3.3.3.3
network 0.0.0.0 255.255.255.255 area 0
do show ip ospf int brief
do show ip ospf neighbor



```
ping 192.168.30.10

r3
```
end
show ip ospf database
```