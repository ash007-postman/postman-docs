---
title: "Let’s Encrypt SSL cert auto-renewal"?
order: 3
page_id: "Let’s-Encrypt-SSL-cert-auto-renewal"?
warning: false
---

### Let’s Encrypt SSL cert auto-renewal

Postman documentation may be hosted on your custom domain if you are on Team, Business or Enterprise plan.

Postman automatically generates an SSL certificate using LetsEncrypt for your documentation on a custom domain if your domain has no CAA records. If your domain has CAA records set, then LetsEncrypt needs an explicit CAA record to issue a certificate for that domain. To enable LetsEncrypt to issue this certificate, refer to the [LetsEncrypt Documentation](https://letsencrypt.org/docs/caa "https://letsencrypt.org/docs/caa").

**Frequently asked questions:**

-** How long are these SSL Certificates valid for?**

Certificates are generated with a 90-day expiry date.

-** How & when does 'Let’s Encrypt' renew SSL certificates for published documentation?**

The certificate gets renewed at 7 days from the expiry.

-** Do I need to perform any steps to renew the certificate?** 

Certificates are renewed automatically, no manual steps are required.

-** Who issues Certificate on the published documentation?**

Certificates for documentation hosted one custom domain are issued via **Let’s Encrypt**.

For the ones on documenter(default), uses the Amazon issued certificate for the \*.getpostman.com domain.

-** How do we enable SSL for documentation on a custom domain?**

Once the documentation is published on a custom domain, SSL is automatically set up and wouldn't require any additional steps further.
