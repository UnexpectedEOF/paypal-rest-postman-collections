Postman Collections for the PayPal REST API
======

Practice making calls to the PayPal REST API without writing any code. This repo contains Collections for Postman that are broken down into the various resources you can access through the API, so you only import what you want.

Never used the Postman extension before? Check out [this link for a tutorial](http://wiki.acstechnologies.com/display/DevCom/POSTMAN+REST+Client+for+Chrome).


How to use this thing
======

Before getting started, make sure you have a PayPal account. Also, install Chrome and Postman.

###1. Create an app on the PayPal Developer Portal
Sign into http://developer.paypal.com with your PayPal account. Once you're there, go to [Your Apps](http://developer.paypal.com/webapps/developer/applications/myapps) and create a new app. *Take note of your "Client ID" and "Secret" under "Test credentials".*


###2. Download and import the Collections and Environment files
Download or clone this repo. Then open up Postman in Chrome, and click "Import Collection" to import all of the collections you want to deal with (make sure to at least import the OAuth collection). Do the same thing with the Environment file by clicking "Manage Environments" and then "Import Environment."


###3. Fill in your credentials and get an access token
Go back to the PayPal-REST-OAuth Collection, open the "OAuth Token Request" call, and then paste the client ID and secret from the first step into the "Basic Auth" tab. Refresh the headers and press "Send"! Copy the "access_token" value that comes back.

Paste the access_token into your Environment file. Now, all of the calls will be able to securely communicate with PayPal. Go nuts!


Progress
======

### PayPal resources we have collections for so far:
* [OAuth 2.0](https://github.com/UnexpectedEOF/paypal-rest-postman-collections/blob/master/collections/PayPal-REST-OAuth.json)
* [Payments](https://github.com/UnexpectedEOF/paypal-rest-postman-collections/blob/master/collections/PayPal-REST-Payments.json)
* [Refunds](https://github.com/UnexpectedEOF/paypal-rest-postman-collections/blob/master/collections/PayPal-REST-Refunds.json)
* [Sales](https://github.com/UnexpectedEOF/paypal-rest-postman-collections/blob/master/collections/PayPal-REST-Sales.json)
* [Captures](https://github.com/UnexpectedEOF/paypal-rest-postman-collections/blob/master/collections/PayPal-REST-Captures.json)
* [Authorizations](https://github.com/UnexpectedEOF/paypal-rest-postman-collections/blob/master/collections/PayPal-REST-Authorizations.json)
* [Stored/tokenized credit card (Vault)](https://github.com/UnexpectedEOF/paypal-rest-postman-collections/blob/master/collections/PayPal-REST-Vault.json)

By the way, this is still very much under construction. Don't expect any level of completeness for a while.