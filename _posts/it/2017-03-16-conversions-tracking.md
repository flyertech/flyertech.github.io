---
layout: docs
title:  "Tracciamento conversioni"
permalink: it/conversions-tracking
---
### Cos'è il tracciamento delle conversioni

Dopo aver ricevuto una **email transazionale**, il cliente atterra sul tuo sito. Se lui/lei sceglie di reclamare il tuo coupon (o offerta) e **concludere l'ordine** sul tuo shop, il **lead** diventa una **conversione diretta**.

Possiamo tracciare queste conversioni se avvengono entro 28 giorni dal primo accesso dell'utente al tuo sito.

### Come funziona

Quando **crei una campagna**, specifichi sempre una **landing page** per la tua offerta speciale.

Nel codice di **quella stessa pagina** bisogna includere lo **snippet di codice per il conversion tracking**.

### Come lo implemento (dettagli tecnici)

> Per prima cosa, devi assicurarti che lo <a href="/it/engage">snippet di integrazione</a> sia stato implementato in tutte le pagine del sito.

Piazza il seguente snippet nella tua **pagina di conferma ordine**. 

Sostituisci ai segnaposti `<ammontare>`, `<valuta>` e `<id_ordine>` i valori reali.

L'`<ammontare>` dell'ordine può essere numero o stringa, con un punto che separa i decimali.

La `<valuta>` va passata come stringa nel formato ISO di 3 caratteri, ad es. `GPB`, `EUR`.   
**Dato che è una stringa** assicurati che sia racchiusa tra virgolette.

L'`<id_ordine>` è una stringa ed è opzionale.

{% highlight html %}
<script src="https://www.transactionale.com/conversion/js/v1/conversion.js"></script>
<script>
    _tr_conversion(<ammontare>, <valuta>, <order_id>);
</script>
{% endhighlight %}

### Ok, allora devo semplicemente copiare questo testo sul mio sito?

> **No. Ricorda che devi adattare questo codice al tuo ambiente.** Questo significa che, ad esempio, `<ammontare>` è solo un segnaposto d'esempio che rappresenta una variabile JavaScript, che deve essere generata/passata dal tuo server con una sintassi corretta (incluse le virgolette se si tratta di una stringa).

Come esempio, se il tuo sito è scritto in PHP, devi passare le variabili necessarie dal tuo sito/CMS, usando le funzioni che il tuo sito ha nativamente per prelevare i dati corretti e inserirli nel JavaScript:

{% highlight php %}
<?php
// Ricorda che questo è un **esempio**.
// Perciò le funzioni getOrderAmount() and getOrderCurrency() sono solo
// di esempio. Per favore adatta l'implementazione al tuo software/CMS!
$orderId = $currentOrder['id'];
$amount = getOrderAmount($orderId);
// Ricordati che la valuta (currency) è una stringa, pertanto richiede *virgolette*.
// Su PHP è possibile crearle con json_encode().
$currency = json_encode(getOrderCurrency($orderId));
?>
<script src="https://www.transactionale.com/conversion/js/v1/conversion.js"></script>
<script>
    _tr_conversion(<?php echo $amount?>, <?php echo $currency ?>, <?php echo $orderId ?> );
</script>
{% endhighlight %}

Così, se il vostro cliente finalizza un ordine da 12.30€, con un id ordine 27894, il codice PHP dovrà produrre il seguente JavaScript:

{% highlight html %}
<script src="https://www.transactionale.com/conversion/js/v1/conversion.js"></script>
<script>
    _tr_conversion(12.30, "EUR", 27894);
</script>
{% endhighlight %}
