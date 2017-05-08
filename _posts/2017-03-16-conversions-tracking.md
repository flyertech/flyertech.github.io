---
layout: docs
title:  "Conversions tracking"
permalink: conversions-tracking
---
### What is conversion tracking

After receiving a **transactional email**, the customer lands on your site. If he/she chooses to redeem your coupon/offer and **finalize the order** on your shop, the **lead** becomes a **direct conversion**.

We can track those conversions for you if they happen within 28 days from the user's first access to your site.

### How does it technically work

When you **create a campaign**, you always specify a **landing page** for the offer. 

On **that page** you must include the **conversion tracking snippet**.

### How do I implement conversion tracking (technical details)

> First of all, you have to make sure the <a href="/engage">integration snippet</a> is present **in your campaigns' landing pages**.

Place the following snippet in the section of your order confirmation page. 

Replace the `<amount>`, `<currency>` and `<order_id>` placeholders with the appropriate values.

The `<amount>` can be either a number or a string, with a dot separator for decimals. 

The `<currency>` must be passed as its ISO 3 letter code, i.e. `USD`, `EUR`.   
**It is a string** so make sure to enclose it in quotes.

The `<order_id>` is a string and it's optional

{% highlight html %}
<script src="https://www.transactionale.com/conversion/js/v1/conversion.js"></script>
<script>
    _tr_conversion(<amount>, <currency>, <order_id>);
</script>
{% endhighlight %}

### Ok, so I have just to copy this code as-is on my website?

> **No. Please remember that you must adapt this code to your particular environment.** This means that, for example, `<amount>` is only an example placeholder that stands for a Javascript variable that must be passed from your server, with a correct JavaScript syntax (this includes using quotes when you pass a string).

Just as an example, if your site is based on PHP, you have to pass somehow the necessary variables from your website/CMS, using the function your site provides natively to fetch the correct data into JavaScript:

{% highlight php %}
<?php
// Remember that this below is an **example code** in PHP.
// The getOrderAmount() and getOrderCurrency() functions are therefore only
// example functions. Please adapt the implementation on your own software/CMS!
$orderId = $currentOrder['id'];
$amount = getOrderAmount($orderId);
// Remember that currency is a string, so it needs *quotes*. In PHP we can provide
// them with json_encode().
$currency = json_encode(getOrderCurrency($orderId));
?>
<script src="https://www.transactionale.com/conversion/js/v1/conversion.js"></script>
<script>
    _tr_conversion(<?php echo $amount?>, <?php echo $currency ?>, <?php echo $orderId ?> );
</script>
{% endhighlight %}

So, if your customer places an order of 12.30 EUR, with an order id of 27894, the above PHP code should render the following JavaScript:

{% highlight html %}
<script src="https://www.transactionale.com/conversion/js/v1/conversion.js"></script>
<script>
    _tr_conversion(12.30, "EUR", 27894);
</script>
{% endhighlight %}

