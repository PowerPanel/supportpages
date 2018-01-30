# PowerDNS DNSSec

In this manual you will find a guide about how you can enable the DNSSec option to enable DNSSec on the PowerDNS. Because the PowerDNS API does not have DNSSec support we have created an add-on to have DNSSec working.
This example is specifically made to use with PowerPanel.
First you will need to get the script (powerdns.php) from  [https://github.com/PowerPanel/PowerDNS-DNSSec/tree/master](https://github.com/PowerPanel/PowerDNS-DNSSec/tree/master)

On the MASTER nameserver (Where dnssec commands are available and can be executed) you will need to follow the next few steps.

```
– Install php5+/Php7
– install webservice (Apache/Nginx)
– Edit + Upload the php script (Top lines)
– insert the following line in sudoers (line 35 in the example)
– Secure your system with firewalls (set port 80 open only for our API: 52.214.1.187)
– In PowerPanel you need to (re-)enable the PowerDns plugin. It will automatically detect the Dnssec script on the MASTER Dns port 8082
```

After this you can enable the DNSSec from PowerPanel.
