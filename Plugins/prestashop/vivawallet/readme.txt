Installation:
-Save the vivawallet directory to a zipped package (viva-payment.zip).
-Install the module through your stores module manager (add new module)
-The module will show in your store admin under modules / payments & gateways.
-Enable and configure Vivawallet module.
-At your Vivawallet backoffice create a new payment source:

Success page: modules/vivawallet/success.php
Fail page: modules/vivawallet/fail.php

-An optinal webhook URL can be set in your Vivawallet backoffice -> Settings/API Access/Webhooks, this assures the order will be handled correctly in case the customer does not return to the estore after the transaction:
WEBHOOK URL: http(s)://(www.)your_domain.com/modules/vivawallet/webhook.php
----------------------------------------------------------------------------------------------------------

Vivawallet setup:
You can find your Merchant ID and API Key when you login your business account under Settings - API Access.

To connect the plugin with your e-commerce platform and Vivawallet you would have to create a new Payment Source in your Vivawallet business account, use the generated source code (usually a four digit number) in the plugin settings.

You can create a new Payment Source from the menu My Sales - Payment Sources - New Website/App.
Code - use this code in your plugin
Source Name - provide a logic name here
Linked Wallet - link the payment source to the wallet you want to use with it
Protocol - in case your e-commerce platform uses SSL on the checkout select https, otherwise use https
Integration method - redirection
Company Logo - your png company logo to display on the Vivawallet payment page
Success URL - as described in the plugin instructions
Failure URL - as described in the plugin instructions
Advanced Configuration - usually no need to make any changes here

Wait until Vivawallet has activated your newly created Payment Source before activating the plugin in your e-commerce platform.
