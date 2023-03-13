<link rel="stylesheet" type="text/css" href="..\markcss.css">

secure shell

```
hostname <name>
ip domain-name <domain>
username <username> secret <password>
crypto key generate rsa modulus <?>
ip ssh version <version>

line vty 0 4 (interface)
login local
transport input ssh
```