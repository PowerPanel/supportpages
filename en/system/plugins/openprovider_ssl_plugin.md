# Configure your Openprovider SSL Plugin

PowerPanel has a fully automated SSL management tool. You can configure serverall SSL providers to PowerPanel. In this document we explain how to connect to Openprovider SSL panel.

Before you can start, make sure you have your Openprovider API information availble. You need the username and API key (Password hash). 
If you don't have this, please read this [article](generate-openprovider-api-key) first 

### 1. Login to PowerPanel
First you need to login to PowerPanel. If you don't have an account you can create an account (use the menu in the header and choose register).
If you need help to login to PowerPanel, please [read](how-to-logon-or-request-password) here how to logon.

### 2. Go to the Plugin Marketplace
To enable the Openprovider SSL plugin, you need to go to the Plugin markteplace. There you can find all Plugins. Find the Openprovider SSL plugin, and click the install button.

![Marketplace](/supportpages/images/plugin_marketplace.png)

### 3. Setup the SSL Plugin
Now the setup page appeard on your screen. You have to fill in the username and password (Password Hash) in the form blow.

![Openprovider SSL Plugin form](/supportpages/images/plugin_openprovider_ssl_form.png)

Information will be saved instantly. If you have enter all fields, you can switch on this plugin. PowerPanel will check the plugin settings to make sure creditentials are correct.
If the plugin can connect to Openprovider below succes message will appear. Now PowerPanel is ready to manage SSL for you.

![Openprovider SSL Plugin test success](/supportpages/images/plugin_openprovider_ssl_done.png)

In the below image you see the settings after the are succesfull tested and saved. Also on the buttom there is the webhook address. You need this later.

![Openprovider SSL Plugin](/supportpages/images/plugin_openprovider_ssl.png)

### 4. Setup the SSL Webhook
If you want to setup the two way connection between Openprovider and PowerPanel you have to enable the webhook in the Openprovider SSL Panel.
SSL panel will send updates about your SSL directly to PowerPanel webhook. To setup follow the below extra steps. This extra steps are not required, but optional.

### 5. Logon to Openprovider SSL Panel
Now login to the Openprovider SSL panel. You can click [here](https://rcp.openprovider.eu/login.php) to logon.

![Openprovider logon screen](/supportpages/images/openprovider_images/login.png)

### 6. Activate SSL webshook
After you are logged on into Openprovider panel, go to SSL Panel. 
On the left click the SSL panel link.

![SSL panel](/supportpages/images/openprovider_images/ssl_panel.png)

Now you see the the settings option. Click the option to go to the hooks section.

![SSL Panel settings](/supportpages/images/openprovider_images/ssl_panel_settings.png)

If there are no webhooks, click the "Add hook" button below the page.

![SSL Panel hooks empty](/supportpages/images/openprovider_images/ssl_panel_hooks_empty.png)

For the event choose the * option. This means all SSL events will send to this webhook.
In the URL you have to copy the PowerPanel webhook address (you have find in step 3 of this article).
Click the save button to save this settings.

![SSL Panel add hook](/supportpages/images/openprovider_images/ssl_panel_add_hook.png)

### 7. Save your new SSL webshook
Now you have created a webhook, and the two way communication has been setup succesfull.

![SSL Panel webhooks](/supportpages/images/openprovider_images/ssl_panel_hooks.png)
