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

<img src="{{ site.url }}/assets/img/woocommerce/modules_menu.png" />

Clicca sul pulsante *Carica plugin*:

<img src="{{ site.url }}/assets/img/woocommerce/module_upload_btn.png" />

Apparirà un form. Seleziona il file zip del modulo per installarlo:

<img src="{{ site.url }}/assets/img/woocommerce/module_upload.png" />

Ora attiva il plugin:

<img src="{{ site.url }}/assets/img/woocommerce/module_activation.png" />

Vedrai il plugin nell'elenco dei plugin installati. Clicca su *Settings*:

<img src="{{ site.url }}/assets/img/woocommerce/module_entry.png" />

Apparirà la pagina delle impostazioni:

<img src="{{ site.url }}/assets/img/woocommerce/module_configuration.png" />

### Configurazione del plugin

Copia la tua API Key dal tuo account Transactionale da My Account -> Integration:

<img src="{{ site.url }}/assets/img/integrate_api_key.png" />

e incollala nel campo API Key delle impostazioni del plugin.

### Dettaglio delle impostazioni

  - *Transactionale status*: imposta su *disabled* per disattivare l'integrazione. Questo disattiverà sia l'integrazione advertier che publisher.
  - *API KEY*: è necessaria per identificare il tuo account. Segui le istruzioni qui sopra per compilarla.
  - *Country code*: il codice ISO di due lettere della nazione in cui opera il tuo shop. Ad es. *IT*
  - *Pass phone*: imposta su *Enabled* per condivider i numeri di telefono con gli advertiser.
  - *Enable Transactional e-mail*: usa il canale mail per inviare offerte ai tuoi utenti, sincronizzate con le tue mail di conferma ordine.
  - *Web touchpoint snippet*: se usi il web touchpoint, incolla qui lo snippet necessario.
  - *Web touchpoint text*: se usi il web touchpoint, puoi specificare qui il testo da mostrare prima delle offerte.



