# Open Redirection



It is used for Phishsing attacks, where user will get confuse where they are visiting.

Target.com/indexfile/

*   Linux

    /var/ww/indexfile/
* Windows: C:\inetpub\www\indexfile

Every path should have opening and closing.

## Example:

onlinesbi.com/[http://bing.com](http://bing.com)&#x20;

onlinesbi.com/bing.com/&#x20;

onlinesbi.com//bing.com/&#x20;

onlinesbi.com///bing.com/

When a user is provided with the above links, user will think he is visiting to a onlinesbi page to do some work but behind the user is actually redirected to the phishing page bing.com(or any fake page hosted by attacker)

Impact:

Attacker can capture or edit the sensitive information of the user without his concern.

Attacker can make this URL more reliable by using the url shortner.

Remediation:

* Disallow Offsite redirection
* whitelist the particular required URL.
* Check the referrer.
