<h3 class="article-title" title="Let&rsquo;s Encrypt SSL cert auto-renewal">Let&rsquo;s Encrypt SSL cert auto-renewal</h3>
<p>Postman documentation may be hosted on your custom domain if you are on Team, Business or Enterprise plan.</p>
<p>Postman automatically generates an SSL certificate using LetsEncrypt for your documentation on a custom domain if your domain has no CAA records. If your domain has CAA records set, then LetsEncrypt needs an explicit CAA record to issue a certificate for that domain. To enable LetsEncrypt to issue this certificate, refer to the&nbsp;<a class="sc-lhVmIH kklaKG" title="https://letsencrypt.org/docs/caa" href="https://letsencrypt.org/docs/caa">LetsEncrypt Documentation</a>.</p>
<p>&nbsp;</p>
<p><span class="wysiwyg-font-size-large"><strong>Frequently asked questions:</strong></span></p>
<p><strong>How long are these SSL Certificates valid for?</strong></p>
<p>Certificates are generated with a 90-day expiry date.</p>
<p>&nbsp;</p>
<p><strong>How &amp; when does 'Let&rsquo;s Encrypt' renew SSL certificates for published documentation?</strong></p>
<p>The certificate gets renewed at 7 days from the expiry.</p>
<p>&nbsp;</p>
<p><strong>Do I need to perform any steps to renew the certificate?&nbsp;</strong></p>
<p>Certificates are renewed automatically, no manual steps are required.</p>
<p>&nbsp;</p>
<p><strong>Who issues Certificate on the published documentation?</strong></p>
<p>Certificates for documentation hosted one custom domain are issued via&nbsp;<strong>Let&rsquo;s Encrypt</strong>.</p>
<p>For the ones on documenter(default), uses the Amazon issued certificate for the *.getpostman.com domain.</p>
<p>&nbsp;</p>
<p><strong>How do we enable SSL for documentation on a custom domain?</strong></p>
<p>Once the documentation is published on a custom domain, SSL is automatically set up and wouldn't require any additional steps further.</p>