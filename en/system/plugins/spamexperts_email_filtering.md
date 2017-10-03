# SpamExperts Email Filtering

With the SpamExperts plugins for incoming and outgoing email filtering you can give your customers a hosting addon to their current hosting package. These filter can be added to PowerPanel as a ‘hosting add-on’. You can add an add-on to an existing hosting package or let customers order the add-on in your webshop. PowerPanel will handle the provisioning of the spamfilter and create a subscription for your customer.

To get started with this plugin go to System -> Plugins and look for the SpamExperts plugin, click on install and fill in your details.
Both the incoming and the outgoing spamfilter can be sold separately by installing one of the plugins. The set up for both plugins works the same way.

![Spamexperts settings](/supportpages/images/plugin_spamexperts.png)

Once you have filled in all your details and enabled the plugin you can go create a hosting add-on and add it to a hosting package.

More information about how to create a hosting add-on can [be found in this item.](/en/sale/plans_and_pricing/create_hosting_addon.md)

If one of your customers has a hosting package with the SpamExperts addon he can use single sign on from within PowerPanel to check his spamfilter.

![Spamfilter plugin view](/supportpages/images/spamfilter_detail_view.png)

For the outgoing filter your customer will see his address and port based on the settings that you have entered.

## Important settings on the SpamExperts filter

On the SpamExpert spam filter you need to create a account for PowerPanel plugin on two places. You need to create this on Software API users and on Manager super-admins. Note: Make sure you create this users using the same username and password.

Step 1) Logon with your admin account (Or account where you have enough permissions to maintain user permissions).

Step 2) Go to server and click software API users. there you need to create an account voor the PowerPanel plugin.

![Spamexperts 1](/supportpages/images/spamexperts_1.png)

Step 3) Go to Webinterface users and click Manage super-admins. there you need to create an account voor the PowerPanel plugin.

![Spamexperts 2](/supportpages/images/spamexperts_2.png)
