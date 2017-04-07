---
layout: docs
title:  "Mail touchpoint integration (server-side)"
permalink: mail-touchpoints
lang: en
---
If enabled, Transactionale sends an email to your customers on your behalf for every transaction they make on your website. In order to do that, you must call our REST API after every order you receive. Calls must be authenticated using the API key you find in the Integrate section of your account. 
Only three data fields are required, while the last is optional:

* Country: the standard ISO two-letter code for the shop the order was placed on
* Email: the customer's email address
* First name: the customer's first name, so we can send a personalized email
* Zip code (optional): if a zip code is provided, we will prioritize ads that are targeted for that area.

The API call is straightforward. Our website has examples in the most common programming languages.

> NOTE: you can also integrate this call client-side. We suggest placing it server-side for a matter of security, because it involves personal information. However, it’s up to you to decide the best strategy.

### Integration examples

We have a deal of examples in the most common server-side languages:

- [{{ site.data.lang.integration_example_in[page.lang] }} PHP](./integrations/php)
- [{{ site.data.lang.integration_example_in[page.lang] }} Ruby](./integrations/ruby)
- [{{ site.data.lang.integration_example_in[page.lang] }} Python](./integrations/python)
- [{{ site.data.lang.integration_example_in[page.lang] }} NodeJS](./integrations/nodejs)
- [{{ site.data.lang.integration_example_in[page.lang] }} C#](./integrations/csharp)
- [{{ site.data.lang.integration_example_in[page.lang] }} cURL](./integrations/curl)

Some notes:

- We use [Unirest](http://unirest.io/) in our examples, but feel free to use any framework or library capable of making HTTP POST requests
- **Remember to customise the variables in the examples - the snippet will not work as-is**
- You have a personal API key in the Integrate section of your account
- The HTTP request’s content type must be `application/json`
- The body of the HTTP request must contain **a JSON-encoded object with your data**
