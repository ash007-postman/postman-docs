The Postman sandbox, our Javascript execution environment for pre-request and test scripts, comes with support for CryptoJS. If you need to use JOSE, you'll need to add get creative about importing the JOSE library/package into Postman, and evaluating (eval()) the function(s) needed within the pre-requests/test scripts. Here's an example of how the workaround can be done – Postman BDD.

Using a library that isn't already implemented in our sandbox would require overhead on your end, and we wouldn't be able to provide much support for project-specific questions.

How-to turn off all SSL checks for the postman for a specific site?

In the settings, turn off the SSL certificate verification option is present but be sure to remember to reactivate it afterward as this is a security feature.

Why am I getting SSL Handshake error?

This is probably because of the proxy setup. Turning off the global and system proxy from settings needs to be checked.

How can I ignore SSL certificate error ‘unable to verify the first certificate error’ in Newman?
There is an option --insecure to disable strict SSL.

1 newman run e_api.json -e ent_env.json --reporters

Note: Troubleshooting document for Self-signed SSL Certificate Issues can be found here