# Collection agency letter example

If an invoice has not been payed by your customer after a few reminders the invoice will get the status, collection agency. You can find all the invoices that needs to be sent to the collection agency in the credit management tool at the tab -> Invoices for collection agency. There you can print out the letter. You will need a template for the letter to be able to print out the letter. In the settings tab you can enter the letter for this. Below you will find an example for that letter.

### Letter to collection agency

Dear employee,

Here a new collection assignment.

Customer data (if data is not filled in, then we have no data available):
Customer name: {{customer.name}}
Contactperson:{{user.name}}
Gender: {{user.gender}}
e-mail address: {{user.email}}
Phone number.: {{customer.phone}}
Address: {{customer.street}}
Zipcode: {{customer.zip}}
City: {{customer.city}}
Chamber of commerce code: {{customer.kvk}}
Vat number.: {{customer.btw}}

Invoice data:
Invoice number.: #{{invoice.number}}
Invoice date: {{invoice.datum}}
Invoice total: € {{invoice.total}}

In the appendix you will find a copy of the invoice. If you have any questions about this letter i would like to hear from you.
With kind regards,
Administration {{vendor.name}}


### Letter to your customer

Below you will find an example for a reminder letter for your customer that can be sent.

 

{{address_block}}

Customernumber:	{{customer_id}}
Date:	{{date}}
concerns:	{{subject}}
Dear {{customer_name}},

Our records show that we have not yet recieved a payment for the invoice(s) below. This despite earlier reminders.

{{invoices}}

We request, and if necessary summon, you to pay the overdue amount within 7 days after the date of this letter. You can transfer the amount to us with the mentioning of the invoicenumber.

Suspension of services
If we do not recieve the payment in the set term, we will hold the right to suspend our services temporarily or permanent. Reactivation costs will be for your account.

Contact for questions.
There could be a good reason why you have not paid this invoice yet. Please get in touch with us if so.

With kinds regards,

Administration {{vendor.name}}

