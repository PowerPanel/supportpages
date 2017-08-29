# How invoicing works in PowerPanel

In this post we will go into detail about how the invoicing system works in PowerPanel.

At each first day of the month PowerPanel will generate new invoices for your customers based on the subscriptions of your customer in combination with the invoice period of the customer.
Based on the set invoice periode of a customer the system will look at his subscriptions and gather all the subscriptions that have a renewal date in the coming invoice period. Each of these subscriptions will be put on the invoice for your customer.
After you have approved the invoice or, if you have set it to automatically, the systems approves the invoice, the services will be renewed and the renewal date will be set forward based on the invoice period of the subscription.

Example:
Customer A has a subscription for domainname.com which has a renewal date on 18-06-2017 with an invoice period of a year. Customer A has a monthly invoice period. On June first the system will run a task to create all the invoices, for Customer A the system will look for all the subscriptions that have a renewal date in the coming month based on the invoice period of the customer. The subscription for domainname.com will be put on the invoice and when the vendor approves the invoice, the subscription for domainname.com will be extended with a year and the domainname will be registered for another year at the connected registrar.
