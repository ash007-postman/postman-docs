---
title: "What is the Usability of SSL Certificates with your requests"?
order: 3
page_id: "What-is-the-Usability-of-SSL-Certificates-with-your-requests"?
warning: false
---
### Usability of SSL Certificates with your requests 

An organization needs to install the SSL Certificate onto its web server to initiate a secure session with browsers. Once a secure connection is established, all web traffic between the web server and the web browser will be secure. When a certificate is successfully installed on your server, the application protocol (also known as HTTP) will change to HTTPs, where the ‘S’ stands for ‘secure’. Depending on the type of certificate you purchase and what browser you are surfing the internet on, a browser will show a padlock or green bar in the browser when you visit a website that has an SSL Certificate installed.

Using the [Postman native apps](https://www.postman.com/downloads "https://www.postman.com/downloads"), you can view and set SSL certificates on a per-domain basis. If you’re using HTTPS in production, this allows your testing and development environments to mirror your production environment as closely as possible.

When you add a client certificate to the Postman app, you associate a domain with the certificate. This means that for all HTTPS requests sent to this configured domain, the certificate will be sent along with the request.

**Frequently asked questions:**

- **Wanted to sign and encrypt the payload before sending the request to the back system, and once the response received from the host needs to decrypt and verify the response payload using the JOSE package?**

The [Postman sandbox](https://www.getpostman.com/docs/postman/scripts/postman_sandbox "https://www.getpostman.com/docs/postman/scripts/postman_sandbox"), our Javascript execution environment for pre-request and test scripts, comes with support for [CryptoJS](https://code.google.com/p/crypto-js/ "https://code.google.com/p/crypto-js/"). If you need to use JOSE, you'll need to add get creative about importing the JOSE library/package into Postman, and evaluating (eval()) the function(s) needed within the pre-requests/test scripts. Here's an example of how the workaround can be done – [Postman BDD](https://github.com/BigstickCarpet/postman-bdd "https://github.com/BigstickCarpet/postman-bdd").Using a library that isn't already implemented in our sandbox would require overhead on your end, and we wouldn't be able to provide much support for project-specific questions**

- **How-to turn off all SSL checks for the postman for a specific site?**

In the settings, turn off the SSL certificate verification option is present but be sure to remember to reactivate it afterward as this is a security feature.

- **Why am I getting SSL Handshake error?** 

This is probably because of the proxy setup. Turning off the global and system proxy from settings needs to be checked.

  
- **How can I ignore SSL certificate error ‘u_nable to verify the first certificate error_’ in Newman?**

There is an option \--insecure to disable strict SSL.

`1` `newman run e_api.json -e ent_env.json --reporters`

  
_Note: Troubleshooting document for Self-signed SSL Certificate Issues can be found [here](https://support.getpostman.com/hc/en-us/articles/-%20https://blog.postman.com/2019/07/17/self-signed-ssl-certificate-troubleshooting/)_
