# SPF record PowerPanel

To make sure that the email that PowerPanel sends from your account to your customers will not be accounted as spam you can add the following spf record to your domain:

```
v=spf1 mx include:spf.powerpanel.io a:
```
