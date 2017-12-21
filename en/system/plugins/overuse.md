# Overuse

PowerPanel gives you the possibility to charge your customers for their overusage on a hostingpackage. To use this feature you will have to go through the next steps to set up the system.

First you will have to set up a cronjob on your server with a script that you can get from https://github.com/PowerPanel/Overuse
Let this script run at least once each day to ensure that the data we receive is up te date.
In the script you will have to set up a webhook url, you can find this unique url in the plugin settings. If for example you use Plesk, go to Settings -> Plugins -> Plugin Settings -> Plesk. 
There you will find a that looks like this: https://api.powerpanel.io/hooks/uniquehash. Paste this in the script together with your admin credentials and you are good to go.

If we receive any data your server overview will look a bit like this:
![Server detail](/supportpages/images/server_detail.png)

The subscriptions that are on the server will also show some data for the used traphic and diskspace.

After you have set up the cronjob you will have to set a few settings in PowerPanel.
The first thing to do is to set up your prices. You can do this by going to your hosting package and scroll down to the settings.

![Hosting plan global settings](/supportpages/images/hosting_plan_global_settings.png)

Behind the settings you see two fields, before usage price and overusage price. The “before usage price” is the pre paid price, customers can choose to pay in advance in case they are expecting that they will have overuse. 
(This feature is not live yet but you can set the price in for when it’s going live).
The second price is the overusage price that your customers will pay when they have overuse without pre buying it.
The units that you see here are based on what is set in the hosting settings. To set this up go to  System -> Settings -> Hosting settings. Here you will find the “Default usage units”, change this to the setting you want.

![Hosting settings](/supportpages/images/hosting_settings.png)

At this screen you can also set the minimum threshold for the overuse, together with the type of minimum overuse, this can be a price or a percentage. 
If a customer reaches the threshold you have set, he will recieve an invoice.  Here you can also enable a warning email for your customer as well as the threshold in percentage when this email will be sent to your customer.

If you enable the email you will have to set up a message that can be sent to your customers. To do this go to System -> Settings -> System messages and look for the Website overconsumption email. 
We have filled in a default mail, but you can customize this for your own needs.

![Overuse message](/supportpages/images/overuse_message.png)

