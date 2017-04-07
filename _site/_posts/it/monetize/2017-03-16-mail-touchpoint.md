---
layout: docs
title:  "Integrazione del touchpoint mail (server-side)"
permalink: it/mail-touchpoints
lang: it
---
Se abilitata, Transactionale manda un'email ai tuoi client a nome tuo per ogni transazione che essi fanno sul tuo sito. Per permettere questa operazione, bisogna chiamare la nostra API REST dopo ogni ordine che ricevi. Le chiamate all'API devono essere autenticate con la chiave API (API key) che troverai nella sezione "Integrazione" del tuo Account. 
Sono richiesti solo tre campi dati, di cui l'ultimo opzionale:

* Country (Stato): il codice nazionale ISO di due lettere (`IT`, `DE` ...) per la nazione sulla quale è stato piazzato l'ordine
* Email: l'indirizzo email del cliente
* First name (Nome): il nome proprio del cliente, in modo da potergli mandare una mail personalizzata
* Zip code (CAP): se verrà fornito un codice CAP del cliente (Zip Code fuori dall'Italia), verranno fornite con priorità più alta le campagne geolocalizzate, in modo che siano più efficaci

La chiamata API è molto semplice. Di seguito troverete esempi nei linguaggi di programmazione più comuni.

> NOTA: è possibile integrare questa chiamata lato client, ma suggeriamo di implementarla lato server per motivi di sicurezza, perché coinvolge informazioni sensibili. Siete tuttavia liberi di optare per la strategia che riterrete opportuna.

### Esempi di integrazione

Abbiamo un po' di esempi nei linguaggi server-side più comuni:

- [{{ site.data.lang.integration_example_in[page.lang] }} PHP](./integrations/php)
- [{{ site.data.lang.integration_example_in[page.lang] }} Ruby](./integrations/ruby)
- [{{ site.data.lang.integration_example_in[page.lang] }} Python](./integrations/python)
- [{{ site.data.lang.integration_example_in[page.lang] }} NodeJS](./integrations/nodejs)
- [{{ site.data.lang.integration_example_in[page.lang] }} C#](./integrations/csharp)
- [{{ site.data.lang.integration_example_in[page.lang] }} cURL](./integrations/curl)

{% capture my_include %}{% include integration_notes_it.md %}{% endcapture %}
{{ my_include | markdownify }}