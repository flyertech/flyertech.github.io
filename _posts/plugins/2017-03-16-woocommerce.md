---
layout: docs
title:  "How to install and configure the WooCommerce plugin"
permalink: plugins/woocommerce
lang: en
---

### Obtaining the latest WooCommerce plugin

You can download the latest version from your dashboard by going to My Account -> Integration -> Click on the WooCommerce button.

### Installing the plugin

From the WordPress menu, select Plugins -> Add new:

<div class='img-responsive'><img src="{{ site.url }}/assets/img/woocommerce/modules_menu.png" /></div>

Click on the *Upload plugin* button:

<div class='img-responsive'><img src="{{ site.url }}/assets/img/woocommerce/module_upload_btn.png" /></div>

A form will appear. Select the zip file to install it:

<div class='img-responsive'><img src="{{ site.url }}/assets/img/woocommerce/module_upload.png" /></div>

Now activate the plugin:

<div class='img-responsive'><img src="{{ site.url }}/assets/img/woocommerce/module_activation.png" /></div>

You will see the plugin in the installed plugins list. Click on *Settings*:

<div class='img-responsive'><img src="{{ site.url }}/assets/img/woocommerce/module_entry.png" /></div>

Now the Settings page will be shown:

<div class='img-responsive'><img src="{{ site.url }}/assets/img/woocommerce/module_configuration.png" /></div>

#### Settings details

*Transactionale status*|set to *disabled* to disable the integration. This will disable both advertiser and publisher integration.
*API KEY*|this is used to identify your account. **Follow the instructions below to fill it**.
*Country code*|the two-letter ISO code for the country in which your shop operates. I.E. *IT*.
*Pass phone*|set to *Enabled* if you want to share phone numbers with advertisers.
*Enable Transactional e-mail*|use the email channel to deliver offers to your user, in sync with your order confirmation emails.
*Web touchpoint snippet*|if you are using web touchpoints, paste the required snippet here.
*Web touchpoint text*|if using the web touchpoint described above, you can specify the text to display above the offers.

### Last steps

Copy your API Key from your Transactionale account under My Account -> Integration:

<div class='img-responsive'><img src="{{ site.url }}/assets/img/integrate_api_key.png" /></div>

and paste it into the API KEY field of the plugin configuration page.




