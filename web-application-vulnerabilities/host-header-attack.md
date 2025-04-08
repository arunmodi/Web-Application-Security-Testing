# Host Header Attack

1. You have to find any URL having code 3xx. like 300 / 301/ 302 ...
2. Then you can use below three methods and see if the web page is redirecting.

a. Add X-Forwarded-Host: attacker.com

b. Set Host to attacker.com & X-Forwarded-Host to real website.

c. Set Host to attacker.com and remove x-forwarded-host.

If a web page redirects by modifying the headers as above there is a vulnerability.
