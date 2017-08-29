# Adyen plugin

To connect your Adyen account to PowerPanel you will have to set up a few things.
First you will need to enter the following credentials into PowerPanel:

* Merchant Account
* SkinCode
* HmacKey
* environment

![adyen plugin settings](/images/plugin_adyen_settings.png)

These settings can be found in your adyen account at the Skins tab.

![adyen skincode](/images/adyen_skincode.png)

You will have to generate the hmackey for you skin in the skin settings yourself. Click on the skin and click on, generate new HMAC Key. Note: you will have to select the platform that matches the enironment you will choose in PowerPanel.

![adyen hmac key](/images/adyen_hmac_key.png)

## Notification url:

To check if a payment was succesfull your customers will be redirected back to PowerPanel after their payment. Customers can break off the process after they have payed their invoice but before they are redirected. To make sure that PowerPanel gets a notification that the invoice has been payed you can set a notification URL in your adyen environment. To do this login to Adyen and go to Settings -> Server communication. There you will add a standard notification and set the url to  https://{{your url}}/json-api/userresponse/adyenpayment/0, set the method to JSON. After that you are done. PowerPanel will recieve a notification from Adyen whenever a payment is done by a customer.

![Adyen notification url](/images/adyen_notification_url.png)

## Note for country’s

At the start of the payment process we do a issuer request to check for the possible issuers in your account. Because our servers are located around the world it can happen that we do for example a request from Ireland. Ideal is not available in that country and is by default prohibited for use. You can manage this yourself in your control panel at Adyen. Go to Skins -> Skin -> Payment methods and click on Ideal. Check the mark at Overwrite available countries and select all the countries available. This will make sure that your selected payment method will work worldwide.

![Adyen country settings](/images/adyen_country_settings.png)
