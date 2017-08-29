# Sending messages from PowerPanel

PowerPanel can send messages to your customers. You can set the email address where the messages are sent from at the branding page of your controlpanel.

![Sender email settings](/images/sender_email_settings.png)

The messages that are in settings -> system messages will be send from the address you have filled in.

To make sure your messages are not marked as spam you will have to add an SPF record to the domain you are sending email from.
For example, we send messages from powerpanel.io
We set a TXT (SPF) record for powerpanel.io to: v=spf1 include:mail.registrar.eu ?all
The CNAME record is default._domainkey.powerpanel.io to: dkim.registrar.eu
