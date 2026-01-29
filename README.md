This repo is a static website to use when wildlifecampus.com is down for whatever reason.
Go to info@thecampusgroup.com's CloudFlare dashboard and change the DNS setting of the
"A" record for "wildlifecampus.com" to point to "185.199.108.153". Add another 3 "A"
records, pointing to "185.199.[109, 110, 111].153"

All requests to [www.]wildlifecampus.com will be redirected to this website

Once wildlifecampus.com is working again (see if test.wildlifecampus.com displays),
change the 1st "A" record to point to the webserver's IP and remove the other 3 "A" records.

**Ensure the "A" records are "proxied" and PURGE the DNS cache for instantaneous results.**
