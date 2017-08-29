# Twinfield

With the Twinfield plugin you can import the invoices that PowerPanel generates into your Twinfield environment. At the moment you approve an invoice, it will be sent to your Twinfield environment.

To start with setting up the Twinfield plugin in PowerPanel you will need to install the plugin first. Go to the marketplace at System -> Plugins and look for the Twinfield plugin. After you have installed the plugin you will see a screen with all the settings that are needed for the Twinfield plugin.

![Twinfield settings](/images/plugin_twinfield_settings.png)

Fill in all the fields with your details. Make sure to fill in the VAT codes and the default ledger code as they are needed for the correct handling of the plugin.
The invoices will be booked on Accounting -> Provisional Transactions in Twinfield.

![Twinfield invoices](/images/twinfield_provisional_invoices.png)

We have two options available for importing the invoicelines into Twinfield, splitted out or grouped by product group. Use the switch in the settings to choose yourself.

### Freetext3

It is possible in Twinfield to link directly to the invoice in PowerPanel. To enable this you will have to enable the freetext3 field in Twinfield and set a document Imaging link.
Go to General ->Transaction types in Twinfield and select  the sales entry’s.
There you will have to set the freetext3 field to allowed. At the Document imaging you will have to set a name and a Link. The link needs to be:

https://{{your PowerPanel url}}/billing/details/invoicedetails/$freetext3/

Click save and enable the setting in PowerPanel and then you are done.

![Twinfield freetext3](/images/twinfield_freetext3.png)

It is really important that you enable the setting in Twinfield when you enable it in PowerPanel or the import to Twinfield will fail.
