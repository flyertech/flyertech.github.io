---
layout: docs
title:  "Installare e configurare il plugin per WooCommerce"
permalink: it/plugins/woocommerce
lang: it
---

### Ottenere la versione più recente del plugin WooCommerce

Puoi scaricare l'ultima versione dalla tua dasbhboard, andando su My Account -> Integration -> Click sul pulsante WooCommerce.

### Installazione del plugin

Dal menù di WordPress, selezione Plugin -> Aggiungi:

<div class='img-responsive'><img src="{{ site.url }}/assets/img/woocommerce/modules_menu.png" /></div>

Clicca sul pulsante *Carica plugin*:

<div class='img-responsive'><img src="{{ site.url }}/assets/img/woocommerce/module_upload_btn.png" /></div>

Apparirà un form. Seleziona il file zip del modulo per installarlo:

<div class='img-responsive'><img src="{{ site.url }}/assets/img/woocommerce/module_upload.png" /></div>

Ora attiva il plugin:

<div class='img-responsive'><img src="{{ site.url }}/assets/img/woocommerce/module_activation.png" /></div>

Vedrai il plugin nell'elenco dei plugin installati. Clicca su *Settings*:

<div class='img-responsive'><img src="{{ site.url }}/assets/img/woocommerce/module_entry.png" /></div>

Apparirà la pagina delle impostazioni:

<div class='img-responsive'><img src="{{ site.url }}/assets/img/woocommerce/module_configuration.png" /></div>


#### Dettaglio delle impostazioni

*Transactionale status*|imposta su *disabled* per disattivare l'integrazione. Questo disattiverà sia l'integrazione advertier che publisher.
*API KEY*|è necessaria per identificare il tuo account. **Segui le istruzioni qui sotto per compilarla.**
*Country code*|il codice ISO di due lettere della nazione in cui opera il tuo shop. Ad es. *IT*
*Pass phone*|imposta su *Enabled* per condivider i numeri di telefono con gli advertiser.
*Enable Transactional e-mail*|usa il canale mail per inviare offerte ai tuoi utenti, sincronizzate con le tue mail di conferma ordine.
*Web touchpoint snippet*|se usi il web touchpoint, incolla qui lo snippet necessario.
*Web touchpoint text*|se usi il web touchpoint, puoi specificare qui il testo da mostrare prima delle offerte.



### Configurazione del plugin

- Vai sul **sito di Transactionale**, nella pagina **My Account -> Integration**.

- Copia la tua **API Key** dalla maschera **"Your API Key"**. Invece di selezionare il testo puoi anche semplicemente cliccare sul tasto **Copy**.

<div class='img-responsive'>
  <img src="{{ site.url }}/assets/img/integrate_api_key.png" />
</div>

- **Torna su Wordpress**

- vai alla **pagina di configurazione del modulo Transactionale** 

- **incolla l'API Key** che hai copiato prima nell'apposito campo.

<div class='img-responsive'>
  <img src="{{ site.url }}/assets/img/woocommerce/api_key.png" />
</div>


