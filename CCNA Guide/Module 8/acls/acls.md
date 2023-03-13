<link rel="stylesheet" type="text/css" href="..\..\markcss.css">

- Can permit or deny trafic

- Can be applied inboud or outbound 

- Can be used to match traffic

![](2023-03-12-18-53-03.png)

---
numbered

![](2023-03-12-18-54-29.png)

```
access-list <? number> permit <?> <ip>
```

```
int <int id>
ip access-group <? usually inside-outside>
```

--- 
![](2023-03-12-19-05-36.png)

```
show access-list
```

```
ip access-list extended <name>
<?>
deny <packet> host <ip> <host> ip
```

edit 
```
ip access-list extended <name> <?>
```