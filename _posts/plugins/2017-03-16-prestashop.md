---
layout: docs
title:  "How to install and configure the Prestashop module"
permalink: plugins/prestashop
lang: en
---

### Obtaining the latest Prestashop module

You can download the latest version from your dashboard by going to My Account -> Integration -> Click on the Prestashop button.

### Installing the module

Go to the Modules page:

<img src="{{ site.url }}/assets/img/prestashop/modules_menu.png" />

Click on the *Add new module* button:

<img src="{{ site.url }}/assets/img/prestashop/modules_buttons.png" />

A form will appear where you can upload the module's zip file:

<img src="{{ site.url }}/assets/img/prestashop/module_upload.png" />

After installing the module, you will need to enable it:

<img src="{{ site.url }}/assets/img/prestashop/module_installed.png" />

Now click con the *Configuration* button to configure the module:

<img src="{{ site.url }}/assets/img/prestashop/module_configuration.png" />

### Configuring the module

Copy your API Key from your Transactionale account under My Account -> Integration:

<img src="{{ site.url }}/assets/img/integrate_api_key.png" />

and paste it into the API KEY field of the module configuration.

### Settings details

  - *API KEY*: this is used to identify your account. Follow the instructions above to fill it.
  - *Country code*: the two-letter ISO code for the country in which your shop operates. I.E. *IT*.
  - *Status*: set to *Disabled* to disable the integration. This will disable both advertiser and publisher integration.
  - *Enable advertiser integration*: set to *Enabled* to enable the landing pop-up when users click on your advertising campaigns. This is only needed if you enabled it in your campaigns.
  - *Enable publisher integration*: use the email channel to deliver offers to your user, in sync with your order confirmation emails.
  - *Enable ads in the order confirmation page*: set to *Disabled/Manual* if you do not want to show offers in your thank-you page, or if you want to manually paste the integration snippet. Select the desired web touchpoint otherwise. **WARNING**: this requires the feature to be enabled on your Transactionale account.
  - *Order confirmation touchpoint text*: if using the web touchpoint described above, you can specify the text to display above the offers.
  - *Send customer VAT ID*: set to *Enabled* if you want to share your customer's VAT ID with advertisers. It is used to work out gender and age, where not explicitly provided.
  - *Send gender*: set to *Enabled* if you want enable targeting campaigns by gender.
  - *Send phone*: set to *Enabled* if you want to share your customers' phone number with advertisers.
  - *Order confirmation page snippet*: if using web touchpoints manually, paste here the required snippet.
  - *Transactionale Host URL*: Only for debugging. Leave as is.



