# Very Important think to keep in mid#
## **DISABLE OPTION 82 in DHCP on S1** ##
### Somne routers dont support this field in dhcp packets and drop them ###
```
no ip dhcp snooping information option
```
## **MAKE SURE THERE ARE DHCP SNOOPING BINDINGS AFTER ENABLING THE FUTURE ON SWITCH AND GETTING THE IP VIA DHCP** ##
```
show ip dhcp snooping binding
```