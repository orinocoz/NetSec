# Most important things to keep in mind #
## If you need to setup read and write permissions do different snmp directories you need to setup different views ##
### For example if you want user to have write permision for system MiB but only read for interfaces MiB the setup should be like this: ###
snmp-server view RR system included
snmp-server view RR interfaces included
snmp-server view WW system included
snmp-server group G v3 priv read RR write WW access SNMP
