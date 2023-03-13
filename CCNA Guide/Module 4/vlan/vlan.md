<link rel="stylesheet" type="text/css" href="..\..\markcss.css">

creates vlan
```
sw1(config)#vlan <1-4094>
name <NAME>
```
assign vlan to interface
```
interface <id>
switchport access vlan <id>

```

deletes vlan
```
no vlan <id>
```

delete vlan db from switch
```
delete flash:vlan.dat
```

```
show interfaces <int id> switchport
```

TRUNKING
```
show interfaces trunk
```
encapsulation
 ```
interface <int idd>
switchport trunk encapsulation ?
    dot1q usually picked
 ```

 set native vlan
 ```
swichport trunk native vlan <id>
 ```
set trunk mode

```
switchport mode ?
    dinamic desirable
    auto
    trunk
```
