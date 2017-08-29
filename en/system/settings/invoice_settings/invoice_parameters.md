# Invoice parameters

To setup your own invoice we have the following parameters available. These parameters will be filled in when the invoice is generated. Surround the parameters with 2 curly brackets like this {{customer.id}} to let our parser know that it has to replace the parameter. Some parameters are HTML, make sure to use 3 curly brackets for these to let the parser know that it’s HTML.

#### Customer
* customer.id
* customer.name
* customer.vendor_id
* customer.is_reseller
* customer.is_end_customer
* customer.address_data, (complete array with all the data)
* customer.address_data.address
* customer.address_data.zipcode
* customer.address_data.city
* customer.address_data.country_code
* customer.address_data.country
* customer.registered_date
* customer.terms_of_payment_days
* customer.company_number
* customer.bankaccount_number
* customer.custom_attribute

#### User
* user.id
* user.status
* user.status_id
* user.name
* user.first_name
* user.last_name
* user.email
* user.role
* user.language
* user.gender
* user.last_login

#### Vendor
* vendor.name
* vendor.address_data.address
* vendor.address_data.zipcode
* vendor.address_data.city
* vendor.address_data.country_code
* vendor.address_data.country
* vendor.support_phonenumber
* vendor.website_url
* vendor.registered_date
* vendor.vat_number
* vendor.terms_of_payment_days
* vendor.company_number
* vendor.bankaccount_number
* vendor.cp_url
* vendor.default_email
* vendor.email.domain
* vendor.email.invoice

#### Invoice
* invoice.price.valuta_symbol_html (Note! 3 curly brackets instead of 2)
* invoice.id
* invoice.number
* invoice.status_id
* invoice.hash
* invoice.is_credit
* invoice.preauthorized_debit_date
* invoice.dates.invoice.year
* invoice.dates.invoice.month
* invoice.dates.invoice.month_full
* invoice.dates.invoice.month_short
* invoice.dates.invoice.day
* invoice.dates.invoice.day_of_month
* invoice.dates.invoice.day_full
* invoice.dates.invoice.day_short
* invoice.dates.invoice.number_of_days_this_month
* invoice.dates.sent.year
* invoice.dates.sent.month
* invoice.dates.sent.month_full
* invoice.dates.sent.month_short
* invoice.dates.sent.day
* invoice.dates.sent.day_of_month
* invoice.dates.sent.day_full
* invoice.dates.sent.day_short
* invoice.dates.sent.number_of_days_this_month
* invoice.dates.expiry.year
* invoice.dates.expiry.month
* invoice.dates.expiry.month_full
* invoice.dates.expiry.month_short
* invoice.dates.expiry.day
* invoice.dates.expiry.day_of_month
* invoice.dates.expiry.day_full
* invoice.dates.expiry.day_short
* invoice.dates.expiry.number_of_days_this_month
* invoice.price.gross_amount
* invoice.price.netto_amount
* invoice.price.tax_amount
* invoice.price.total_amount
* invoice.price.gross_amount_real
* invoice.price.netto_amount_real
* invoice.price.tax_amount_real
* invoice.price.total_amount_real

#### Invoice Lines
#invoice.lines
* id
* name
* description
* product_name
* gross_amount
* netto_amount
* discount_amount
* discount_percentage
* subscription_type_id
* period
* period_id
* subscription_type
* start_date
* end_date
* subscription_id
* invoice_id
* order_id
* is_order
* amount
* number
/invoice.lines

#invoice.discount.lines
* description
* percentage
* price
/invoice.discount.lines

* vat.percentage
* vat.value
* vat.number

Within the tags {{#invoice.lines}} and {{/invoice.lines}} you can use the tags

* {{amount}}
* {{units}} number of units.
* {{price.unit}} price per unit
* {{price.gross}} gross price
* {{price.netto}} Netto price
* {{price.discount}} Discount price
* {{ledger_code}}

Deprecated parameters:
The following parameters are deprecated and will not be supported anymore somewhere in the future.

* {{gross_amount}}
* {{netto_amount}}
* {{discount_amount}}
