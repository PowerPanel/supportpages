# Get the pricelist from the API

You can get all the tld prices with the example below.
Just fill in your own API key which can be found in your account in PowerPanel.

You will have to whitelist the IP address from where you are running the script to make sure that it works.

Note: Please make sure that you cache the prices for some time so that you don’t make a call every time someone visits the place where you show the prices.

 
```php

$ch = curl_init();
curl_setopt($ch, CURLOPT_URL, ‘https://api.powerpanel.io/1.0/domain/getTldPriceList’);
curl_setopt($ch, CURLOPT_CUSTOMREQUEST, ‘POST’);
curl_setopt($ch, CURLOPT_RETURNTRANSFER, 1);

// Set headers
curl_setopt($ch, CURLOPT_HTTPHEADER, array(
    “API_KEY: apikey”,
    “Content-Type: application/json”
    )
);
$body = json_encode(array());
curl_setopt($ch, CURLOPT_POST, 1);
curl_setopt($ch, CURLOPT_POSTFIELDS, $body);
$resp = curl_exec($ch);
$http_code = curl_getinfo($ch, CURLINFO_HTTP_CODE);

if($resp && http_code == 200) {
    $response = json_decode($resp, true);

    if($response[‘code’] == 1) {
        $result = $response[‘result’];

        // Do something with the result (array met TLD’s/prijzen/etc)
    }
}
curl_close($ch);
```
