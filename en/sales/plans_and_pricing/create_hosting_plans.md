# Create a hosting plan (package)

You can manage your hosting plans in PowerPanel. Whenever a customer orders a hosting package in your webshop, a hosting package with your hosting plan settings will be created on your server.
It can happen that a customer orders multiple hosting packages that will be installed on the same server. In that case PowerPanel will create a different client/user for each hosting package. This has been created this way because of single sign on. If a customer uses single sign on to login on the server the customer will only see the hosting package that he logs in to. Other hosting packages are not available for that customer.

Let’s start with creating a new hostingplan. For this guide we will create a Plesk plan as an example, creating a plan for cPanel or DirectAdmin works the same way.
First make sure that you have installed the Plesk plugin, [you can follow the following guide to do this.](/en/hosting/my_servers/add_plesk_server.md)

If you have done this you can create your hosting plan. Go to Sale -> Plans & Pricing -> Hosting Plan and click on add.

![Add hosting plan](/supportpages/images/add_hosting_package.png)

Here you can choose if you want to use predefined plans or a custom one, the unchanged plans are for your resellers, the can sell your packages without changes to it. Select ‘I want to compose a customised package’, fill in a name and click on save.
Now you can start customising your plan.
In the top part you can manage the settings that will be visible in the webshop. You can manage the hosting plan name, the color that is visible in the webshop, and the description that is available in the webshop.

![Hosting plan basic settings](/supportpages/images/hosting_package_basic_settings.png)

You can create a hosting plan that is not activated in the webshop so that you can activate it for a customer, to do this you can leave the switch ‘Activate in web shop’ disabled.
Allow copy is a setting that is useful if you have resellers, if you enable this setting your resellers can copy the hosting plan and use it for themselves.

Below these settings you can set the resources for the hosting plan.

![Hosting package settings](/supportpages/images/hosting_package_settings.png)

Make sure to check all these settings to create your hosting plan.
