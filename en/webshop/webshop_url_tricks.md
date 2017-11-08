# Webshop url tricks
You can use a few url’s to the webshop to link them directly from your own site.

### Start the domain checker from remote site
Check a domain directly: https://demoshop.mypp.io/checkdomain?domain=google.com
You can use an input field on your website, and send the GET request to the webshop to start the domain checker.

An other option is to implement the API command [domain/available](https://api.powerpanel.io/docs/Domain/available)


### Send data to the shoppingcart of your webshop (Experimental)
Prepair a json object on your website and send this object to the webshop shoppingcart directly. If you are combine this with the SSO option your customer need only go though the checkout page.

You have to combine this function on the ```Domain/getTldPriceList```. More information [here](https://api.powerpanel.io/docs/Domain/getTldPriceList) and [here](get-pricelist-api).

JSON object example:
```json
{
    "domains": {
        "google.be": {
            "val_unit": 1,
            "dt_id": 13,
            "tld": "be",
            "valuta": "EUR",
            "sp_id": 3,
            "sp_period": 12,
            "da_id": 2,
            "val_symbol": "€",
            "request_price": 24,
            "transfer_price": 49,
            "renew_price": 49,
            "dom_name": "google.be"
        },
        "google.nl": {
            "val_unit": 1,
            "dt_id": 14,
            "tld": "nl",
            "valuta": "EUR",
            "sp_id": 3,
            "sp_period": 12,
            "da_id": 2,
            "val_symbol": "€",
            "request_price": 19.8,
            "transfer_price": 29,
            "renew_price": 9,
            "dom_name": "google.nl"
        }
    }
}
```

Sending this object into a POST payload to the following URL: ```https://demoshop.mypp.io/api/system/setShoppingCart/add```
You can use this URL to test your solution, but don't forget to replace demoshop.mypp.io to your own URL.
          
If you want to add SSO (Singl Sign On) support in the same request you can use this options:

```JSON
{
	"sso": true,
	"sso_user": "user@gmail.com"
}
```

Combine this json to one object:

```json
{
	"cart": {
		"domains": {
			"google.be": {
				"val_unit": 1,
				"dt_id": 13,
				"tld": "be",
				"valuta": "EUR",
				"sp_id": 3,
				"sp_period": 12,
				"da_id": 2,
				"val_symbol": "€",
				"request_price": 24,
				"transfer_price": 49,
				"renew_price": 49,
				"dom_name": "google.be"
			},
			"google.nl": {
				"val_unit": 1,
				"dt_id": 14,
				"tld": "nl",
				"valuta": "EUR",
				"sp_id": 3,
				"sp_period": 12,
				"da_id": 2,
				"val_symbol": "€",
				"request_price": 19.8,
				"transfer_price": 29,
				"renew_price": 9,
				"dom_name": "google.nl"
			}
		}
	},
	"options": {
		"sso": true,
		"sso_user": "user@gmail.com"
	}
}

```


Object keys explained:

```
val_unit = Calculate for foreign valuta (Get this info from API command ```Domain/getTldPriceList```)
dt_id = Extension ID (Get this info from API command ```Domain/getTldPriceList```)
sp_id = periode ID
sp_period = Period in moths (1 = month, 3 = quartal, 12 = year etc.)
da_id = domain action (1 = request new, 2 = transfer)
Get all pricing information from API command ```Domain/getTldPriceList```
```

[Download here a working example (html / javascript)](files/addtocart.html)

