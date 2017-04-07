---
layout: docs
title:  "Tracciamento conversioni"
permalink: it/conversions-tracking
---
> **IMPORTANTE!** Assicuratevi che lo <a href="/it/engage">snippet di integrazione</a> sia presente nelle landing page delle vostre campagne.
> Tracceremo le conversioni nei 28 giorni successivi al primo accesso del vostro utente.

Place the following snippet in the section of your order confirmation page. 

Replace the `<amount>`, `<currency>` and `<order_id>` placeholders with the appropriate values.

The `amount` can be either a number or a string, with a dot separator for decimals. 

The `currency` is the ISO 3 letter code, i.e. `EUR`. 

The `order_id` is a string and it's optional

{% highlight html %}
<script src="https://www.transactionale.com/conversion/js/v1/conversion.js"></script>
<script>
    _tr_conversion(<amount>, <currency>, <order_id>);
</script>
{% endhighlight %}

> **Please adapt this code to your particular environment.** For example, if you are implementing in PHP, make sure to pass the correct variables:

{% highlight php %}
<?php
$amount = getOrderAmount($orderId);
$currency = json_encode(getOrderCurrency($orderId));
?>
<script src="https://www.transactionale.com/conversion/js/v1/conversion.js"></script>
<script>
    _tr_conversion(<?php echo $amount?>, <?php echo $currency ?>, <?php echo $orderId ?> );
</script>
{% endhighlight %}

For example, if the order is 12.30 EUR, and has an id :

{% highlight html %}
<script src="https://www.transactionale.com/conversion/js/v1/conversion.js"></script>
<script>
    _tr_conversion(12.30, "EUR", 27894);
</script>
{% endhighlight %}

