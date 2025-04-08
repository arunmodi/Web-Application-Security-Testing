# DNS Rule

![](<../../../.gitbook/assets/image (7).png>)

![](<../../../.gitbook/assets/image (33).png>)





```
alert udp any any -> any 53 (msg:"DNS Request Detected";sid:9000000;)
alert udp any 53 -> any any (msg:"DNS Reply Detected";sid:9000001;)
```
