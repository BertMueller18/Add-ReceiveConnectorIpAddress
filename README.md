# Add-ReceiveConnectorIpAddress
Add remote IP address ranges to an Exchange Server 2013 receive connctor.

##Description
Add IP address(es) to an existing receive connector on selected or all Exchange 2013 Servers

##Inputs
ConnectorName  
Name of the connector the new IP addresses should be added to  

FileName
Name of the input file name containing IP addresses

ViewEntireForest
View entire Active Directory forest (default FALSE)

##Outputs
Status information written to shell

##Examples
Add IP addresses from ip.txt to MYCONNECTOR
```
.\Add-ReceiveConnectorIpAddress.ps1 -ConnectorName MYCONNECTOR -FileName D:\Scripts\ip.txt
```

```
.\Add-ReceiveConnectorIpAddress.ps1 -ConnectorName REMOTECONNECTOR -FileName .\ip-new.txt -ViewEntireForest $true
```


##Credits
Written by: Thomas Stensitzki

Find me on:

* My Blog:	http://www.sf-tools.net/
* Twitter:	https://twitter.com/apoc70
* LinkedIn:	http://de.linkedin.com/in/thomasstensitzki
* Github:	https://github.com/Apoc70

For more Office 365, Cloud Security and Exchange Server stuff checkout services provided by Granikos

* Blog:     http://blog.granikos.eu/
* Website:	https://www.granikos.eu/en/
* Twitter:	https://twitter.com/granikos_de
