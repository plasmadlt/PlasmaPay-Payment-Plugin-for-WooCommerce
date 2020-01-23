# PlasmaPay Payment Plugin for WooCommerce
* **Contributors**: Plasmapay
* **Tags**: Payments, сredit-card
* **Requires at** least: 5.3.2
* **Tested up to**: 5.3.2
* **Requires PHP**: 7.0
* **Stable tag**: 1.0.0
* **License**: GPLv2 or later
* **License URI**: http://www.gnu.org/licenses/gpl-2.0.html


## Description
### Available payment methods on the PlasmaPay platform 
* accepting Visa / Mastercard cards (business verification required)
* accepting payment in Bitcoin (verification is not required)
* accepting payments from PlasmaPay wallets (verification is not required)
= Available payment methods =
* payment to the user\'s wallet in the PlasmaPay system with further withdrawal of funds to the card / bank account / payment systems / cryptocurrency (verification is not required)
### Available ways to replenish and withdraw funds from your PlasmaPay account 
* replenishment and withdrawal to Visa/Mastercard
* replenishment and withdrawal via bank transfers SEPA/SWIFT
* deposit and withdrawal using AdvCash
* replenishment and withdrawal of funds for online banking for Asian banks
* withdrawal of funds to the cryptocurrency BTC, ETH, USDT, etc. (upon request)
* replenishment and withdrawal of funds with the help of partners on
Visa / Mastercard / Mir
bank accounts in hryvnia and ruble
payment systems: Paypal, Qiwi, Yandex.Money, WebMoney, etc.
cash: USD, RUB, UAH
### Integration of payment acceptance by Visa/Mastercard cards. Card Processing.
By connecting PlasmaPay you can accept card payments for your goods and services from more than 150 countries. The card processing service is available only for companies with a registered legal entity and legal address of registration. To use the PlasmaPay system, a bank account for the company is not a prerequisite.
### To connect service you need 
* register an account on plasmapay.com
* activate Plasma account with company or site name
* pass personal verification and receive the status of \"Digital Citizen\" on the platform
* request a company profile by mail business@plasmapay.com
* fill out and send a questionnaire along with scans of statutory documents
* after checking the documents and signing the electronic contract, your account will be assigned the status \"Business\" and you will be able to generate API keys for integrating checkout windows into your online store or service

 [Details page](https://about.plasmapay.com/en/articles/3505108-open-business-account-in-payment-system-plasmapay)

### Payment process 
After integration with PlasmaPay, a new payment method will become available on your website: *Pay with Plasma* or *Pay with PlasmaPay*.
To pay the invoice, the user will be redirected to checkout page on the PlasmaPay side, certified according to PCI DSS security standards.
The user should enter an email to identify him/her in the payment system and selects one of the available payment methods:
*  With a PlasmaPay personal wallet
*  By credit card
*  With a cryptocurrency wallet
Upon completion of payment, the user receives a cashier\'s check for the transaction. In the user\'s mobile bank or statement, this operation will be indicated as: PlasmaPay.




# Installation
### Automatic installation 
Automatic installation is the easiest option as WordPress handles the file transfers itself and you don’t need to leave your web browser. To do an automatic install of the WooCommerce Plasmapay  plugin, log in to your WordPress dashboard, navigate to the Plugins menu and click Add New.
In the search field type “WooCommerce Plasmapay Payment” and click Search Plugins. Once you’ve found our plugin you can view details about it such as the point release, rating, and description. Most importantly, of course, you can install it by simply clicking “Install Now”, then “Activate”.
= Manual installation =
The manual installation method involves downloading our plugin and uploading it to your web server via your favorite FTP application. To learn more, see Installing and Managing Plugins.
Updating
Automatic updates should work like a charm; as always though, ensure you backup your site just in case.

### Configuration 

The main application setting is in the application Plasmapay after which you get the API  keys

*Plasmapay webiste*   >  *Business*  > *Create Application*  >   *And follow line Settings*

**Settings**: 

**Application title**
The name of your site or application
Success uri
URI link to the successful payment page. The user will be redirected to this page along with the identifier of his invoice

 *Example: https://yoursite.com/checkout/order-receive*


**Failure uri**
URI link to the page about failed payment or cancellation of payment. Together with this, the invoice identifier is transmitted

*Example: https://yoursite.com/cart*

**Whitelist Domain**
The domain/address of your site on which the PlasmaPay payment method will be available

*Example: yoursite.com*

**WebHooks**
The URI on which we send the invoice when the status is changed new -> pending -> success, so that the merchant can determine that the invoice has been processed and paid

*Example: https://yoursite.com/?wc-api=plasmapay_gateway*


**Who will pay  fee**
You can choose who will pay the fee for processing the payment: company or client. If the company pays the commission, then the invoice amount will be final for the payer, if the client pays the commission, then for payment he will receive the invoiced amount + payment system commission.
  After when you get API KEY  you need go to your *WordPress* >   *WooCommerce* > *Settings* > *Payment* > *Plasmapay Payment* > *and then add API KEY*

[Details page](https://about.plasmapay.com/en/articles/3505108-open-business-account-in-payment-system-plasmapay)

# Frequently Asked Questions 
### Does this support recurring payments, like for subscriptions?
Yes!
### Does this require an SSL certificate? 
Yes! In Live Mode, an SSL certificate must be installed on your site to use PlasmaPay. In addition to SSL encryption, PlasmaPay provides an extra JavaScript method to secure card data.
### Does this support both production mode and sandbox mode for testing? 
 Yes, it does – production mode is driven by the API keys you use. Sandbox  we are planning a future update.
### Where can I get support or talk to other users? =
If you get stuck, you can ask for help in the Plugin Forum.


# Screenshots

### Installation Dashboard inside WooCommerce > Settings
<img align="сenter" width="500" height="250" src="https://github.com/plasmadlt/woocommerce-plasmapay-gateway/raw/master/img/screenshot-1.png"> </br> 

### Use Standard Checkout Page  WooCommerce (can be you customized) 

<img align="сenter" width="250" height="350" src="https://github.com/plasmadlt/woocommerce-plasmapay-gateway/raw/master/img/screenshot-2.png"> </br> 

### Redirect payment on after Checkout Process on PlasmaPay  
<img align="сenter" width="390" height="450" src="https://github.com/plasmadlt/woocommerce-plasmapay-gateway/raw/master/img/screenshot-3.png"> </br> 

# Changelog
**1.0.0**
* First Realize


