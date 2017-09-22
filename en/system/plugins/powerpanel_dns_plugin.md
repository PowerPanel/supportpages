# PowerPanel DNS plugin

We provide a PowerPanel DNS plugin which you can use to manage the DNS from within PowerPanel. To enable this plugin you have to follow the next few steps.
First you will have to install the plugin. Go to the Settings -> Plugins and search for PowerPanel DNS. You will only have to switch the plugin on to install it.

![PowerPanel PowerDNS](/supportpages/images/plugin_powerpanel_dns.png)

After you have turned on the plugin you have to create the nameserver. The domainname that you want to use as nameserver will have to be managed in PowerPanel. To create the nameserver go to System -> Settings -> Domain settings and scroll to Default nameserver settings. Click on the “add name server set” button in the bottom. The next screen will pop up:

![Add nameserver set](/supportpages/images/add_nameserver_set.png)

You can name the nameservers yourself to an address you want, for example ns1.demodns.io and ns2.demodns.io. You will have to set the ip addresses to the following:


| Hostname          | IPv4            | IPv6                                     |
| ----------------- | --------------- | ---------------------------------------- |
| ns1.powerpanel.io  | 52.28.191.114   | 2a05:d014:c84:fb00:e831:6e75:cd66:cd9e |
| ns2.powerpanel.io  | 52.207.110.159  | 2600:1f18:400:3c02:5fae:30d3:c0ca:78c7 |
| ns3.powerpanel.nl  | 52.213.66.39    | 2a05:d018:5de:7f02:2fc5:fadd:7ada:300c |

If you want to use ns1.powerpanel.io and ns2.powerpanel.io you won’t have to fill in the IP addresses, so you can uncheck “Add IP address”.

After you have created your nameserver set you will have to fill in the SOA settings.

![Soa settings](/supportpages/images/soa_settings.png)

Fill in your information and enable “Activate Name Server Set”.

Below this you also have the option to enable this for your resellers, so your resellers can enable their own nameserver set. To enable this, switch on “Allow Name Server Registration”

If you have done all these things you will have to create a few DNS records for the domain you have set as your nameserver.
A record with the IP address and name for our nameservers.
At your registrar you have to create a glue record that points to our ip addresses
