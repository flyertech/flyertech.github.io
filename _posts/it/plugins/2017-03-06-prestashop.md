---
layout: docs
title:  "Configurare ed installare il modulo Prestashop"
permalink: it/plugins/prestashop
lang: it
---

### Ottenere l'ultima versione del modulo Prestashop

Puoi scaricare la versione più recente dalla tua dashbaord andando su My Account -> Integration -> Click sul pulsante *Prestashop*.

### Installazione del modulo

Vai alla sezione *Moduli e Servizi*:

<div class='img-responsive'>
  <img src="{{ site.url }}/assets/img/prestashop/modules_menu.png" />
</div>

Clicca sul pulsante *Aggiungi nuovo modulo*:

<div class='img-responsive'>
  <img src="{{ site.url }}/assets/img/prestashop/modules_buttons.png" />
</div>

Apparirà un form dove potrai caricare il file zip del modulo:

<div class='img-responsive'>
  <img src="{{ site.url }}/assets/img/prestashop/module_upload.png" />
</div>

Dopo averlo installato, lo devi abilitare:

<div class='img-responsive'>
  <img src="{{ site.url }}/assets/img/prestashop/module_installed.png" />
</div>

Ora cliccando su *Configura* appariranno le impostazioni del modulo:

<div class='img-responsive'>
  <img src="{{ site.url }}/assets/img/prestashop/module_configuration.png" />
</div>


#### Dettaglio delle impostazioni

*API KEY*|necessario per identificare il tuo account. **Segui le istruzioni qui sotto per compilarlo**.
*Codice nazione*|il codice ISO a due lettere della nazione in cui opera il tuo shop. AD es. *IT*.
*Stato*|imposta su *Disabilitato* per disabilitare l'integrazione. Questo disabiliterà sia l'integrazione advertiser che publisher.
*Abilita integrazione Advertiser*|imposta su *Abilitato* per abilitare il popup di atterraggio quando gli utenti cliccano sulle tue campagne di acquisizione. E' necessario solo se il popup è stato abilitato nelle tue campagne.
*Abilita integrazione Publisher*|usa il canale mail per inviare offerte ai tuoi utenti, sincronizzate con le tue mail di conferma ordine.
*Abilita annunci in pagina di conferma ordine*|imposta su *Disabled/Manual* se non vuoi mostrare offerte nella tua thank-you page, oppure se vuoi incollare a mano lo snippet di integrazione. Altrimenti seleziona il touchpoint web desiderato. **ATTENZIONE**: questo richiede che la funzionalità sia abilitata nel tuo account Transactionale. 
*Testo prima di annunci in pagina di conferma ordine*|se usi il web touchpoint descritto sopra, puoi specificare il testo da mostrare prima delle offerte.
*Trasmetti codice fiscale*|imposta su *Abilitato* se vuoi trasmettere il codice fiscale dei tuoi clienti. Viene impiegato per determinare il sesso e l'età, qualora non esplicitamente compilati.
*Trasmetti il sesso*|imposta su *Abilitato* se vuoi consentire campagne targettizzate per sesso.
*Trasmetti numero di telefono*|imposta su *Abilitato* se vuoi condividere il numero di telefono con gli advertiser.
*Snippet per annunci in pagina di conferma ordine*|se si intende usare un web touchpoint manualmente, è possibile incollare qui lo snippet necessario.
*Transactionale Host URL*|Solo per debugging. Lasciare invariato.

### Ultimi passi

- Vai sul **sito di Transactionale**, nella pagina **My Account -> Integration**.

- Copia la tua **API Key** dalla maschera **"Your API Key"**. Invece di selezionare il testo puoi anche semplicemente cliccare sul tasto **Copy**.

<div class='img-responsive'>
  <img src="{{ site.url }}/assets/img/integrate_api_key.png" />
</div>

- **Torna su Prestashop**

- vai alla **pagina di configurazione del modulo** 

- **incolla l'API Key** che hai copiato prima nell'apposito campo.

<div class='img-responsive'>
  <img src="{{ site.url }}/assets/img/prestashop/api_key.png" />
</div>



