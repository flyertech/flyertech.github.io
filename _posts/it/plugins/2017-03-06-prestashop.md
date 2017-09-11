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

<img src="{{ site.url }}/assets/img/prestashop/modules_menu.png" />

Clicca sul pulsante *Aggiungi nuovo modulo*:

<img src="{{ site.url }}/assets/img/prestashop/modules_buttons.png" />

Apparirà un form dove potrai caricare il file zip del modulo:

<img src="{{ site.url }}/assets/img/prestashop/module_upload.png" />

Dopo averlo installato, lo devi abilitare:

<img src="{{ site.url }}/assets/img/prestashop/module_installed.png" />

Ora cliccando su *Configura* appariranno le impostazioni del modulo:

<img src="{{ site.url }}/assets/img/prestashop/module_configuration.png" />

### Configurazione del modulo

Copia la tua API KEY dal tuo accout transactionale da My Account -> Integration:

<img src="{{ site.url }}/assets/img/integrate_api_key.png" />

e incollala nel campo API KEY delle impostazioni del modulo.

### Dettaglio delle impostazioni

  - *API KEY*: necessario per identificare il tuo account. Segui le istruzioni qui sopra per compilarlo.
  - *Codice nazione*: il codice ISO a due lettere della nazione in cui opera il tuo shop. AD es. *IT*.
  - *Stato*: imposta su *Disabilitato* per disabilitare l'integrazione. Questo disabiliterà sia l'integrazione advertiser che publisher.
  - *Abilita integrazione Advertiser*: imposta su *Abilitato* per abilitare il popup di atterraggio quando gli utenti cliccano sulle tue campagne di acquisizione. E' necessario solo se il popup è stato abilitato nelle tue campagne.
  - *Abilita integrazione Publisher*: usa il canale mail per inviare offerte ai tuoi utenti, sincronizzate con le tue mail di conferma ordine.
  - *Abilita annunci in pagina di conferma ordine*: imposta su *Disabled/Manual* se non vuoi mostrare offerte nella tua thank-you page, oppure se vuoi incollare a mano lo snippet di integrazione. Altrimenti seleziona il touchpoint web desiderato. **ATTENZIONE**: questo richiede che la funzionalità sia abilitata nel tuo account Transactionale. 
  - *Testo prima di annunci in pagina di conferma ordine*: se usi il web touchpoint descritto sopra, puoi specificare il testo da mostrare prima delle offerte.
  - *Trasmetti codice fiscale*: imposta su *Abilitato* se vuoi trasmettere il codice fiscale dei tuoi clienti. Viene impiegato per determinare il sesso e l'età, qualora non esplicitamente compilati.
  - *Trasmetti il sesso*: imposta su *Abilitato* se vuoi consentire campagne targettizzate per sesso.
  - *Trasmetti numero di telefono*: imposta su *Abilitato* se vuoi condividere il numero di telefono con gli advertiser.
  - *Snippet per annunci in pagina di conferma ordine*: se si intende usare un web touchpoint manualmente, è possibile incollare qui lo snippet necessario.
  - *Transactionale Host URL*: Solo per debugging. Lasciare invariato.



