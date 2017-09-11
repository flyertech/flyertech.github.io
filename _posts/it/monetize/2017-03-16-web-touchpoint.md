---
layout: docs
title:  "Web touchpoint integration"
permalink: it/web-touchpoints
---
If you prefer not to send one more email to your customers, you can use **web touchpoints**.
Web touchpoints define areas in your website where we will display ads with the same criteria as our transactional emails, but the email address will only be shared:
- after the user clicks on an advertisement (**implicit opt-in**) 
- after accepting the advertiser's privacy policy (**double opt-in**). 

This will ensure your privacy standards remain high.

The Monetize => Web touchpoints section of your account provides the necessary Javascript snippets that can be pasted into your website, plus full instructions.
This is an example of Web touchpoint snippet:

<script>
    // Email and optional zip-code here:
    // window.TR_EMAIL = "uncomment@me";
    // window.TR_ZIP_CODE = "12345";

    // Create a div in your page where you want the ads to appear.
    // By default it has to have id tr_touchpoint_container.
    // Or you can specify a custom id like this:
    // window.TR_CONTAINER_ID = "tr_touchpoint_container";
    
    if(typeof window.TR_EMAIL == 'undefined') {
        throw Error('No TR_EMAIL defined!');
    }

    var _trzip = window.TR_ZIP_CODE || '';
    var _trd = document.createElement('div'); _trd.id='transactionale';document.body.appendChild(_trd);
    var _trs = document.createElement('script');
    _trs.src = 'https://www.transactionale.com/touchpoints/1/embed?auth=XXXXX&zip_code=' + _trzip + '';
        document.getElementsByTagName('head')[0].appendChild(_trs);
</script>

