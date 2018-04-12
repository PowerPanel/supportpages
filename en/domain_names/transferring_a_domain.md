# Transferring a domain
This article explains how to transfer a domain correctly in PowerPanel. However, be aware that the full transfer process is different depending on the TLD. The owner and existing registrar should be aware of the transfer as a minimum. Additionally a transfer code may be required, and the owner may need to respond to a confirmation email. In some cases additional paperwork may be required. Please consult the documentation of your registrar to understand the correct process before starting the transfer in PowerPanel. Also note, that depending on the TLD, the transfer may be instant, or it could take several weeks to complete.

If you need a domain to be operational from the instant it has been transferred, then you will need to set up the DNS before beginning the transfer proper. If you wish to setup the DNS after the domain has been transferred, please skip ahead to the [second part of the article](#transfer).

### 1.  Setup DNS for the domain (optional)

**NB** If you are a reseller performing a transfer, before you start, please **first make sure you log in as the customer** who wishes the domain to be transferred. (See the article on [logging in as a customer](/supportpages/account_management/my_customers/login_as_customer.md)

1. In the side menu click on "Domain names" and then "My domains".

    ![Domain names menu item](/supportpages/images/my_domains.png)
    
2. A table will appear listing all your domains. Click the "+ Add" button above the table.

    ![Add a domain](/supportpages/images/add_domain.png)

3. A dialog box will pop up, asking whether you want "to create a new DNS zone" or "request a new domain or transfer an existing domain". Transferring the domain will come later, at this stage we wish to create a new DNS zone, so choose the first option.

4. After indicating that we wish to create a new DNS zone, you will be prompted for a domain name. Make sure you enter the name of the domain you wish to transfer. Leave the "Enable DNS hosting" checkbox checked, as this indicates that we want a DNS zone to be created.

    ![Creating a DNS Zone](/supportpages/images/dns_zone.png)

5. Click the the green "Save" button and the domain record will be created. You will see that the that the status of the domain is "Registered elsewhere", which is indeed the case as we have yet to transfer the domain.

    ![Status of the new domain](/supportpages/images/registered_elsewhere.png)

6. Scrolling a bit further down to the "Domain settings" section, you will see the "DNS Zone" button. Click this button to edit the DNS settings for this domain.

    ![Status of the new domain](/supportpages/images/dns_zone_button.png)

7. You will now see the DNS settings for the domain. You should set them up ready for when the domain is transferred. The configuration of DNS won't be covered here as it is a complex topic that is beyond the scope of this article.

###<span id="transfer">2. Transferring the domain</span>

We will now start the transfer proper.

**NB** If you are a reseller performing a transfer, before you start, please **first make sure you log in as the customer** who wishes the domain to be transferred. (See the article on [logging in as a customer](/supportpages/account_management/my_customers/login_as_customer.md)

1. In the side menu click on "Domain names".

    ![Domain names menu item](/supportpages/images/domain_names.png)

2.  In the main panel you will see the tab "Order domain". Click on this tab.

	![Domain dashboard](/supportpages/images/order_domain.png)

3. In "Step 1" enter the domain name you wish to transfer, and click the green "Check" button.

    ![Step 1](/supportpages/images/step_1.png)

4. PowerPanel will then list your domain with several other variations (this is because the same screen is used for ordering new domains). Make sure you click on the orange "Transfer" button for the domain you want to transfer.

    ![Step 1](/supportpages/images/step_1_2.png)
     
5. The other steps will appear. In "Step 2" the contacts for the domain can be chosen. Use the "Add" button if you need to create a new contact.

    ![Step 2](/supportpages/images/step_2.png)

6. In "Step 3" the nameservers must be chosen for the domain. The simplest option is to choose "Use the default nameserver settings" as this requires no further configuration. If you understand DNS then you can choose the "I have my own name servers (not managed by the system)" option and use your own servers.

    ![Step 3](/supportpages/images/step_3.png)

7. In "Step 4" you need to enter an authorization code. This is a secret code that the current domain owner should give you. This proves to the registry that the owner has agreed to the transfer. You can also request whois privacy if desired.

    ![Step 4](/supportpages/images/step_4.png)

8. Finally in the "Check your order" section, confirm that you are happy with the price, and click the green "Order" button to go ahead with the transfer.

    ![Check your order](/supportpages/images/check_order.png)

9. Now that you've requested the transfer, you can find the domain under "Domain names > My domain". The domain will be in one of the following states:

    * **Error** - There is a problem with the transfer that you need to address
    * **Pending** - The transfer process has been started
    * **Active** - Congratulations, the domain has been transferred!

The next section describes what to do in the event of a problem with the transfer.

### 3. Dealing with errors

As noted at the beginning of the article the transfer processes varies by TLD. However typical problems may include an incorrect or expired authorization code, or the failure of the current owner to respond to a confirmation email.

To correct problems with the transfer and retry, click on the record for the domain. Then click on the green "Process Domain Order" button in the "Domain properties" section.

![Process Domain Order](/supportpages/images/domain_properties.png)

The "Process domain order" dialog will pop up. There are three tabs that allow you to change information connected with the order: "Domain Contact Details", "Edit Name Server" and "Transfer". The fields in these tabs will be familiar from the screen where the domain was originally ordered. Frequently you will need to correct or enter an new authorization code. This can be done under the "Transfer" tab.

![Process Domain Order](/supportpages/images/transfer_authcode.png)

After any corrections have been made, the transfer can be retried by clicking on the green "Process Domain Order" button at the bottom of the dialog.

### 3. Summary
This article has explained the need to research the transfer process for a TLD before starting. We have also covered setting up the DNS for an incoming domain, so that the domain is immediately functional upon transfer, and we have also looked at how to do the actual transfer.

For resellers we have also seen that it is important to ensure that we are logged in as the correct user when performing these operations on behalf of a customer.

We have also seen how we can correct problems with the transfer and restart the process.

