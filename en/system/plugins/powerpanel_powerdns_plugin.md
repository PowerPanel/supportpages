# PowerPanel PowerDNS plugin

We provide a PowerDNS plugin which you can use to manage the DNS from within PowerPanel. To enable this plugin you have to follow the next few steps.
First you will have to install the plugin. Go to the Settings -> Plugins and search for PowerPanel DNS. You will only have to switch the plugin on to install it.

![PowerPanel PowerDNS](/images/plugin_powerpanel_dns.png)

After you have turned on the plugin you have to create the nameserver. The domainname that you want to use as nameserver will have to be managed in PowerPanel. To create the nameserver go to System -> Settings -> Domain settings and scroll to Default nameserver settings. Click on the “add name server set” button in the bottom. The next screen will pop up:

![Add nameserver set](/images/add_nameserver_set.png)

You can name the nameservers yourself to an address you want, for example ns1.demodns.io and ns2.demodns.io. You will have to set the ip addresses to the following:

ns1.powerpanel.io : 52.28.191.114
ns2.powerpanel.io : 52.207.110.159
ns3.powerpanel.nl: 52.213.66.39

If you want to use ns1.powerpanel.io and ns2.powerpanel.io you won’t have to fill in the IP addresses, so you can uncheck “Add IP address”.

After you have created your nameserver set you will have to fill in the SOA settings.

![Soa settings](/images/soa_settings.png)

Fill in your information and enable “Activate Name Server Set”.

Below this you also have the option to enable this for your resellers, so your resellers can enable their own nameserver set. To enable this, switch on “Allow Name Server Registration”

 

If you have done all these things you will have to create a few DNS records for the domain you have set as your nameserver.
A record with the IP address and name for our nameservers.
At your registrar you have to create a glue record that points to our ip addresses
