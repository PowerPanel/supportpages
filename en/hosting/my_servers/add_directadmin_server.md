# Connecting your DirectAdmin server

You can manage your DirectAdmin server from PowerPanel. This way your customers can manage their own sitesettings like subdomains, email addresses and aliasses.

### Single sign on

Another feature for your customers is single sign on, they can logon to the server with a simple click of a button.
For this to work on DirectAdmin the server admin first will have to enable a few settings.
In the file /usr/local/directadmin/conf/directadmin.conf you will have to set login_keys=1 (not ON, but 1).
A reseller has 2 files that have this settings:
user.conf (the settings for this acount)
reseller.conf(this will give the rights through to lower accounts and is needed for this option to work)

Here the settings voor login_keys should be ON or OFF (A bit confusing, but thats how we now it works)
An existing account with this settings disabled will not work and will have to work through all the config files to enable this settings. You can use the following lines to prevent doing this by hand:
find /usr/local/directadmin/data/users -type f -print0 | xargs -0 sed -i ‘s/login_keys=OFF/login_keys=ON/g’
find /usr/local/directadmin/data/admin -type f -print0 | xargs -0 sed -i ‘s/login_keys=OFF/login_keys=ON/g’

### Connecting DirectAdmin to PowerPanel

To connect your DirectAdmin server to PowerPanel you’ll have to follow the next steps.

First you will have to enable the DirectAdmin plugin.
To do this go to System -> Plugins -> look for the DirectAdmin plugin, install it and enable it in the settings.

![Directadmin plugin](/images/directadmin_plugin.png)

After you have done this you can add a server with the directAdmin plugin by going to Hosting -> My servers -> Add server
![Add directadmin server](/images/add_directadmin_server.png)

After this the sites on the server will appear in the site conflicts where you can assign them to a customer.
Make sure that you use the hostname as the following example: https://hostname.io
